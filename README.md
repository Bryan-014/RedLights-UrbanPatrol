# Red Lights: Urban Patrol

## 1. Visão Geral

**Nome do Projeto:** Red Lights: Urban Patrol
**Gênero:** Simulador / Ação em Mundo Aberto
**Plataforma:** PC
**Engine:** Unity

### Referências

* Sistema policial de Grand Theft Auto IV
* Dinâmica de equipe da série The Rookie

### Descrição

Red Lights: Urban Patrol é um simulador policial em mundo aberto focado em tomada de decisão, progressão de carreira e resposta a ocorrências dinâmicas. O jogador inicia como patrulheiro e evolui até cargos mais estratégicos, como detetive.

---

# 2. Game Design Overview (GDD)

## 2.1 Core Loop

1. Receber ocorrência
2. Deslocar-se até o local
3. Avaliar a situação
4. Tomar decisões (diálogo, ação, reforço)
5. Resolver ocorrência
6. Receber recompensa/penalidade
7. Evoluir personagem

## 2.2 Pillars (Pilares do Jogo)

* Realismo operacional
* Tomada de decisão com consequências
* Progressão de carreira significativa
* Variedade de ocorrências

---

# 3. Sistemas do Jogo

## 3.1 Sistema de Ocorrências

* Spawn procedural + eventos contextuais
* Classificação por risco (baixo, médio, alto)
* Prioridade dinâmica

## 3.2 Sistema de Decisão

* Escolhas impactam:

  * XP
  * Reputação
  * Progressão

## 3.3 Sistema de IA

* Civis com comportamentos variados
* Suspeitos com estados (fuga, agressivo, rendição)
* Parceiros controlados por IA (futuro multiplayer)

## 3.4 Sistema de Progressão

* XP por desempenho
* Penalidades por conduta inadequada
* Desbloqueio de funções

---

# 4. Arquitetura Técnica (Unity)

## 4.1 Estrutura Base

* Padrão de arquitetura: Component-Based + ScriptableObjects
* Separação por sistemas:

  * Gameplay
  * AI
  * UI
  * Input

## 4.2 Sistemas Principais

* Game Manager
* Event Manager (Ocorrências)
* Player Controller
* Vehicle Controller
* AI Controller

## 4.3 Ferramentas

* Unity Input System
* NavMesh (IA)
* ScriptableObjects para dados

---

# 5. Roadmap de Desenvolvimento

## Fase 1 - Protótipo (1-2 meses)

* Movimento do personagem
* Direção de viatura
* Sistema simples de ocorrência
* UI básica

## Fase 2 - Vertical Slice (2-4 meses)

* 3 tipos de ocorrência
* Sistema de decisão
* IA básica
* Sistema de XP

## Fase 3 - Expansão (4-8 meses)

* Mapa maior
* Mais ocorrências
* Customização
* Polimento de gameplay

## Fase 4 - Multiplayer (avançado)

* Coop online
* Sincronização de eventos
* Sistema de lobby

---

# 6. MVP (Produto Mínimo Viável)

## Conteúdo

* 1 mapa pequeno
* 1 viatura
* 3 tipos de ocorrência

## Objetivo

Validar o loop principal e a diversão do jogo

---

# 7. Estrutura de Projeto

```
/Project
  /Assets
    /Scripts
    /Prefabs
    /Scenes
    /UI
    /Audio
  /Docs
  /Build
```

---

# 8. Backlog Inicial

## Alta Prioridade

* Sistema de direção
* Sistema de ocorrências
* Navegação até destino

## Média Prioridade

* Sistema de decisão
* IA básica

## Baixa Prioridade

* Customização
* Polimento visual

---

# 9. Publicação (Steam Ready)

## Descrição Curta

Simulador policial em mundo aberto focado em ocorrências dinâmicas e decisões com impacto.

## Tags Sugeridas

* Simulation
* Open World
* Police
* Action
* Multiplayer

---

# 10. Próximos Passos Imediatos

1. Criar projeto Unity
2. Implementar controle de veículo
3. Criar sistema básico de ocorrência
4. Testar primeiro loop jogável

---

# 11. Considerações Finais

Manter escopo controlado é essencial. O foco deve ser sempre validar o gameplay principal antes de expandir funcionalidades.
