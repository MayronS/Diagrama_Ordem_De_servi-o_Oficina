# Diagrama_Ordem_De_serviço_Oficina

##

### Obejetivo:

Criação de um modelo relacional de uma Ordem de serviço de uma oficina.

##

### Narrativa fornecida:

- Sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica
- Clientes levam veículos à oficina mecânica para serem consertados ou para passarem por revisões  periódicas
- Cada veículo é designado a uma equipe de mecânicos que identifica os serviços a serem executados e preenche uma OS com data de entrega.
- A partir da OS, calcula-se o valor de cada serviço, consultando-se uma tabela de referência de mão-de-obra
- O valor de cada peça também irá compor a OSO cliente autoriza a execução dos serviços
- A mesma equipe avalia e executa os serviços
- Os mecânicos possuem código, nome, endereço e especialidade
- Cada OS possui: n°, data de emissão, um valor, status e uma data para conclusão dos trabalhos.

##

Com base na narrativa fornecida foi criado 6 tabelas:

- Cliente
- Veículo
- Equipe de mecânicos
- Serviço
- Peça do carro
- Tabela de referência de mão de obra
- Ordem de serviço

  ##

  ### Descrição:
  
Inciando o diagrama com o Cliente no qual pode ter e levar varios veículos na oficina.

Cada equipe de mecânicos pode analisar apenas um veículo por vez. A equipe analisa e pode criar varios serviços para o carro.

Uma ordem de serviço pode ter varios serviços e os serviços podem ser distribuidos para mais de uma ordem de serviço.

Para calcular o valor da mão de obra, é verificado em uma tabela de referência.

Também é verificado os valores das peças necessárias para o conserto ou manutenção do veículo.

Por último o cliente analisa a ordem de serviço e autoriza.

##

Projeto proposto como exercicio no bootcamp Heineken - Inteligência Artificial Aplicada a Dados com Copilot fornecido pela DIO.
