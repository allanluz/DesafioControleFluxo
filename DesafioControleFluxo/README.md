# DesafioControleFluxo

## Descrição
Este projeto foi desenvolvido como um exercício de controle de fluxo em Java. O sistema `DesafioControleFluxo` recebe dois números inteiros como parâmetros de entrada via terminal e, em seguida, imprime uma sequência de números incrementados de acordo com a diferença entre os parâmetros. Caso o primeiro número seja maior que o segundo, o sistema lança uma exceção personalizada chamada `ParametrosInvalidosException`, alertando o usuário sobre a condição inválida.

## Estrutura do Projeto
O projeto consiste em duas classes principais:
- **Contador.java**: Classe principal que executa a leitura dos parâmetros e realiza a lógica de contagem.
- **ParametrosInvalidosException.java**: Classe de exceção personalizada para validar se o segundo parâmetro é maior que o primeiro.

## Requisitos
- **Java JDK 8** ou superior
- **IDE** (recomendado) ou terminal para execução do programa

## Como Executar
1. Clone o repositório ou faça o download dos arquivos.
2. Compile as classes `Contador.java` e `ParametrosInvalidosException.java`.
3. Execute a classe `Contador` no terminal ou IDE, fornecendo dois números inteiros como entrada.

### Exemplo de Execução
No terminal:

javac Contador.java ParametrosInvalidosException.java
java Contador


Ao executar, o sistema pedirá dois números inteiros como entrada.

### Entrada e Saída Esperadas

#### Caso 1: Entrada Válida
Se o primeiro número for 12 e o segundo número for 30, a saída será:

Digite o primeiro parâmetro
12
Digite o segundo parâmetro
30
Imprimindo o número 1
Imprimindo o número 2
...
Imprimindo o número 18


#### Caso 2: Parâmetro Inválido
Se o primeiro número for maior que o segundo, por exemplo, `30` e `12`, a saída será:

Digite o primeiro parâmetro
30
Digite o segundo parâmetro
12
O segundo parâmetro deve ser maior que o primeiro


## Estrutura do Código

### Contador.java
Esta classe contém a lógica do programa:
- Lê dois inteiros do terminal.
- Lança uma exceção personalizada `ParametrosInvalidosException` se o primeiro parâmetro for maior que o segundo.
- Caso contrário, calcula a diferença entre os dois números e usa um loop `for` para imprimir a contagem.

### ParametrosInvalidosException.java
Define a exceção personalizada que estende `Exception`, com a mensagem específica `"O segundo parâmetro deve ser maior que o primeiro"`.

## Considerações
Este projeto demonstra controle de fluxo em Java, uso de exceções personalizadas e prática com entrada/saída no console. É um exemplo didático para aprendizado de estruturas de decisão e validações de entrada em sistemas de linha de comando.

## Autor
Projeto desenvolvido por Allan Luz.
