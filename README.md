# Relatório: Explicação do Algoritmo

## Introdução

Este relatório descreve o funcionamento de um programa desenvolvido em linguagem C que realiza operações aritméticas e verificações lógicas com três números inteiros fornecidos pelo usuário. O objetivo é demonstrar o uso prático dos diferentes tipos de operadores disponíveis na linguagem C.

## Descrição do Algoritmo

O programa foi estruturado de forma sequencial, seguindo uma lógica simples e direta. Primeiro, ele solicita ao usuário que informe três números inteiros através da função `scanf()`. Esses valores são armazenados em variáveis do tipo `int` chamadas `num1`, `num2` e `num3`.

### Operadores Aritméticos

Após a entrada dos dados, o programa realiza quatro operações aritméticas básicas:

**Soma**: Utiliza o operador `+` para somar os três números. A expressão `soma = num1 + num2 + num3` calcula o resultado total da adição dos três valores.

**Subtração**: Usa o operador `-` para subtrair sequencialmente os números. A expressão `subtracao = num1 - num2 - num3` realiza a subtração do segundo e terceiro número do primeiro.

**Multiplicação**: Aplica o operador `*` para multiplicar os três números. A expressão `multiplicacao = num1 * num2 * num3` calcula o produto dos três valores.

**Divisão**: Utiliza o operador `/` para dividir os números. Porém, antes de realizar a divisão, o programa verifica se os divisores (num2 e num3) são diferentes de zero, evitando assim um erro matemático. Quando a condição é satisfeita, a expressão `divisao = (float)num1 / num2 / num3` realiza a divisão sequencial, convertendo o primeiro número para float para garantir precisão no resultado decimal.

### Operadores Relacionais

O programa também realiza comparações entre os números usando operadores relacionais:

**Maior que (`>`)**: Compara se o primeiro número é maior que o segundo através da expressão `num1 > num2`. Se a condição for verdadeira, exibe uma mensagem informando que o primeiro número é maior; caso contrário, informa que não é maior.

**Menor que (`<`)**: Compara se o segundo número é menor que o terceiro usando `num2 < num3`. Similar à comparação anterior, exibe uma mensagem apropriada baseada no resultado da verificação.

### Operadores Lógicos

Para demonstrar o uso de operadores lógicos, o programa verifica duas condições combinadas:

**Operador AND (`&&`)**: Verifica se duas condições são verdadeiras simultaneamente. Primeiro, verifica se o primeiro número é positivo usando `num1 > 0`. Em seguida, verifica se o segundo número é par através do operador módulo (`%`), que retorna o resto da divisão por 2. Se o resto for zero, o número é par. A expressão completa `primeiro_positivo && segundo_par` só será verdadeira se ambas as condições forem satisfeitas.

**Operador Módulo (`%`)**: Embora seja um operador aritmético, foi utilizado aqui para verificar a paridade do número. A expressão `num2 % 2 == 0` verifica se o resto da divisão do segundo número por 2 é igual a zero, indicando que o número é par.

## Estrutura de Controle

O programa utiliza estruturas condicionais `if-else` para controlar o fluxo de execução. Essas estruturas permitem que o programa tome decisões baseadas nas condições verificadas, exibindo mensagens diferentes dependendo do resultado das comparações e operações lógicas.

## Conclusão

O algoritmo demonstra de forma prática o uso dos principais operadores da linguagem C: aritméticos (+, -, *, /, %), relacionais (>, <) e lógicos (&&). A implementação inclui tratamento básico de erros, como a verificação de divisão por zero, mostrando boas práticas de programação. O programa é interativo, permitindo que o usuário teste diferentes valores e observe os resultados das operações e verificações realizadas.

