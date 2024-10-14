# Tratamento de dados em Python e criação de Dashboard utilizando PoweBI

Estado original do Dataset:

## Renomeação das colunas do dataset

O dataset original continha nomeadas em inglês, para facilitar a visualização, segue a tradução e descrição de todas as colunas:

| Nome Original             | Nome Atual                | Descrição                                       |
|---------------------------|---------------------------|-------------------------------------------------|
| `InvoiceId`               | `IdFatura`                | Identificador único da fatura da venda           |
| `Branch`                  | `Filial`                  | Código da filial onde a venda foi realizada      |
| `City`                    | `Cidade`                  | Nome da cidade onde a venda ocorreu             |
| `CustomerType`            | `TipoCliente`             | Tipo de cliente (Membro ou Normal)              |
| `Gender`                  | `Gênero`                  | Gênero do cliente                               |
| `ProductLine`             | `LinhaProduto`            | Categoria de produto                            |
| `UnitPrice`               | `PrecoUnitario`           | Preço unitário do produto                       |
| `Quantity`                | `Quantidade`              | Quantidade de produtos comprados                |
| `Tax5Percent`             | `Imposto5Porcento`        | Valor do imposto de 5% sobre a venda            |
| `TotalAmount`             | `ValorTotal`              | Valor total da compra                           |
| `TransactionDate`         | `DataTransacao`           | Data em que a transação foi realizada           |
| `TransactionTime`         | `HoraTransacao`           | Hora da transação                               |
| `PaymentMethod`           | `MetodoPagamento`         | Método de pagamento usado (Ewallet, Cash, etc.) |
| `COGS`                    | `CustoMercadoriasVendidas`| Custo das mercadorias vendidas (CMV)            |
| `GrossMarginPercentage`   | `PercentualMargemBruta`   | Percentual da margem bruta                      |
| `GrossIncome`             | `RendaBruta`              | Lucro bruto da venda                            |
| `Rating`                  | `Avaliacao`               | Avaliação do cliente em relação à experiência   |

Codigo utilizado:

```python

#utilizamos uma função para renomar as colunas com base na ordem do dataset original, portanto, a ordem não foi alterada

dataset.columns = [
    'IdVenda', 'Filial', 'Cidade', 'TipoCliente', 'Gênero',
    'LinhaProduto', 'PrecoUnitario', 'Quantidade', 'Imposto5Porcento', 'ValorTotal',
    'DataTransacao', 'HoraTransacao', 'MetodoPagamento', 'CustoMercadoriasVendidas',
    'PercentualMargemBruta', 'RendaBruta', 'Avaliacao'
]

```

## Explorando conjunto de dados

Funções utilizadas:

```python
dataset.head() # demonstra os dados nas posições iniciais (1)
dataset.tail() # demonstra os dados nas posições finais (2)
dataset.sample() # seleciona posições aleatórias e demonstra os dados (3)
```

Resultado (1):

Resultado (2):

Resultado(3):



  
