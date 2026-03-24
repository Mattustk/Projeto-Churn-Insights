![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Insights](https://img.shields.io/badge/Insights-007ACC?style=for-the-badge&logo=lightbulb&logoColor=white)

 **TODOS OS INSGIHTS AQUI FORAM COLETADOS DE UM PROJETO CRIADO POR MIM**
![Dashboard](Insight-Projeto-Churn.PNG)


## 📊 Insights Dashboard

**- A partir desse Dashboard fica notório que a grande parcela de cancelamentos acontece devido ao método de pagamento boleto eletrônico. Ao alterar alguns filtros e analisar as estatísticas, eu concluí que os dois métodos que mais agregam renda para a empresa são, em ordem, Credit Card (Cartão de Crédito) e bank transfer (Transferência Bancária).
  De acordo com isso, eu adotaria uma política de bonificação para a transferência do método de pagamento de boleto bancário para os dois citados anteriormente, bonificações essas como descontos de 10%, extensão de contratos de streaming ou de linhas, ou parcerias com outras plataformas.**
  **Observa-se que, além do boleto bancário, há outro problema: o contrato de mês a mês. A taxa de cancelamento em contratos curtos é extremamente maior do que nas opções contratuais de dois anos e um ano. É necessário tomar algumas medidas para resolver isso, como por exemplo descontos nas assinaturas de maiores intervalos de tempo ou melhores produtos para esses contratos.**
  
🛠 **Parte Técnica: Para visualizar o processo de limpeza de dados com Pandas, tratamento de nulos e os scripts de nuvem AWS que geraram a base para esta análise,**
  https://github.com/Mattustk/Projeto-churn

  

## 🥇 Insights Gold
        *Insights feitos pela Freature "Gold"
        

# DF Fidelidade em Markdown
| | Contract | Churn | Total_Clientes | Media_Mensalidade | Faturamento_Total | Media_Meses_Fidelidade |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| 0 | **Month-to-month** | No | 2220 | 61.46 | 3.378.679,25 | 21.03 |
| 1 | **Month-to-month** | **Yes** | **1655** | **73.02** | **1.927.182,25** | **14.02** |
| 2 | **One year** | No | 1306 | 62.54 | 3.792.062,30 | 41.71 |
| 3 | **One year** | Yes | 166 | 85.05 | 674.991,20 | 44.96 |
| 4 | **Two year** | No | 1637 | 60.11 | 6.022.500,25 | 56.95 |
| 5 | **Two year** | Yes | 48 | 86.78 | 260.753,45 | 61.27 |



Como citado anteriormente, um dos maiores motivos dessa taxa de cancelamento é o que está sendo mostrado na linha 2, nos contratos Month-to-month. Observa-se que há 1655 clientes que cancelaram SOMENTE nesses contratos; isso remete a 88% do total de clientes que cancelaram. É uma necessidade de extrema urgência transferir esse modelo contratual, tornando os outros mais abrangentes para o público.



# DF Internet em Markdowm

| | InternetService | Churn | Total_Clientes | Media_Mensalidade |
| :--- | :--- | :--- | :---: | :---: |
| 0 | DSL | No | 1957 | 60.20 |
| 1 | DSL | Yes | 459 | 49.08 |
| 2 | **Fiber optic** | No | 1799 | 93.93 |
| 3 | **Fiber optic** | **Yes** | **1297** | **88.13** |
| 4 | No | No | 1407 | 21.13 |
| 5 | No | Yes | 113 | 20.37  |

Aqui está mais um problema oculto e o principal deles: quem apenas olha o dashboard não consegue perceber que a fibra óptica, por mais lucrativa que seja, também é uma faca de dois gumes. Basta analisar as suas perdas: por mais que a fibra seja o serviço mais rentável da empresa, ela sozinha conseguiu causar um prejuízo de mais de 142 milhões de reais ao total, mais de 85% de toda a receita perdida pelo cancelamento da companhia. Isso acontece devido à falta de suporte e atendimento técnico aos consumidores que utilizam a fibra óptica


| | PaymentMethod | Churn | Total_Clientes | Media_Mensalidade | Faturamento_Total |
| :--- | :--- | :--- | :---: | :---: | :---: |
| 0 | Bank transfer (automatic) | No | 1286 | 65.05 | 4.749.117,10 |
| 1 | Bank transfer (automatic) | Yes | 258 | 77.73 | 643.141,60 |
| 2 | Credit card (automatic) | No | 1290 | 64.56 | 4.664.814,90 |
| 3 | Credit card (automatic) | Yes | 232 | 77.36 | 533.155,95 |
| 4 | **Electronic check** | No | 1294 | 74.23 | 3.551.488,55 |
| 5 | **Electronic check** | **Yes** | **1071** | **78.70** | **2.333.134,80** |
| 6 | Mailed check | No | 1304 | 41.40 | 1.411.332,60 |
| 7 | Mailed check | Yes | 308 | 54.56 | 165.748,35 |

 Outro problema citado anteriormente o boleto bancario, olhando a tabela de pagamentos, o Electronic check (Boleto) é o que mais gera dinheiro, mas também é disparado o que mais perde. É bizarro: enquanto no Cartão de Crédito a gente perdeu uns 232 clientes, no boleto a gente teve um prejuízo de mais de 1071 cancelamentos. Isso causou um rombo de mais de R$ 2,3 milhões de reais que sumiram do faturamento.

Conclusçoes Finais: A análise revela um padrão crítico: o cliente contrata o serviço de Fibra Óptica via Boleto Bancário sob um modelo de assinatura Month-to-month (mensal). Quando esse serviço apresenta qualquer defeito técnico, a empresa falha em oferecer o suporte necessário.

Como o contrato é curto (sem fidelidade) e o pagamento exige uma ação manual do cliente (emissão do boleto), ele possui total liberdade, e incentivo, para cancelar o plano imediatamente ao enfrentar o primeiro problema.





