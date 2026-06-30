# A Soma de uma PA — reconstruída pelo método de Gauss

> **Curso:** *Raízes do Saber: Princípios de Matemática* — Prof. Dr. Deividi Pansera
> **Tema:** Progressões e Logaritmos — Aula 13 / Lista 8 (PA)
> **Como nasceu:** derivação hands-on, construída do zero pela observação — não decorada.

---

## Por que reconstruir em vez de decorar

Uma fórmula decorada é um vão sobre o abismo: sustenta enquanto a memória aguenta, e cede no
primeiro esquecimento. Uma fórmula **reconstruída** é alicerce — se um dia ela escapar, bastam
duas filas de números para erguê-la de novo. É essa a diferença entre saber *que* a fórmula é
assim e entender *por que* ela não poderia ser de outro jeito. Comecemos, como sempre, pelo
*porquê*.

## O desafio de Gauss

A lenda conta que, ainda menino, Gauss foi mandado somar todos os números de 1 a 100 — e
respondeu em segundos. O segredo não foi cálculo veloz: foi **enxergar uma estrutura**.

Escreva a soma **duas vezes** — a segunda de trás para frente — e alinhe em colunas:

```
   1  +   2  +   3  +  ...  +  98  +  99  + 100
 100  +  99  +  98  +  ...  +   3  +   2  +   1
 ───────────────────────────────────────────────
 101    101    101    ...    101    101    101
```

Cada coluna soma **101** = (primeiro + último). E há **100** colunas — uma por termo. Logo:

```
   100 colunas × 101 = 10.100      (soma escrita em DOBRO)
   10.100 ÷ 2        =  5.050      (a soma verdadeira)
```

O `÷ 2` desfaz exatamente o truque de termos escrito a fila duas vezes.

## O padrão que emergiu

```
            (primeiro + último) × (quantos termos)
   Soma  =  ──────────────────────────────────────
                            2
```

- **(primeiro + último)** → o valor que cada coluna pareada produz.
- **(quantos termos)** → o número de colunas.
- **÷ 2** → corrige a fila escrita em dobro.

## A armadilha da contagem (a regra do +1)

Quantos termos há de **7 até 20**? A intuição grita "13" (20 − 7) — e erra. A conta certa:

```
   quantos termos = último − primeiro + 1
                  =   20   −    7    + 1  =  14
```

**Por quê o +1?** Pense numa cerca: 14 mourões têm apenas 13 vãos entre eles. `último −
primeiro` conta os **vãos**; nós queremos os **mourões** (os próprios termos). O `+1` repõe o
poste da ponta que a subtração engole. (Vale para passo 1; com outro passo, há um detalhe a
mais — ver adiante.)

## Verificações feitas à mão

```
   1 + 2 + ... + 10   →  (1 + 10) × 10 ÷ 2  =  110 ÷ 2  =   55
   7 + 8 + ... + 20   →  (7 + 20) × 14 ÷ 2  =  378 ÷ 2  =  189
```

(Conferência independente: 1+…+20 = 210; 1+…+6 = 21; 210 − 21 = 189. ✔)

## Síntese para a memória

1. **Truque de Gauss** — soma em dobro, de trás para frente → cada coluna = primeiro + último.
2. **Contagem** — quantos termos = último − primeiro + 1 (conte os mourões, não os vãos).
3. **Soma da PA** — (primeiro + último) × (quantos termos) ÷ 2.

> Quem reconstrói não depende da memória; depende do entendimento. Esqueça a fórmula à vontade
> — duas filas de números a trazem de volta.

---

## Ponta solta (próximo passo)

Aqui o passo entre os termos foi sempre **1** (7, 8, 9, …). Quando o passo (a **razão**) for
outro — por exemplo 5, 10, 15, 20… —, o "(primeiro + último)" continua valendo, mas a
**contagem dos termos** já não é `último − primeiro + 1`: é preciso a fórmula do **termo geral
da PA**, que liga o primeiro termo, a razão e a posição. É o degrau seguinte da trilha.

*Ver também: [mapa-mestre-do-curso.md](../notas/mapa-mestre-do-curso.md) (onde a PA abre o
caminho para PG, Logaritmos e, mais adiante, o Cálculo).*
