# DIO - Trilha Java Básico
[www.dio.me](https://www.dio.me)

## Autores
- [Eliezer Moraes Silva](https://github.com/eliezermoraesss)

# Desafio do Contador

Este é um desafio de programação em Java que envolve a criação de um programa chamado "Contador". O programa solicita dois parâmetros inteiros do usuário, realiza uma validação e, em seguida, conta e imprime uma sequência de números entre esses dois parâmetros. Se os parâmetros inseridos não forem válidos, o programa lança uma exceção personalizada `ParametrosInvalidosException`.

## Funcionamento do Programa

O programa funciona da seguinte maneira:

1. Solicita ao usuário que insira o primeiro parâmetro inteiro, `parametroUm`.

2. Solicita ao usuário que insira o segundo parâmetro inteiro, `parametroDois`.

3. Chama o método `contar(parametroUm, parametroDois)` para realizar a contagem e a impressão dos números.

4. Dentro do método `contar`, o programa faz o seguinte:

   - Valida se `parametroUm` é MAIOR ou igual a `parametroDois`. Se for, lança uma exceção `ParametrosInvalidosException` com a mensagem "O parâmetro UM é maior ou igual ao parâmetro DOIS".

   - Calcula a diferença entre `parametroDois` e `parametroUm` e armazena o resultado na variável `contagem`.

   - Utiliza um loop `for` para imprimir os números na sequência, a partir de `parametroUm`.

5. Se a exceção `ParametrosInvalidosException` for lançada durante a validação, o programa a captura no bloco `catch` no método `main` e imprime a mensagem de erro correspondente.

6. Fecha o scanner usado para receber as entradas do usuário.

## Exceções Personalizadas

O programa define uma exceção personalizada chamada `ParametrosInvalidosException` para lidar com a situação em que `parametroUm` é maior ou igual a `parametroDois`. Isso garante que o programa trate casos inválidos adequadamente.

## Uso do Programa

Para usar o programa:

1. Compile o código Java.

2. Execute o programa.

3. Insira os dois parâmetros inteiros quando solicitado.

4. O programa contará e imprimirá a sequência de números entre esses dois parâmetros, desde que `parametroUm` seja menor que `parametroDois`. Caso contrário, uma exceção será lançada e uma mensagem de erro será exibida.

## Observações

- Certifique-se de que a exceção `ParametrosInvalidosException` seja definida em um arquivo separado e importada corretamente para o programa principal.

- O programa assume que o usuário inserirá números inteiros válidos como entrada. Qualquer entrada inválida não é tratada neste desafio.

- Este desafio demonstra o uso de exceções personalizadas em Java para lidar com casos específicos de erro.
