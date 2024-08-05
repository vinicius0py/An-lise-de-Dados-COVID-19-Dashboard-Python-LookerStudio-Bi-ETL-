**Análise de Dados: COVID-19 Dashboard**<br>
**Autor** [Vinícius Oliveira](https://www.linkedin.com/in/vinicius-oliveira-p1/)

---

**Objetivo do Projeto**
O objetivo deste projeto é **desenvolver um dashboard interativo** para a análise detalhada da evolução dos casos de ***COVID-19*** e da vacinação no **Brasil**.

O projeto inclui o **processamento e a preparação dos dados**, garantindo a **qualidade e a integridade das informações**. Utilizaremos o **Looker Studio** para a visualização desses dados, permitindo a criação de **representações visuais interativas e dinâmicas**.
Combinando o processamento meticuloso dos dados e uma visualização avançada, o projeto visa oferecer uma **ferramenta robusta** para a análise e interpretação eficaz das informações sobre a pandemia no Brasil.


**TLDR**
 - **Dashboard**:
  - Looker Studio ([Link](https://lookerstudio.google.com/reporting/7a414632-a04e-4602-988e-b435e2d6d505)).
 - **Processamento**:
  - Kaggle Notebook [Link](https://www.kaggle.com/code/vinciusoliveirap1/an-lise-de-dados-covid-19-dashboard).
 - **Fontes**:
  - Casos pela universidade John Hopkins ([link](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_daily_reports));
  - Vacinação pela universidade de Oxford ([link](https://covid.ourworldindata.org/data/owid-covid-data.csv)).


**Pandemia Coronavírus 2019**
> A COVID-19 é uma infecção respiratória aguda causada pelo coronavírus SARS-CoV-2, potencialmente grave, de elevada transmissibilidade e de distribuição global. Fonte: Governo brasileiro ([link](https://www.gov.br/saude/pt-br/coronavirus/o-que-e-o-coronavirus)).

A disponibilidade de dados sobre a evolução da pandemia ao longo do tempo em uma determinada região geográfica é fundamental para seu combate. Este projeto tem como objetivo construir um dashboard para a exploração e visualização interativa dos dados sobre o avanço dos casos e da vacinação no Brasil.

O processamento dos dados pode ser acessado [neste link](https://www.kaggle.com/code/vinciusoliveirap1/an-lise-de-dados-covid-19-dashboard) e o dashboard está disponível ([Link](https://lookerstudio.google.com/reporting/7a414632-a04e-4602-988e-b435e2d6d505)).


**Dados**
Os dados sobre **casos de COVID-19** são compilados pelo Centro de Ciência de Sistemas e Engenharia da Universidade Johns Hopkins ([link para a universidade](https://www.jhu.edu)). Estes dados são atualizados diariamente desde janeiro de 2020, com granularidade temporal diária e geográfica detalhada por regiões de países, como estados e condados.

Você pode acessar o website do projeto [aqui](https://systems.jhu.edu/research/public-health/ncov/), e os dados estão disponíveis [neste repositório do GitHub](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_daily_reports).

Abaixo, descrevemos os dados derivados do processamento realizado.


- **date:** Data de referência.
- **state:** Estado.
- **country:** País.
- **population**: População estimada.
- **confirmed:** Número acumulado de infectados.
- **confirmed_1d:** Número diário de infectados.
- **confirmed_moving_avg_7d:** Média móvel de 7 dias do número diário de infectados.
- **confirmed_moving_avg_7d_rate_14d:** Relação entre a média móvel de 7 dias do número diário de infectados e a média móvel de 7 dias de 14 dias atrás.
- **deaths:** Número acumulado de mortos.
- **deaths_1d:** Número diário de mortos.
- **deaths_moving_avg_7d:** Média móvel de 7 dias do número diário de mortos.
- **deaths_moving_avg_7d_rate_14d:** Relação entre a média móvel de 7 dias do número diário de mortos e a média móvel de 7 dias de 14 dias atrás.
- **month:** Mês de referência.
- **year:** Ano de referência.

  
Os dados sobre **vacinação da COVID-19** são compilados pelo projeto Nosso Mundo em Dados (*Our World in Data* ou OWID) da Universidade Britânica de **Oxford** ([link para a universidade](https://www.ox.ac.uk)). Esses dados são **atualizados diariamente** desde janeiro de 2020, com uma **granularidade temporal de dias e geográfica de países**.

Você pode acessar o website do projeto [aqui](https://ourworldindata.org), e os dados estão disponíveis [neste link](https://covid.ourworldindata.org/data/owid-covid-data.csv).

Abaixo, estão descritos os dados derivados do seu processamento.


- **date:**Data de referência.
- **country:** País.
- **population:** População estimada.
- **total:** Número acumulado de doses administradas.
- **one_shot:** Número acumulado de pessoas que receberam uma dose.
- **one_shot_perc:** Percentual acumulado de pessoas que receberam uma dose.
- **two_shots:** Número acumulado de pessoas que receberam duas doses.
- **two_shot_perc:** Percentual acumulado de pessoas que receberam duas doses.
- **three_shots:** Número acumulado de pessoas que receberam três doses.
- **three_shot_perc:** Percentual acumulado de pessoas que receberam três doses.
- **month:** Mês de referência.
 -**year:** Ano de referência.
  
<br>
<br>

**Visualizações pelo Looker Studio**
Link da vizualização interativa pelo Looker Studio [Link](https://lookerstudio.google.com/reporting/7a414632-a04e-4602-988e-b435e2d6d505)

A seguir, apresento como ficou a visualização no **Looker Studio**

**Visualização dos KPIs relacionados a casos e mortes, incluindo a proporção de vacinados, com filtragem por data específica, além da exibição do mapa de distribuição.**<br>
![Screenshot_32](https://github.com/user-attachments/assets/43742d9b-afc1-4aeb-a00c-dc9178b55926)


**Visualização dos gráficos de casos e mortes ao longo de todo o período analisado**<br>
![Screenshot_33](https://github.com/user-attachments/assets/c81123c8-35a0-4238-a58b-2dbd243f939b)


**Por fim, a visualização dos gráficos selecionados, onde foi aplicado um filtro para exibir apenas um período específico de dados diretamente no gráfico.**<br>
![Screenshot_34](https://github.com/user-attachments/assets/9032f025-11e6-4504-bc14-780930507b02)


