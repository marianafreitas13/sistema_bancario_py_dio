# Sistema Simples de Conta Bancária

Um sistema simples em Python para simular operações básicas de uma conta bancária.

## Funcionalidades

- Depositar dinheiro na conta.
- Sacar dinheiro da conta, com validações de saldo, limite e número máximo de saques.
- Exibir extrato das operações realizadas.
- Encerrar o programa.

## Definição de Funções:

- exibir_menu(): Esta função exibe um menu para o usuário escolher entre as operações disponíveis: depósito, saque, extrato ou sair do sistema.

- realizar_deposito(saldo, extrato): Esta função solicita ao usuário que informe o valor a ser depositado. Se o valor for válido (maior que zero), ele é adicionado ao saldo da conta e registrado no extrato.

- realizar_saque(saldo, extrato, numero_saques, limite, LIMITE_SAQUES): Esta função permite ao usuário fazer um saque da conta. Ela verifica se o saldo é suficiente, se o valor do saque excede o limite estabelecido ou se o número máximo de saques foi atingido. Se todas as condições forem atendidas, o valor do saque é subtraído do saldo e registrado no extrato.

- exibir_extrato(saldo, extrato): Esta função mostra ao usuário o extrato das operações realizadas, incluindo depósitos e saques, além de exibir o saldo atual da conta.

- main(): Esta função controla o fluxo principal do programa. Ela inicializa variáveis como saldo, limite de saque, extrato e número de saques. Dentro de um loop infinito (while True), ela exibe o menu, permite ao usuário escolher uma operação e chama as funções correspondentes para realizar a operação desejada até que o usuário escolha sair (q).

  ### Variáveis Iniciais:

- saldo: Inicializado como 0, representa o saldo atual da conta.
- limite: Define o limite máximo que pode ser sacado de uma vez.
- extrato: Inicialmente vazio, é usado para armazenar as operações realizadas (depósitos e saques).
- numero_saques: Inicia como 0 e conta o número de saques realizados.
- LIMITE_SAQUES: Define o número máximo de saques permitidos antes de exceder o limite.
### Funcionamento:

- O programa entra em um loop onde o menu é exibido repetidamente até que o usuário escolha sair (q).
- Para cada opção escolhida pelo usuário (d para depósito, s para saque, e para extrato, q para sair), o programa executa a operação correspondente chamando as funções apropriadas.
- Cada operação realiza as devidas validações e atualizações no saldo e no extrato, informando ao usuário sobre o resultado da operação (sucesso ou falha).
- Quando o usuário escolhe sair (q), o programa encerra o loop e imprime uma mensagem de saída.
