O programa funcionará da seguinte forma:

Entrada 1: O programa pede o valor para depósito.

Entrada 2: O programa pede o valor para saque.

O saldo será mostrado após cada operação, e se o usuário tentar realizar uma operação inválida, uma mensagem de erro será exibida.

   ----------------------------Explicação do Código----------------------------------------------------------------------------------

Inicialização do saldo e Scanner:

Criamos uma variável saldo que começa com o valor 0.

O Scanner é usado para capturar a entrada do usuário (os valores para depósito e saque).

Depósito:

O programa solicita que o usuário insira um valor para o depósito.

Se o valor for negativo, um erro é gerado com throw new IllegalArgumentException(), e o programa avisa que o valor não pode ser negativo.

Se o valor for válido, ele é somado ao saldo.

Saque:

O programa solicita que o usuário insira um valor para o saque.

O programa verifica:

Se o valor do saque é negativo.

Se o saldo é suficiente para o saque.

Se algum dos erros ocorrer, o programa lança uma exceção.

Se tudo estiver correto, o valor do saque é subtraído do saldo.

Tratamento de erros:

Usamos o try-catch para capturar possíveis exceções.

Caso o usuário insira valores inválidos (como um valor negativo ou um saque maior que o saldo), uma mensagem de erro será exibida.

Bloco finally:

O bloco finally é utilizado para garantir que o Scanner seja fechado após o uso, evitando possíveis vazamentos de recursos.
