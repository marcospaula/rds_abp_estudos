# O Quadrado das Oposições

> **Curso:** *A Arte do Bem Pensar* — Prof. Dr. Deividi Pansera
> **Aula:** 04 — Julgamento / Propriedades das Proposições
> **Fonte:** lousa da aula (captura) + tradição aristotélica (sistematizada por Boécio na Escolástica)

---

## Por que isto importa

Antes de raciocinar, o intelecto **julga** — afirma ou nega algo de algo. Toda proposição
categórica diz que um **sujeito (S)** está, ou não está, contido num **predicado (P)**. O
Quadrado das Oposições é o mapa que organiza, com rigor geométrico, **como a verdade de uma
proposição condiciona a verdade das outras**. Não é adorno: é a arquitetura que sustenta a
inferência imediata. Quem domina o Quadrado deixa de "achar" e passa a **deduzir**.

## As quatro proposições categóricas

Dos pares latinos **AffIrmo** (afirmo → vogais **A**, **I**) e **nEgO** (nego → **E**, **O**)
nascem os quatro tipos. Tome S = "homens", P = "mortais":

| Tipo | Sigla da lousa | Quantidade · Qualidade | Forma | Exemplo |
|:---:|:---:|---|---|---|
| **A** | U.A. | Universal **Afirmativa** | Todo S é P | Todo homem é mortal |
| **E** | U.N. | Universal **Negativa** | Nenhum S é P | Nenhum homem é mortal |
| **I** | P.A. | Particular **Afirmativa** | Algum S é P | Algum homem é mortal |
| **O** | P.N. | Particular **Negativa** | Algum S não é P | Algum homem não é mortal |

## O diagrama

```
            CONTRÁRIAS  (não ambas V; podem ambas F)
        A (U.A.) ───────────────────────────── E (U.N.)
        │  ╲                               ╱   │
        │    ╲                           ╱     │
        │      ╲                       ╱       │
   sub- │        ╲   CONTRADITÓRIAS  ╱         │ sub-
   alt. │          ╲    (V ⇄ F)    ╱           │ alt.
   V↓F↑ │            ╲           ╱             │ V↓F↑
        │              ╲       ╱               │
        │                ╳   (cruzam)          │
        │              ╱       ╲               │
        I (P.A.) ───────────────────────────── O (P.N.)
            SUBCONTRÁRIAS (não ambas F; podem ambas V)
```

## As quatro relações (as regras de ouro)

1. **Contraditórias** — diagonais: **A↔O** e **E↔I**
   Sempre com **valores opostos**. Se uma é verdadeira, a outra é necessariamente falsa, e
   vice-versa. É a oposição mais forte: não admite meio-termo.
   *“Todo homem é mortal” (A) contradiz “Algum homem não é mortal” (O).*

2. **Contrárias** — aresta superior: **A · E** (as duas universais)
   **Não podem ser ambas verdadeiras**, mas **podem ser ambas falsas**.
   (Lousa: "V→F ou ambas F".) Se "Todo S é P" é verdadeira, "Nenhum S é P" é falsa — mas as
   duas podem falhar juntas (ex.: "Todo animal é gato" e "Nenhum animal é gato": ambas falsas).

3. **Subcontrárias** — aresta inferior: **I · O** (as duas particulares)
   **Não podem ser ambas falsas**, mas **podem ser ambas verdadeiras**.
   (Lousa: "F→V ou ambas V".) Espelho exato das contrárias.

4. **Subalternas** — laterais: **A→I** e **E→O** (universal sobre sua particular)
   - A **verdade desce** (V↓): se a universal é verdadeira, a particular também é.
     Se "Todo homem é mortal" (A) é V, então "Algum homem é mortal" (I) é V.
   - A **falsidade sobe** (F↑): se a particular é falsa, a universal também é.
     Se "Algum homem é mortal" (I) é F, então "Todo homem é mortal" (A) é F.
   - **Atenção:** o inverso não vale. A verdade da particular **não** garante a da universal,
     nem a falsidade da universal garante a da particular.

## Tabela de inferência imediata

Dada a verdade de **uma** proposição, o que se segue para as demais:

| Se… é V | A | E | I | O |
|:---:|:---:|:---:|:---:|:---:|
| **A** verdadeira | V | F | V | F |
| **E** verdadeira | F | V | F | V |
| **I** verdadeira | ? | F | V | ? |
| **O** verdadeira | F | ? | ? | V |

*( ? = indeterminado: a relação não força um valor.)*

## Síntese para a memória

- **Diagonais** = contradição → **opostos sempre**.
- **Topo** (universais) = contrárias → **nunca ambas V**.
- **Base** (particulares) = subcontrárias → **nunca ambas F**.
- **Lados** = subalternas → **verdade desce, falsidade sobe**.

> Decorar os quatro nomes é o de menos. O que se busca é **enxergar a estrutura**: uma vez
> compreendida, a inferência deixa de ser esforço e passa a ser visão. É esse o ginásio que
> a lógica clássica oferece à mente.

---

*Ver também o material original: `material/Cursos Deividi Pansera/Arte do Bem Pensar/Módulo 2/Aula 02/quadrado das oposicoes - aristoteles.png`. Tópico vizinho: conversão, obversão e contraposição (inferências imediatas).*
