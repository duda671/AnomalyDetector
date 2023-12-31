

# AnomalyDetector
Modelo de detecção de anomalias em transações financeiras utilizando Python e algoritmo 'Isolation Forest'.

## Recursos

- Uso do algoritmo 'Isolation Forest' para identificar anomalias em dados. 
- Análise exploratória dos dados para identificar padrões e irregularidades.
- Detecção de anomalias como o modelo detector.
- Visualizações das informações obtidas.

## Demonstração
Nesse exemplo é criado um Scatter plot que verifica a relação de causa e efeito entre o valor médio de transação e idade do titular da conta.

![Visualização](images/valor_med_transVSidade.png)


Ao usar o modelo detector, o usuário insere os valores nos campos específicos, e a previsão é feita com base nos dados colhidos durante o treinamento.

```
Insira o valor para 'Transação_Valor': 10000
Insira o valor para 'Transação_Valor_Médio': 900
Insira o valor para 'Frequência': 6
```

```
<!-- Saída:  -->

Anomalia detectada: Essa transação está sinalizada como fraudulenta (anomalia).
```

## Como Utilizar

- Requisitos de Instalação: Verifique se você tem as bibliotecas necessárias instaladas. Você pode instalar as dependências com o seguinte comando:
```
pip install -r requirements.txt
```

- Dados de Treinamento: Prepare seus dados de transações financeiras rotuladas para treinar o modelo. Os recursos importantes devem incluir 'Transaction_Amount', 'Average_Transaction_Amount' e 'Frequency_of_Transactions'. Desative ou edite as colunas renomeadas em casos de erro.

- Treinamento do Modelo: Use o código fornecido para treinar o modelo de detecção de anomalias com base nos seus dados de treinamento.

- Previsões de Anomalia: Com o modelo treinado, você pode fazer previsões de detecção de anomalias para novas transações, fornecendo os valores relevantes.