# Documentação da Linguagem de Programação C-Spring

## Sumário

1. [Introdução](#introduction)
2. [Primeiros Passos](#getting-started)
3. [Módulos](#modules)
    1. [MathOperations](#mathoperations-module)
4. [Funções](#functions)
    1. [calculateSquare](#calculatesquare-function)
5. [Programa Principal](#main-program)
6. [Bibliotecas Padrão](#standard-libraries)
    1. [Terminal](#terminal-library)
    2. [Console](#console-library)
    3. [Offspring IDE](#offspring-ide)

---

## Introdução <a name="introduction"></a>

C-Spring é uma linguagem de programação projetada para ser simples, intuitiva e eficiente. É adequada para uma ampla gama de aplicações, desde pequenos scripts até desenvolvimento de software em larga escala. Esta documentação fornece uma visão geral da sintaxe e dos recursos da linguagem.

## Primeiros Passos <a name="getting-started"></a>

### Conceitos Básicos

Os programas C-Spring são organizados em módulos, e cada módulo contém funções. O programa principal é uma função especial chamada 'main'. Módulos e funções são definidos usando as palavras-chave `module` e `:FUNCTION`, respectivamente.

```c-spring
module 'NomeDoModulo';
{
    :FUNCTION 'nomeDaFuncao':
        // Corpo da função
    :END 'nomeDaFuncao';
}
```

### Exemplo de Programa

```c-spring
:INCLUDE TERMINAL AS APPLICATION:
:INCLUDE CONSOLE AS APPLICATION:
:INCLUDE OFFSPRING AS IDE:
:START:

module 'OperacoesMatematicas';
{
    :FUNCTION 'calcularQuadrado':
        :param num x;
        quadrado = calculo
            quadrado num [
                multiplicar num x por num x;
            ];
        definir resultado como num;
        :return [quadrado];
    :END 'calcularQuadrado':

    :START 'main':
        solicitar num valor como pedir("Digite um número para calcular seu quadrado:");
        resultado = calcularQuadrado(valor);
        imprimir("O quadrado de [valor] é [resultado]");
        imprimir("Fim do programa");
    :END 'main':
}

:END:
```

Neste exemplo, temos um módulo chamado 'OperacoesMatematicas' com uma função 'calcularQuadrado' e o programa principal na função 'main'.

## Módulos <a name="modules"></a>

Os módulos são usados para organizar o código em unidades lógicas. Cada módulo encapsula um conjunto de funções e variáveis relacionadas.

### Módulo MathOperations <a name="mathoperations-module"></a>

O módulo 'MathOperations' fornece funções matemáticas.

## Funções <a name="functions"></a>

Funções são blocos de código que realizam tarefas específicas. Elas podem receber parâmetros, executar um conjunto de instruções e retornar um valor.

### Função calculateSquare <a name="calculatesquare-function"></a>

A função 'calculateSquare' calcula o quadrado de um número fornecido.

```c-spring
:FUNCTION 'calcularQuadrado':
    :param num x;
    quadrado = calculo
        quadrado num [
            multiplicar num x por num x;
        ];
    definir resultado como num;
    :return [quadrado];
:END 'calcularQuadrado':
```

## Programa Principal <a name="main-program"></a>

O programa principal é uma função especial chamada 'main'. É o ponto de entrada do programa.

```c-spring
:START 'main':
    // Código do programa principal
:END 'main':
```

## Bibliotecas Padrão <a name="standard-libraries"></a>

C-Spring inclui bibliotecas padrão que fornecem funcionalidades comuns.

### Biblioteca Terminal <a name="terminal-library"></a>

A biblioteca `TERMINAL` permite interação com o terminal.

### Biblioteca Console <a name="console-library"></a>

A biblioteca `CONSOLE` fornece funções para entrada e saída no console.

### Offspring IDE <a name="offspring-ide"></a>

A biblioteca `OFFSPRING` integra-se ao ambiente de desenvolvimento Offspring, oferecendo um ambiente de desenvolvimento abrangente.
