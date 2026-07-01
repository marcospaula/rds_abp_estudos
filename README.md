# RDS — Raízes do Saber

Repositório pessoal de estudos do curso de **Matemática "Raízes do Saber"**,
ministrado pelo **Prof. Dr. Deividi Pansera**.

Objetivo: organizar aulas, exercícios, anotações e resumos de forma versionada,
acompanhando o progresso ao longo do curso.

## Mapa do conhecimento

Grafo vivo de tudo o que já construímos no caderno. Atualizado a cada avanço.
**Legenda:** ✅ concluído · ⏳ próximo passo.

```mermaid
graph TD
    TRAD["Tradição clássica<br/>Sócrates · Platão · Aristóteles · Euclides"] --> RAIZ
    RAIZ(["🎓 Cursos do Prof. Dr. Deividi Pansera"]) --> RDS
    RAIZ --> ABP
    RAIZ --> MAPA["🗺️ Mapa-mestre do curso<br/>notas/mapa-mestre-do-curso.md"]

    subgraph RDS ["📐 RDS — Matemática (Raízes do Saber)"]
        FUND["Fundamentos Aritméticos<br/>ℤ → ℚ → ℝ"]
        PA["Progressão Aritmética"]
        PASOMA["✅ Soma da PA (Gauss)<br/>resumos/soma-da-pa-gauss.md"]
        PATERMO["✅ Termo geral da PA<br/>resumos/termo-geral-da-pa.md"]
        PG["⏳ Progressão Geométrica"]
        LOG["⏳ Logaritmos"]
        FUND --> PA
        PA --> PASOMA
        PA --> PATERMO
        PA --> PG
        PG --> LOG
        PASOMA -. "fencepost: +1 / −1" .- PATERMO
    end

    subgraph ABP ["🦉 ABP — Lógica Clássica (A Arte do Bem Pensar)"]
        ATO1["Ato 1 · Simples Apreensão"]
        ARQ["✅ Arquitetura da lógica clássica<br/>resumos/arquitetura-da-logica-classica.md"]
        ATO2["Ato 2 · Juízo"]
        QUAD["✅ Quadrado das Oposições<br/>resumos/quadrado-das-oposicoes.md"]
        ATO3["⏳ Ato 3 · Raciocínio (Silogismo)"]
        ATO1 --> ARQ
        ARQ --> ATO2
        ATO2 --> QUAD
        QUAD --> ATO3
    end

    RDS --> BIB
    ABP --> BIB
    subgraph BIB ["📚 Biblioteca — aplicação (a copa)"]
        BIBNOTA["notas/biblioteca-matematica-e-o-curso.md"]
        APOSTOL["Apostol · Cálculo"]
        AXLER["Axler · Álgebra Linear"]
        ROSS["Ross · Probabilidade"]
        BIBNOTA --> APOSTOL
        BIBNOTA --> AXLER
        BIBNOTA --> ROSS
    end
```

## Estrutura

```
aulas/        # material e anotações por aula (uma pasta/arquivo por aula)
exercicios/   # exercícios resolvidos
listas/       # listas de exercícios / problem sets
notas/        # anotações livres, dúvidas, insights
resumos/      # resumos e fórmulas por tópico
```

## Como usar (com o Claude Code)

Este é um projeto **separado**. Para trabalhar nele com o Claude, abra o Claude
**dentro desta pasta** (`RDS/`) — assim ele tem o próprio contexto e memória,
sem misturar com outros projetos.

## Convenções sugeridas

- Nomeie arquivos com data/tópico, ex.: `aulas/2026-06-29-limites.md`.
- Um resumo por tópico em `resumos/` (ex.: `resumos/derivadas.md`).
- Anote dúvidas em `notas/` para revisar depois.

---

*Estudo pessoal. Sem fins comerciais.*

*Os materiais de base utilizados são créditos do curso Raízes do Saber, do Prof. Dr. Deividi Pansera.*
