# SQL- Eleições de 2018 em Minas Gerais.
Explorando informações sobre as Eleições de 2018 em Minas Gerais através do BigQuery no Google Cloud Platform usando linguagem SQL.

Objetivo: Demonstrar algumas análises possíveis de fazer com as bases de dados de Eleições, que foram extraídas do TSE e organizado no Google Cloud Platform pelo site basedosdados.org . 

As bases de dados podem ser acessadas pelo link : https://basedosdados.org/dataset/br-tse-eleicoes?bdm_table=bens_candidato

No Big Query através do código:

Dados de Candidatos: SELECT * FROM `basedosdados.br_tse_eleicoes.candidatos` LIMIT 100 ,

Dados de Vagas: `basedosdados.br_tse_eleicoes.vagas` 

Dados de Bens_Candidatos: `basedosdados.br_tse_eleicoes.bens_candidato` 

Dados de Despesas_Candidatos: `basedosdados.br_tse_eleicoes.despesas_candidato` 

Dados de Receitas_Candidatos: `basedosdados.br_tse_eleicoes.receitas_candidato` 

Dados de Resultados_Candidatos: `basedosdados.br_tse_eleicoes.resultados_candidato` 




#Tabela 1 - Número de Vagas - MG 2018.

![tabela1_vagas_cargo](https://user-images.githubusercontent.com/89020533/172913214-dfc85de8-cf20-4a73-aa90-f5952661b9e6.png)

#Tabela 2_Gráfico- Distribuição de Frequência dos candidatos por data de nascimento - MG 2018.

![tabela2_dist freq_data_nascimento](https://user-images.githubusercontent.com/89020533/172913755-8e27b9c1-ae24-4759-8020-f586955721c3.png)

Percebe-se uma concentração maior de candidatos com data de nascimento entre 1960 e 1985. 

#Tabela 3_Gráfico - Proporção do número de candidatos por Gênero - MG 2018.

![tabela3_n_candidatos_genero](https://user-images.githubusercontent.com/89020533/172914316-928b33cb-622b-4abc-b53e-7599c34d479a.png)

O gênero masculino é predominante e representa 68,2% dos candidatos. O gênero feminino corresponde a 31,8%. 
A Lei das Eleições (9.504/1997) estabelece que "cada partido ou coligação preencherá o mínimo de 30% e o máximo de 70% para candidaturas de cada sexo". Portanto, o número de candidaturas do sexo feminino em Minas Gerais ficou um pouco acima do mínimo exigido.

#Tabela 4.1 - Número de Votos para Governador - MG 2018.

![tabela4 1_votos_governador](https://user-images.githubusercontent.com/89020533/172915753-8adf9312-b480-4fd6-bbd2-79155ec0c666.png)

Romeu Zema foi para o 2º turno com Antonio Anastasia para o Governo de Minas, sendo eleito posteriormente.

#Tabela 4.2 - Número de Votos para Senador - MG 2018.

![tabela4 2_votos_Senador](https://user-images.githubusercontent.com/89020533/172915870-f8ccee4f-10c8-4c3c-aff9-4563a1f01d56.png)

Rodrigo Pacheco e Carlos Viana foram eleitos Senadores por Minas Gerais. A disputa foi acirrado entre 4 candidatos, com Diniz Pinheiro e Dilma Roussef ficando de fora das 2 vagas. 

#Tabela 4.3 - Número de Votos para Deputado Federal (TOP 20) - MG 2018.

![tabela4 3_votos_Dep Federal](https://user-images.githubusercontent.com/89020533/172915940-bb8d5915-7d3b-4de8-a861-17684c7cf075.png)

Marcelo Henrique Teixeira Dias(mais conhecido como Marcelo Álvaro Antônio) foi ministro do Turismo do Brasil de 2019 a 2020, no governo de Jair Bolsonaro. Exerce o cargo de Deputado Federal desde 2020, sendo que no ano de 2018 foi o candidato mais votado em Minas Gerais. 
Em segundo lugar geral, Reginaldo Lopes foi o mais votado do PT, que aparece 5 vezes nessa lista dos 20 candidatos mais votados.

#Tabela 4.4 - Número de Votos para Deputado Estadual (TOP 20) - MG 2018.

![tabela4 4_votos_Dep Estadual](https://user-images.githubusercontent.com/89020533/172915985-764e6616-e3b8-4529-8a9b-c66a59a3317a.png)

O candidato Mauro Henrique Tramonte foi eleito com 516.390 votos, sendo o candidato mais votado em Minas Gerais e segundo Deputado estadual mais votado no Brasil, perdendo apenas para a Deputada estadual paulistana, Janaína Paschoal (PSL).

#Tabela 5.1 - Número de Votos por grau instrução - MG 2018.

![Tebela5 1_votos_Instrucao](https://user-images.githubusercontent.com/89020533/172916566-753f4285-0bdd-42c8-8028-b6ecc0aacd7b.png)

#Tabela 5.2_Gráfico - Gráfico de rosca para proporção do Número de Votos por grau instrução - MG 2018.

![Tebela5 2_gráfico_rosca_votos_Instrucao](https://user-images.githubusercontent.com/89020533/172916915-ee111e43-6b7e-4568-87aa-df8206cd4a0a.png)

Observa-se uma forte predominância do grau de instrução 'Ensino Superior Completo' com 90,9% das candidaturas. Do restante, a grande maioria tem grau de instrução 'Ensino Médio Completo' com 3,8% ou 'Ensino Superior Incompleto' com 3,6%. 

#Tabela 6.0 - Número de Candidatos por raça - MG 2018.

![Tebela6 0_candidatos_raca](https://user-images.githubusercontent.com/89020533/172931147-b5779dbe-23ef-4c3d-b666-59fb2e452285.png)

O nº de candidaturas de pessoas com a raça 'branca' foi 1.142, pouco acima de 968 que é a soma entre a raça 'parda' e 'preta'.

#Tabela 6.1 - Número de Votos por raça - MG 2018.

![Tebela6 1_votos_raca](https://user-images.githubusercontent.com/89020533/172918324-6663691f-380c-48ec-8e9e-c816de262c60.png)

O nº de votos foi aproximadamente 5 vezes maior para a raça 'branca' em relação a 'parda' e 'preta' somadas. O que indica tendência maior em votos para a raça 'branca', já que essa diferença foi mínima no número de candidaturas. 

#Tabela 6.2 - Resultado por raça 'branca' - MG 2018.

![Tebela6 2_resultado_raca_branca](https://user-images.githubusercontent.com/89020533/172918812-a4a45c58-b6d2-4f93-9d68-a13d357063f5.png)

#Tabela 6.3 - Resultado por raça 'preta' - MG 2018.

![Tebela6 3_resultado_raca_preta](https://user-images.githubusercontent.com/89020533/172918919-ba775c4a-4159-4f50-a40b-1b8273bb8a5b.png)

#Tabela 6.4 - Resultado por raça 'parda' - MG 2018.

![Tebela6 4_resultado_raca_parda](https://user-images.githubusercontent.com/89020533/172934221-b5125209-451a-4b94-a1c6-ec9dd1e81809.png)

#Tabela 7.1 - Número de Votos por genero - MG 2018.

![Tebela7 1_votos_genero](https://user-images.githubusercontent.com/89020533/172918983-8535258a-6078-463a-8b4e-0ad5373e32b9.png)

As Mulheres receberam apenas 9,9% dos votos, sendo que teve 31,8% das candidaturas. Esses resultados indicam preferência de votos em Homens.

#Tabela 7.2 - Resultado por gênero 'masculino' - MG 2018.

![Tebela7 2_resultado_genero_masculino](https://user-images.githubusercontent.com/89020533/172919030-273f88ea-b778-40ad-b2a3-e1f0c6e80ce5.png)

#Tabela 7.3 - Resultado por gênero 'feminino' - MG 2018.

![Tebela7 3_resultado_genero_feminino](https://user-images.githubusercontent.com/89020533/172919065-99a932d8-3cbf-4377-8b0e-26100b3abae3.png)

# Tabela 8 - Receitas, número de votos e resultado - Candidatos a Governador - MG 2018. 

![Tabela8_receitas_votos_resultado_gov](https://user-images.githubusercontent.com/89020533/172947502-84354917-81a4-4ead-b88e-240ad1f664a8.png)

Antonio Anastasia teve 2 vezes mais receitas que Romeu Zema, porém ficou atrás no número de votos. 
O terceiro colocado Fernando Pimentel também teve mais receitas que Romeu Zema, porém conseguiu apenas metade do nº de votos(aproximadamente) que obteve o candidato do Partido Novo.
