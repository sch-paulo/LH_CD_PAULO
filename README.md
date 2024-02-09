# Projeto de Ciência de Dados - Análise e Modelagem de Preços de Aluguel de Imóveis em Nova York
## Introdução
Neste projeto, vamos construir um modelo preditivo de preços de aluguéis temporários na cidade de Nova York. O foco principal é compreender melhor o cenário para conseguir desenvolver uma plataforma inovadora e que seja competitiva no mercado. Para isso, será utilizada uma base de dados de uma plataforma concorrente, no qual o nosso objetivo é entender os dados através de uma análise exploratória e posteriormente utilizar desse conhecimento para desenvolver um modelo de predição de preços.

O dataset disponibilizado possui 16 colunas, sendo 11 numéricas e 5 categóricas, e 48.894 linhas. As colunas são as seguintes:

* **id** – Atua como uma chave exclusiva para cada anúncio nos dados do aplicativo
* **nome** - Representa o nome do anúncio
* **host_id** - Representa o id do usuário que hospedou o anúncio
* **host_name** – Contém o nome do usuário que hospedou o anúncio
* **bairro_group** - Contém o nome do bairro onde o anúncio está localizado
* **bairro** - Contém o nome da área onde o anúncio está localizado
* **latitude** - Contém a latitude do local
* **longitude** - Contém a longitude do local
* **room_type** – Contém o tipo de espaço de cada anúncio
* **price** - Contém o preço por noite em dólares listado pelo anfitrião
* **minimo_noites** - Contém o número mínimo de noites que o usuário deve reservar
* **numero_de_reviews** - Contém o número de comentários dados a cada listagem
* **ultima_review** - Contém a data da última revisão dada à listagem
* **reviews_por_mes** - Contém o número de avaliações fornecidas por mês
* **calculado_host_listings_count** - Contém a quantidade de listagem por host
* **disponibilidade_365** - Contém o número de dias em que o anúncio está disponível para reserva


## Descrição do Projeto
O projeto consiste nas seguintes etapas:

### Importação, análise e tratamentos iniciais
Importação do dataset e bibliotecas necessárias, análise inicial da composição do dataset e tratamentos básicos de incongruências encontradas.

### Análise Exploratória dos Dados
Investigação as características mais relevantes, buscar insights e apresentar hipóteses para solucionar nossos problemas de negócio.

### Resposta às Perguntas-chave

1. Onde seria mais indicada a compra de um apartamento para aluguel na plataforma?
2. O número mínimo de noites e a disponibilidade ao longo do ano interferem no preço?
3. Existe algum padrão no texto do nome do local para lugares de mais alto valor?
   
### Modelagem Preditiva de Preços
Desenvolver um modelo de previsão de preços utilizando as variáveis disponíveis nos dados. Avaliar diferentes modelos e escolher o mais adequado, considerando as métricas de performance.

* *Feature Engineering*: através da análise exploratória, foi possível identificar novas possíveis variáveis que poderiam impactar positivamente no modelo;
* Separação da variável *target price* e divisão do dataset em treino e teste;
* Teste com validação cruzada em diversos modelos de regressão (Regressão linear simples, Decision Tree, XGBoost, LightGBM e CatBoost);
* Tunagem de hiperparâmetros;
* Avaliação do modelo final.


## Conteúdo do projeto

* Notebook (.ipynb) com o relatório das análises exploratórias e modelagem dos dados.
* Arquivo .pkl contendo o modelo desenvolvido.
* README explicando como instalar e executar o projeto.
* Arquivo de requisitos ``requirements.txt`` com os pacotes utilizados e suas versões.
* Respostas às Perguntas-chave

## Instalação e Execução do Projeto
Para executar o projeto, siga as instruções abaixo:

* Clone o repositório do projeto: ``git clone https://github.com/sch-paulo/LH_CD_PAULO.git``;
* Instale os pacotes necessários: ``pip install -r requirements.txt``;
* Execute os notebooks de análise exploratória e modelagem;
* Utilize o arquivo .pkl para carregar o modelo desenvolvido e testá-lo em novos dados.

## Conclusão
Este projeto visa fornecer insights valiosos para uma nova plata investidores interessados no mercado de aluguéis de imóveis em Nova York, fornecendo uma análise detalhada dos dados disponíveis e um modelo preditivo de preços para auxiliar na tomada de decisão.
