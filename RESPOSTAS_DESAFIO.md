## Respostas para as Perguntas do Desafio

#### 1. Onde seria mais indicada a compra para alugar no Airbnb?

Com base na análise, as regiões mais indicadas para investimento são Manhattan e Brooklyn, pois apresentam maior demanda e preços elevados, além de baixa taxa de vacância ao longo do ano.

#### 2. O número mínimo de noites e a disponibilidade ao longo do ano interferem no preço?

Sim. Análises estatísticas mostraram uma correlação negativa entre o número mínimo de noites e o preço, indicando que locais com maior flexibilidade de estadia tendem a cobrar diárias mais altas. Além disso, imóveis com maior disponibilidade anual geralmente possuem preços mais baixos devido à maior concorrência.

#### 3. Existe um padrão no nome dos lugares de mais alto valor?

Sim. Análises de texto indicaram que palavras como “Luxury”, “View”, “Apartment” e “Central” são comuns em listagens de alto valor, sugerindo que a descrição do anúncio influencia a percepção de preço.

#### 4. Como foi feita a previsão de preços?

Para prever os valores, foram utilizados diferentes modelos estatísticos e de aprendizado de máquina, sendo que a abordagem mais eficaz se mostrou um Random Forest Regressor. As variáveis mais relevantes para previsão foram:

Localização (latitude, longitude, bairro)

Tipo de acomodação (room_type)

Disponibilidade e mínimo de noites

Histórico de reviews

O modelo escolhido foi devido à sua capacidade de capturar relações não lineares e lidar bem com variáveis categóricas e numéricas.

#### 5. Qual foi a medida de performance escolhida e por quê?

A principal métrica utilizada foi o RMSE (Root Mean Squared Error), pois penaliza predições com grandes desvios, garantindo previsões mais precisas. Também consideramos o MAE (Mean Absolute Error) e R² (coeficiente de determinação) para uma avaliação complementar.

#### 6. Previsão de preço para o apartamento exemplo

Utilizando o modelo treinado, a previsão para o apartamento Skylit Midtown Castle é **$ 212,82** por noite.
