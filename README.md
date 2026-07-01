# RDS & ABP — Cadernos de Estudo

Caderno pessoal e versionado de estudos de dois cursos do **Prof. Dr. Deividi Pansera**:

- **Raízes do Saber** — Princípios de Matemática (aritmética, álgebra, progressões, logaritmos);
- **A Arte do Bem Pensar** — lógica clássica (os três atos da mente).

Objetivo: organizar aulas, exercícios, anotações e resumos de forma versionada, registrando o
raciocínio por trás de cada tópico — o *porquê* antes do *como* — e acompanhando o progresso
ao longo dos cursos.

## Mapa do conhecimento

Grafo vivo de tudo o que já construímos no caderno. Atualizado a cada avanço.
**Legenda:** ✅ concluído · ⏳ próximo passo.

```mermaid
%%{init: {'theme':'dark','themeVariables':{'fontSize':'20px','fontFamily':'sans-serif','clusterBkg':'transparent','clusterBorder':'#9aa0a6'}}}%%
graph TD
    TRAD["Tradição clássica"] --> RAIZ
    RAIZ(["🎓 Cursos<br/>Prof. Deividi Pansera"]) --> RDS
    RAIZ --> ABP
    RAIZ --> MAPA["🗺️ Mapa-mestre"]

    subgraph RDS ["📐 RDS · Matemática"]
        FUND["Fundamentos<br/>ℤ → ℚ → ℝ"]
        PA["Progressão Aritmética"]
        PASOMA["✅ Soma da PA · Gauss"]
        PATERMO["✅ Termo geral"]
        PG["⏳ Prog. Geométrica"]
        LOG["⏳ Logaritmos"]
        FUND --> PA
        PA --> PASOMA
        PA --> PATERMO
        PA --> PG
        PG --> LOG
        PASOMA -. "fencepost +1/−1" .- PATERMO
    end

    subgraph ABP ["🦉 ABP · Lógica Clássica"]
        ATO1["Ato 1 · Apreensão"]
        ARQ["✅ Arquitetura da lógica"]
        ATO2["Ato 2 · Juízo"]
        QUAD["✅ Quadrado das Oposições"]
        ATO3["⏳ Ato 3 · Silogismo"]
        ATO1 --> ARQ --> ATO2 --> QUAD --> ATO3
    end

    RDS --> BIB
    ABP --> BIB
    subgraph BIB ["📚 Biblioteca · aplicação"]
        APOSTOL["Apostol · Cálculo"]
        AXLER["Axler · Álgebra Linear"]
        ROSS["Ross · Probabilidade"]
    end

    classDef done fill:#2f9e44,stroke:#8ce99a,color:#ffffff;
    classDef todo fill:#e8590c,stroke:#ffc078,color:#ffffff;
    classDef hub fill:#3b5bdb,stroke:#91a7ff,color:#ffffff;
    class PASOMA,PATERMO,ARQ,QUAD done;
    class PG,LOG,ATO3 todo;
    class RAIZ,MAPA hub;

    style RDS fill:transparent,stroke:#9aa0a6,stroke-width:1px
    style ABP fill:transparent,stroke:#9aa0a6,stroke-width:1px
    style BIB fill:transparent,stroke:#9aa0a6,stroke-width:1px
```

**Documentos:**
[Arquitetura da lógica clássica](resumos/arquitetura-da-logica-classica.md) ·
[Quadrado das Oposições](resumos/quadrado-das-oposicoes.md) ·
[Soma da PA (Gauss)](resumos/soma-da-pa-gauss.md) ·
[Termo geral da PA](resumos/termo-geral-da-pa.md) ·
[Mapa-mestre do curso](notas/mapa-mestre-do-curso.md) ·
[Biblioteca matemática](notas/biblioteca-matematica-e-o-curso.md)

## Estrutura

```
aulas/        # material e anotações por aula (uma pasta/arquivo por aula)
exercicios/   # exercícios resolvidos
listas/       # listas de exercícios / problem sets
notas/        # anotações livres, dúvidas, insights
resumos/      # resumos e fórmulas por tópico
```

## Convenções sugeridas

- Nomeie arquivos com data/tópico, ex.: `aulas/2026-06-29-limites.md`.
- Um resumo por tópico em `resumos/` (ex.: `resumos/derivadas.md`).
- Anote dúvidas em `notas/` para revisar depois.

---

*Estudo pessoal. Sem fins comerciais.*

*Os materiais de base utilizados são créditos do curso Raízes do Saber, do Prof. Dr. Deividi Pansera.*
