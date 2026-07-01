# O Termo Geral de uma PA — achar sem listar

> **Curso:** *Raízes do Saber: Princípios de Matemática* — Prof. Dr. Deividi Pansera
> **Tema:** Progressões e Logaritmos — Aula 13 / Lista 8 (PA)
> **Como nasceu:** derivação hands-on, construída pela contagem de passos — a fórmula emergiu
> da conta, não o contrário. Fecha a "ponta solta" de [soma-da-pa-gauss.md](soma-da-pa-gauss.md).

---

## A pergunta que a fórmula responde

Dada a PA `4, 7, 10, 13, …`, qual é o **100º** termo? Listar cem números é bruteza, não
método. O termo geral é o atalho que respeita o *porquê*: em vez de caminhar termo a termo,
**saltamos direto** para a posição desejada.

## A receita, descoberta pela contagem

Para ir do primeiro termo até um termo qualquer, você dá **passos** do tamanho da razão. A
observação-chave:

```
   do 1º ao 2º termo  → 1 passo
   do 1º ao 3º termo  → 2 passos
   do 1º ao 10º termo → 9 passos
   do 1º ao nº termo  → (n − 1) passos
```

É o **fencepost** de novo, agora do avesso: entre 10 postes há 9 vãos, e são os **vãos** (os
passos) que se percorrem. Por isso `n − 1`, e não `n`. (Compare com a *contagem* de termos, que
usava `+1`: são as duas faces do mesmo mourão-e-vão.)

Daí a receita, em palavras:

```
   termo que eu quero  =  (primeiro termo)  +  (quantos passos) × (tamanho do passo)
```

## Verificações feitas à mão (PA: 4, 7, 10, 13, … com passo 3)

```
   10º termo :   4 + (10 − 1) × 3  =  4 + 9  × 3  =  4 + 27   =   31
  100º termo :   4 + (100 − 1) × 3 =  4 + 99 × 3  =  4 + 297  =  301
```

Conferência do 10º pela contagem a partir de um termo visível (o 4º = 13):
`13 + 6 × 3 = 31`. ✔ (mesmo resultado, outro ponto de partida.)

## A fórmula (a receita em taquigrafia)

Batizando os ingredientes:

```
   a₁  =  primeiro termo         (aqui, 4)
   d   =  razão / tamanho do passo (aqui, 3)   — "d" de diferença
   n   =  a posição desejada     (10, 100, …)

   ┌──────────────────────────────────┐
   │   aₙ  =  a₁  +  (n − 1) · d       │
   └──────────────────────────────────┘
```

`aₙ` significa apenas "o termo da posição n". A fórmula **não** é regra a decorar: é o resumo da
conta que já sabemos fazer. Esquecê-la não é problema — primeiro termo, mais passos vezes o
tamanho do passo, e ela renasce.

## Síntese para a memória

1. **Quantos passos** do 1º ao nº termo? `n − 1` (fencepost: vãos, não postes).
2. **Termo geral:** `aₙ = a₁ + (n − 1) · d`.
3. Com a [soma de Gauss](soma-da-pa-gauss.md), fecham-se as duas operações centrais da PA:
   **achar** um termo qualquer e **somar** os termos.

> A fórmula boa é aquela que você poderia ter inventado. Esta, você inventou — contando passos.

---

## Ponta solta (próximo passo)

Com o termo geral na mão, abre-se a **PG (Progressão Geométrica)**: lá o "passo" não é uma
**soma** constante (`+d`), mas uma **multiplicação** constante (`×q`). A pergunta análoga —
"qual o nº termo?" — troca `(n − 1) × d` por `q` elevado a `(n − 1)`. Mesmo esqueleto, outra
operação. É o degrau seguinte da trilha (ver [mapa-mestre](../notas/mapa-mestre-do-curso.md)).
