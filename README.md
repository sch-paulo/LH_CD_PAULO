# Desafio Cientista de Dados Indicium
## Introdução
Neste projeto, vamos construir um modelo preditivo de preços de aluguéis temporários na cidade de Nova York. O foco principal é compreender melhor o cenário para conseguir desenvolver uma plataforma inovadora e que seja competitiva no mercado. Para isso, será utilizada uma base de dados de uma plataforma concorrente, no qual o nosso objetivo é entender os dados através de uma análise exploratória e posteriormente utilizar desse conhecimento para desenvolver um modelo de predição de preços.

Vamos conhecer melhor o nosso dataset e cada uma de suas colunas:
**id** – Atua como uma chave exclusiva para cada anúncio nos dados do aplicativo

**nome** - Representa o nome do anúncio

**host_id** - Representa o id do usuário que hospedou o anúncio

**host_name** – Contém o nome do usuário que hospedou o anúncio

**bairro_group** - Contém o nome do bairro onde o anúncio está localizado

**bairro** - Contém o nome da área onde o anúncio está localizado

**latitude** - Contém a latitude do local

**longitude** - Contém a longitude do local

**room_type** – Contém o tipo de espaço de cada anúncio

**price** - Contém o preço por noite em dólares listado pelo anfitrião

**minimo_noites** - Contém o número mínimo de noites que o usuário deve reservar

**numero_de_reviews** - Contém o número de comentários dados a cada listagem

**ultima_review** - Contém a data da última revisão dada à listagem

**reviews_por_mes** - Contém o número de avaliações fornecidas por mês

**calculado_host_listings_count** - Contém a quantidade de listagem por host

**disponibilidade_365** - Contém o número de dias em que o anúncio está disponível para reserva


São 16 colunas, sendo 11 numéricas e 5 categóricas, e 48.894 linhas.

## Estruturação do projeto
**Introdução**: Pequena descrição do problema e objetivos do projeto.

**Importação, análise e tratamentos iniciais**: Importação do dataset e bibliotecas necessárias, análise inicial da composição do dataset e tratamentos básicos de incongruências encontradas.

**Análise Exploratória**: Investigação e busca de insights para solucionar nossos problemas de negócio.

***Feature Engineering***: Baseado na análise, são criadas algumas variáveis (*features*) que podem nos auxiliar na performance de nossos modelos.



Perguntas Exploradas: Responda a perguntas relevantes para o negócio.
Modelagem Preditiva: Aprenda como o modelo de previsão funciona.
Previsão de Preço: Simule o preço para um apartamento específico.
Requisitos e Instalação: Configure seu ambiente para executar o projeto.
Relatórios e Códigos: Explore os resultados em detalhes.
Próximos Passos: Explore ideias para aprimorar o projeto.
Desafio:
Auxiliar na criação de uma plataforma de aluguel em Nova York, realizando:

Análise exploratória dos dados do Airbnb (concorrente).
Desenvolvimento e validação de um modelo preditivo de preços.
Análise Exploratória (EDA):
Visão geral dos dados:
Distribuição dos preços, tipos de acomodação, bairros, etc.
Identificação de outliers e valores inconsistentes.
Análise por bairro:
Preços médios, sazonalidade, tipos de acomodação mais frequentes.
Correlação entre preço e variáveis como número de quartos, reviews, etc.
Análise por tipo de acomodação:
Preços médios, comodidades mais comuns, etc.
Diferenças de preço entre apartamentos, casas, quartos, etc.
Análise do texto do anúncio:
Palavras-chave que impactam o preço.
Sentimento do texto e sua relação com o preço.
Perguntas Exploradas:
Onde investir? Sugestões de bairros com boa rentabilidade e alta demanda.
Noites e disponibilidade: Impacto no preço e otimização da estratégia.
Texto do anúncio: Padrões em anúncios de alto valor e dicas para otimização.
Modelagem Preditiva:
Problema: Regressão - Previsão do preço de um imóvel.

Modelo: Selecionado com base em testes e análise de performance.

Variáveis:

Bairro: Localização do imóvel.
Tipo de acomodação: Apartamento, casa, quarto, etc.
Número de quartos: Quantidade de quartos disponíveis.
Número de banheiros: Quantidade de banheiros disponíveis.
Comodidades: Presença de piscina, Wi-Fi, etc.
Número de reviews: Quantidade de avaliações recebidas.
Média das avaliações: Avaliação média do imóvel.
Disponibilidade: Número de dias disponíveis para aluguel no ano.
Métricas de Performance:

Erro médio quadrático (MSE): Mede a média dos erros quadráticos das previsões.
R²: Indica a porcentagem da variabilidade do preço explicada pelo modelo.
Previsão de Preço:
Para um apartamento com as características do exemplo, o preço sugerido seria de R$ 1.150.

️ Requisitos e Instalação:
Python 3.8 ou superior
Pacote pipenv
Pacotes listados no arquivo requirements.txt
Para instalar, execute:

pipenv install
Relatórios e Códigos:
Relatório EDA: Apresentação dos resultados da análise exploratória em PDF ou Jupyter Notebook.
Código EDA: Jupyter Notebook com código da análise exploratória.
Código de Modelagem: Jupyter Notebook com código da modelagem preditiva.
Modelo Pickle (.pkl): Modelo treinado para previsão de preços.
Próximos Passos:
Incluir mais dados: Airbnb, sites de imobiliárias, etc.
Testar outros modelos: Regressão linear, Random Forest, etc.
Ajustar o modelo: Otimizar hiperparâmetros e avaliar outras variáveis.
Criar interface web: Facilitar a consulta de preços e sugestões de investimento.
