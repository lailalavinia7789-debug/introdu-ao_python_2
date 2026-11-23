# Aulas de Python — Aulas 21 a 40

Este repositório reúne os exercícios desenvolvidos nas aulas 21 a 40. Os exemplos praticam operações matemáticas, estruturas condicionais (`if`, `elif`, `else`), ciclos de repetição (`for` e `while`), validação de entradas, contadores e formatação de resultados em Python.

## Conteúdos por aula

| Aula | Tema | Descrição |
|---:|---|---|
| 21 | Calculadora simples | Recebe dois números e permite escolher entre soma, divisão, subtração e multiplicação. |
| 22 | Simulação de empréstimo para habitação | Calcula a prestação mensal de uma casa e verifica se ultrapassa 30% do salário do comprador. |
| 23 | Cálculo do consumo de eletricidade | Calcula o valor a pagar pela energia de acordo com o tipo de instalação e a quantidade de kWh consumida. |
| 24 | Preços de frutas | Apresenta uma lista de frutas e mostra o preço correspondente à opção escolhida. |
| 25 | Identificação de número par ou ímpar | Verifica se um número inteiro é par ou ímpar através do resto da divisão por 2. |
| 26 | Ordenação de três números | Recebe três valores e apresenta-os por ordem crescente, verificando também se são negativos. |
| 27 | Cálculo de custos de viagem | Calcula os custos estimados de combustível e portagens para as estradas A1, A20 ou A21. |
| 28 | Cálculo do vencimento líquido | Calcula os descontos sobre o vencimento bruto e apresenta o vencimento líquido. |
| 29 | Cálculo da nota final | Calcula a média ponderada de quatro testes e de um exame e indica a situação do aluno. |
| 30 | Números pares e ímpares com ciclo | Percorre os números de 1 a 10 e identifica quais são pares e quais são ímpares. |
| 31 | Classificação de alunos | Pede as notas de cinco alunos, valida se estão entre 0 e 20 e apresenta a classificação. |
| 32 | Classificação de temperaturas | Recebe as temperaturas de sete dias e classifica cada uma como fria, amena, quente ou muito quente. |
| 33 | Preço de bilhetes por idade | Recebe a idade de cinco pessoas e indica o tipo de entrada correspondente. |
| 34 | FizzBuzz | Percorre uma sequência de números e apresenta “Fizz”, “Buzz” ou “FizzBuzz” conforme a divisibilidade por 3 e 5. |
| 35 | Contagem de números | Lê 10 números inteiros e conta quantos são positivos, negativos ou zero. |
| 36 | Descontos em compras | Lê o valor de 5 compras e calcula o desconto e o total a pagar. |
| 37 | Tabuada e classificação | Mostra os produtos de um número por multiplicadores de 0 a 9 e classifica cada resultado. |
| 38 | Jogo do número secreto | Dá até 5 tentativas para adivinhar o número secreto, indicando se o palpite é maior ou menor. |
| 39 | Calculadora | Permite realizar 3 operações matemáticas escolhidas pelo utilizador. |
| 40 | Classificação de números com `while` | Lê 5 números inteiros e indica se cada um é positivo, negativo ou zero. |

## Descrição das aulas 35 a 40

### Aula 35 — Contar positivos, negativos e zeros

O programa pede ao utilizador 10 números inteiros. Conforme o valor introduzido, incrementa um dos três contadores:

- `positivos`: números superiores a zero;
- `negativos`: números inferiores a zero;
- `zeros`: números iguais a zero.

No final, apresenta o total de cada categoria.

**Conceitos praticados:** variáveis contadoras, `for`, `input()`, conversão com `int()` e estruturas condicionais.

### Aula 36 — Cálculo de descontos

O programa processa 5 compras. Para cada valor introduzido:

- Se o valor for negativo, apresenta uma mensagem de compra inválida.
- Se for inferior a 50 €, não aplica desconto.
- Se for igual ou superior a 50 € e inferior a 100 €, aplica 5%.
- Se for igual ou superior a 100 €, aplica 10%.

Depois calcula o valor do desconto e o total a pagar.

**Conceitos praticados:** ciclos `for`, condições encadeadas, percentagens, operações aritméticas e formatação de valores decimais.

### Aula 37 — Tabuada com classificação

O utilizador introduz um número inteiro. O programa multiplica esse número pelos valores de 0 a 9 e apresenta cada operação.

Cada produto é classificado:
- como múltiplo de 3, se for divisível por 3;
- caso contrário, como par, se for divisível por 2;
- caso contrário, como ímpar.

A condição de múltiplo de 3 é verificada primeiro. Por isso, um resultado que seja simultaneamente múltiplo de 3 e par recebe a classificação **“Múltiplo de 3”**.

**Conceitos praticados:** ciclo `for`, operador módulo (`%`), condições `if`/`elif`/`else` e multiplicação.

### Aula 38 — Jogo do número secreto

O número secreto está definido como `7`. O utilizador tem até 5 tentativas para o adivinhar.

Em cada tentativa:
- Se acertar, o programa apresenta “Acertou!” e termina o ciclo com `break`.
- Se o palpite for inferior ao número secreto, informa que o número é maior.
- Se o palpite for superior, informa que o número é menor.

A variável `acertou` regista se o utilizador conseguiu adivinhar. Se as tentativas terminarem sem sucesso, o programa revela o número secreto.

**Conceitos praticados:** ciclo `for`, condições, variável booleana, `break` e negação lógica com `not`.

### Aula 39 — Calculadora com várias operações

O programa permite realizar 3 operações. Em cada uma, pede dois números e um operador. Estão previstas as operações de adição (`+`), subtração (`-`), multiplicação (`*`) e divisão (`/`).

Na divisão, verifica se o segundo número é zero. Se for, apresenta uma mensagem de erro e passa à operação seguinte com `continue`. Também apresenta uma mensagem caso o operador não seja válido.

**Conceitos praticados:** ciclo `for`, seleção de operações com `if`/`elif`/`else`, operadores aritméticos, validação e `continue`.

> **Nota sobre o código:** na condição da multiplicação, o ficheiro da aula contém `elif operador == ""` em vez de `elif operador == "*"`. Assim, introduzir `*` não ativa a multiplicação. Para a opção funcionar como previsto, essa condição deve comparar com `"*"`.

### Aula 40 — Classificar números com `while`

O programa utiliza um ciclo `while` para pedir 5 números inteiros. Para cada número, indica se é positivo, negativo ou zero.

A variável `contador` começa em zero e aumenta uma unidade em cada repetição. O ciclo termina quando o contador deixa de ser inferior a 5. No fim, é apresentada a mensagem “O processamento terminou.”

**Conceitos praticados:** ciclo `while`, contador, incremento (`+= 1`), condições e leitura de números inteiros.

## Conceitos de Python praticados

Ao longo destas aulas são praticados os seguintes conceitos:

- Variáveis e tipos de dados (`int`, `float` e `str`).
- Entrada de dados com `input()` e apresentação de resultados com `print()`.
- Conversão de valores com `int()` e `float()`.
- Operações aritméticas.
- Cálculos com percentagens e médias.
- Operador módulo (`%`) para verificar divisibilidade e números pares ou ímpares.
- Estruturas condicionais: `if`, `elif` e `else`.
- Operadores de comparação e operadores lógicos.
- Ciclos `for` e `while`.
- Utilização de `range()` em ciclos.
- Contadores e incremento de variáveis.
- `break` para terminar imediatamente um ciclo.
- `continue` para avançar para a repetição seguinte.
- Formatação de resultados com f-strings, incluindo `{valor:.2f}` para apresentar duas casas decimais.

## Requisitos

- Python 3 instalado.
- Um editor de código, como Visual Studio Code, ou outro ambiente compatível com Python.

## Como executar os exercícios

1. Descarregar ou clonar este repositório.
2. Abrir a pasta do projeto no editor de código ou no terminal.
3. Escolher o ficheiro da aula que pretende executar.
4. Executar o ficheiro com Python. Por exemplo:

   ```bash
   python aula_21.py
   ```

   Substitua `aula_21.py` pelo nome do ficheiro pretendido (`aula_22.py` até `aula_40.py`).

5. Seguir as instruções apresentadas no terminal e introduzir os valores pedidos.

## Ficheiros

```text
.
├── aula_21.py
├── aula_22.py
├── aula_23.py
├── aula_24.py
├── aula_25.py
├── aula_26.py
├── aula_27.py
├── aula_28.py
├── aula_29.py
├── aula_30.py
├── aula_31.py
├── aula_32.py
├── aula_33.py
├── aula_34.py
├── aula_35.py
├── aula_36.py
├── aula_37.py
├── aula_38.py
├── aula_39.py
├── aula_40.py
└── README.md
```

## Objetivo

Este conjunto de exercícios tem como objetivo desenvolver os conhecimentos básicos de programação em Python, praticando cálculos, decisões, validação de dados e repetições através de pequenos problemas.
