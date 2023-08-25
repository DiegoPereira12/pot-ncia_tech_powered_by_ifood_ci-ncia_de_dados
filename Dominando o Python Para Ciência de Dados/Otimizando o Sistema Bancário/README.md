# Sistema Bancário

## Obejtivo Geral

Separar as funções existentes de saque, depósito e extrato em funcões. Criar duas novas funcões: cadastrar usuário(cliente) e cadastrar conta bancária.


### Desafio

Precisamos deixar nosso código mais modularizado, para isso vamos criar funcões para operações existentes: sacar, depositar e visualizar histórico. Além disso, para a versão 2 do nosso sistema precisamos criar duas novas funções: criar usuário(cliente banco) e criar conta corrente (vincular com usuário).

### Separação em funções

Devemos criar funcões para todas as operações do sistema, cada função vai ter uma regra na passagem de argumento. 

### Saque

A função saque deve receber os argumentos apenas por nome (keyword only). Sugestão de argumentos: saldo, valor, extrato, limite, numero_saques, limite_saques. Sugestão de retorno: saldo e extrato.

### Depósito

A função depósito deve receber os argumentos apenas por posiçao (positional only). Sugestão de arqumentos: saldo, valor, extrato. Sugestão de retorno: saldo e extrato.

### Extrato

A funççao extratti deve recebr os argumentos por posição e nome (positional only e keyword only). Argumentos posicionais: saldo, arqumentos nomeados: extrato

### Novas funcões

Precisamos criar duas novas funções: criar usuário e criar conta corrente. Ex: Listar contas

### Criar usuário (cliente)

O programa deve armazenar os usuários em uma lista, um usuário é composto por: nome, data de nascimento, cpf e endereço. O endereço é uma string com o formato: logradouro, nro - bairro - cidade/sigla estado. Deve ser armazenado somente os números do CPF. Não podemos cadastrar 2 usuários com o memso CPF.

### Criar conta corrente

O programa deve armazenar contas em uma lista, uma conta é composta por: agência, número da conta e usuário. O número da conta é sequencial, iniciando em 1. O número da agência é fixo: "0001". O usuário pode ter mais de uma conta, mas uma conta pertence a somente um usuário.

OBS:. Para vincular um usuário a uma conta, filtre a lista de usuários buscando o nnúmero do CPF informando para cada usuário da lista.