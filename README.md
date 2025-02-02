# semaforo

## Semáforo Periódico (Cíclico)

## O que é?

Um semáforo periódico, também conhecido como semáforo cíclico, opera em um ciclo repetitivo e infinito, alternando entre diferentes estados (cores) em intervalos de tempo predefinidos. Esse tipo de semáforo segue sempre a mesma sequência de cores, criando um padrão constante.

## Funcionamento

A lógica básica de um semáforo periódico é a seguinte:

1. vermelho: O semáforo acende a luz vermelha, indicando parada obrigatória. Permanece nesse estado por um período determinado (ex: 3 segundos).
2. amarelo: A luz amarela se acende, alertando para a iminente mudança para o verde. Sua duração também é predefinida (ex: 3 segundos).
3. verde: O semáforo exibe a luz verde, indicando permissão para prosseguir. Fica nesse estado por um tempo específico (ex: 3 segundos).
4. repetição: O ciclo se repete indefinidamente, voltando ao vermelho e continuando a sequência.

## Como o código funciona?

1. loop:O código utiliza um loop `while(true)` para garantir que o semáforo funcione continuamente, sem interrupções.
2. temporizador: Um temporizador é implementado para controlar os intervalos de tempo em que cada cor permanece acesa. Esse temporizador define o momento exato para a troca de cores.
3. função time_reached():Essa função verifica se o tempo definido para a troca de cor já foi atingido. Quando o tempo se esgota, a função retorna verdadeiro, indicando que é hora de mudar o estado do semáforo.
4. variavel estado: Essa variável armazena a informação sobre qual cor do semáforo está acesa no momento. Ela é atualizada a cada troca de cor, garantindo a sequência correta (vermelho -> amarelo -> verde).

