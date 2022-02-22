# [Intermediário] Calculo do Percentual de Stockout de uma Empresa
Este programa recebe um dicionário que possui a seguinte estrutura:

`vendas = {
  "VE0001": (9868, "Concluído", ""),
  "VE0002": (9642, "Concluído", ""),
  "VE0003": (6007, "Concluído", "")
}`

Cada chave desse dicionário representa o ID da transação. Assim, a primeira venda foi VE0001, a segunda foi VE0002, a terceira foi VE0003 etc. Já os valores desse dicionário são tuplas, as quais são compostas pelo valor vendido, status do pedido e motivo do cancelamento.

Para calcular o percentual de stockout, é necessário dividir o total de vendas canceladas por falta de estoque pela soma do total de vendas realizadas com o total de vendas canceladas por falta de estoque.
Esse procedimento é realizado pela função `calcular_stockout`.

Ao fim de sua execução, o programa exibe o percentual de stockout.
