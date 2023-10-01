# Análise de Crédito
## Introdução
Neste projeto, fui encarregado de analisar um conjunto de dados relacionados à concessão de empréstimos por um banco. O objetivo é identificar se o estado civil dos clientes e o número de filhos têm algum impacto na inadimplência de empréstimos. Além disso, será investigada a relação entre a renda dos clientes, a finalidade do empréstimo e a pontualidade no pagamento dos empréstimos. O resultado desta análise será considerado na criação de uma pontuação de crédito para potenciais clientes.

## Passo 1: Análise Inicial dos Dados
Para iniciar o projeto, abri o arquivo de dados "credit_scoring_eng.csv" e examinei suas informações gerais. Este passo é fundamental para entender a estrutura dos dados com os quais estamos lidando e definir como proceder.

## Passo 2: Pré-processamento dos Dados
Nesta etapa, realizei o pré-processamento dos dados para garantir que estivessem adequados para análise. As principais tarefas realizadas foram:

### -Valores Ausentes
Identifiquei valores ausentes no conjunto de dados. Isso é importante para garantir que nossa análise seja baseada em dados completos e confiáveis. Os principais campos com valores ausentes foram:

* days_employed: Quantidade de dias empregados.
* total_income: Renda total do cliente.

Possíveis razões para valores ausentes podem incluir erros no registro ou omissão de informações pelos clientes. Para preencher esses valores ausentes, utilizei a mediana dos respectivos campos, pois ela é menos sensível a valores extremos e preserva a distribuição dos dados.

### -Dados Duplicados
Identifiquei e removi dados duplicados do conjunto de dados. Dados duplicados podem distorcer nossas análises, pois representam informações repetidas. As razões para a presença de dados duplicados podem incluir erros na inserção de dados ou processos de registro duplicados.

### -Conversão de Tipos de Dados
Convertemos os campos de número real para número inteiro para simplificar a análise. Os campos convertidos incluem days_employed e total_income. Essa conversão é apropriada, uma vez que não requer precisão decimal.

### -Categorização dos Dados
Categorizei os dados em grupos relevantes, como estado civil e finalidade do empréstimo. Isso facilitará a análise e a interpretação dos resultados.

Os dicionários selecionados para os campos de estado civil e finalidade do empréstimo foram escolhidos com base na clareza e na capacidade de agrupar categorias semelhantes.

## Passo 3: Análise das Relações
A análise das relações entre as variáveis foi realizada respondendo às seguintes perguntas:

### -Relação entre Ter Filhos e Inadimplência
* Analisando os dados, foi observado que há uma relação entre o número de filhos e a probabilidade de inadimplência. Clientes com filhos têm uma tendência ligeiramente maior de inadimplência em comparação com aqueles sem filhos.
### -Relação entre Estado Civil e Inadimplência
* Houve uma relação entre o estado civil e a inadimplência. Clientes solteiros tendem a ser mais propensos à inadimplência, enquanto clientes casados ou em união estável apresentam uma taxa de inadimplência mais baixa.
### -Relação entre Renda e Pagamento Pontual
* Verificou-se que a renda dos clientes tem impacto na probabilidade de pagamento pontual. Clientes com renda mais alta têm uma probabilidade maior de pagar seus empréstimos no prazo.
### -Impacto da Finalidade do Empréstimo no Pagamento Pontual
* A finalidade do empréstimo também influencia o pagamento pontual. Empréstimos para educação e compra de carro apresentam taxas mais altas de pagamento pontual, enquanto empréstimos para casamento e compra de imóveis têm taxas mais baixas de pagamento pontual.
## Passo 4: Conclusão Geral
Neste projeto, analisamos um conjunto de dados relacionados à concessão de empréstimos e identificamos diversas relações entre as variáveis, como estado civil, número de filhos, renda e finalidade do empréstimo, e a inadimplência. Essas informações são valiosas para a criação de um modelo de pontuação de crédito que auxilie o banco na avaliação da capacidade de pagamento de seus clientes em potencial. Além disso, o pré-processamento dos dados garantiu a qualidade das análises realizadas. É importante notar que as relações identificadas são observacionais e não implicam causalidade direta, mas podem ser úteis para fins de tomada de decisão no banco.
