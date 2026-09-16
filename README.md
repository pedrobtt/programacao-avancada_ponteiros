# Ponteiros em C — 30 Exercícios Resolvidos

Coletânea de **30 problemas resolvidos** sobre ponteiros, aritmética de endereços, alocação dinâmica e gerenciamento de memória em C — incluindo questões do **ENADE**.

Cada arquivo é autocontido, com o enunciado no topo e a resolução comentada linha a linha, justificando *por que* cada expressão se comporta daquela forma.

**Stack:** C · Ponteiros · Aritmética de Ponteiros · Alocação Dinâmica · Estruturas de Dados

---

## Como executar

Cada questão compila de forma independente:

```bash
gcc -o questao01 questao01.c
./questao01
```

Todas de uma vez:

```bash
for f in questao*.c; do gcc -o "${f%.c}" "$f"; done
```

---

## Índice

### Fundamentos e aritmética de ponteiros

| # | Arquivo | Problema |
|---|---|---|
| 01 | [`questao01.c`](questao01.c) | Análise de trecho de programa com ponteiros |
| 02 | [`questao02.c`](questao02.c) | Previsão de saída com endereço fixo — `p`, `p+1`, `*p+2`, `**&p` |
| 03 | [`questao03.c`](questao03.c) | Validade de expressões entre variáveis `int` e ponteiros `int*` |
| 04 | [`questao04.c`](questao04.c) | Rastreamento de 14 trechos (a–n) com múltiplos ponteiros |
| 07 | [`questao07.c`](questao07.c) | Previsão de saída e verificação por compilação |
| 09 | [`questao09.c`](questao09.c) | Interpretação de declarações de ponteiros |
| 12 | [`questao12.c`](questao12.c) | Previsão de saída de programa com indireção |

### Ponteiro para ponteiro e indireção múltipla

| # | Arquivo | Problema |
|---|---|---|
| 05 | [`questao05.c`](questao05.c) | Depuração: por que a saída esperada não é impressa (`char**`) |
| 06 | [`questao06.c`](questao06.c) | Saída de programa com `char **p`, assumindo `int` de 4 bytes |
| 14 | [`questao14.c`](questao14.c) | Justificativa da saída `22` com `int`, `int*` e `int**` |
| 28 | [`questao28.c`](questao28.c) | Expressão `*--*++c + 3` sobre ponteiro triplo de strings |
| 30 | [`questao30.c`](questao30.c) | Matriz 3D dinâmica com `int***` — alocação, modificação e liberação |

### Vetores, matrizes e strings

| # | Arquivo | Problema |
|---|---|---|
| 08 | [`questao08.c`](questao08.c) | Quais expressões referenciam corretamente elementos de um vetor |
| 13 | [`questao13.c`](questao13.c) | Aritmética de endereços sobre vetor de 4 elementos |
| 15 | [`questao15.c`](questao15.c) | Saída de matriz 4×3 — `x+3`, `*(x+3)`, `*(x+2)+3` |
| 16 | [`questao16.c`](questao16.c) | Validade de 7 operações sobre arrays de `float` e ponteiros |
| 23 | [`questao23.c`](questao23.c) | Soma de dois vetores com alocação dinâmica |
| 24 | [`questao24.c`](questao24.c) | Multiplicação matricial `C = A×B` com matrizes linearizadas |

### Alocação dinâmica e memory leak

| # | Arquivo | Problema |
|---|---|---|
| 10 | [`questao10.c`](questao10.c) | Análise de três programas distintos |
| 11 | [`questao11.c`](questao11.c) | Correção de `struct` acessada por ponteiro |
| 17 | [`questao17.c`](questao17.c) | O que é memory leak — exemplo e correção |
| 25 | [`questao25.c`](questao25.c) | **ENADE 2023** — identificação de vazamento de memória |

### Ponteiros para função e ordenação

| # | Arquivo | Problema |
|---|---|---|
| 18 | [`questao18.c`](questao18.c) | Ponteiro para função — passando `somar` e `subtrair` como argumento |
| 19 | [`questao19.c`](questao19.c) | Ordenação de `n` valores com bubble sort e alocação dinâmica |
| 20 | [`questao20.c`](questao20.c) | Reimplementação com `qsort()` e função de comparação |
| 21 | [`questao21.c`](questao21.c) | Implementação de um `qsort` genérico próprio, crescente e decrescente |
| 22 | [`questao22.c`](questao22.c) | Medição de tempo de execução e comparação com o `qsort()` nativo |

### Sistemas embarcados e ENADE

| # | Arquivo | Problema |
|---|---|---|
| 26 | [`questao26.c`](questao26.c) | **ENADE 2023** — posições de memória em sistemas embarcados |
| 27 | [`questao27.c`](questao27.c) | **ENADE 2021** — análise de busca em vetor (linear vs. binária) |
| 29 | [`questao29.c`](questao29.c) | Controle de matriz de LEDs 8×8 via manipulação de bits |

---

## Contexto

Exercícios da disciplina de **Programação Avançada** — Engenharia de Computação, UFRN.
Resolvidos e versionados incrementalmente ao longo de 67 commits.
