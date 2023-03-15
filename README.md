 
# <p align="center"> <b> CLUSTERIZAÇÃO DE PAÍSES POR INDICADORES DE CRESCIMENTO VERDE, DADOS DE 2019 DA OCDE </b> 

##  💻 Sobre o projeto</br> </br> 

Acesse o notebook completo <a href="https://github.com/diassmatheus/ClusterizacaoDadosOCDE/blob/master/CLUSTERIZACAO_DE_PAISES_POR_INDICADORES_DE_CRESCIMENTO_VERDE.ipynb"> aqui </a>

Acesse o artigo publicado na Revista Principia do Instituto Federal de Educação, Ciência e Tecnologia da Paraíba (IFPB) <a href="https://periodicos.ifpb.edu.br/index.php/principia/article/view/7168"> aqui </a>

O projeto foi proposto durante a realização da disciplina optativa de Mineração de Dados do curso de Engenharia de Produção da <a href="http://www.utfpr.edu.br/"> Universidade Tecnológica Federal do Paraná </a>, entre junho e agosto de 2021. Foram analisados indicadores de crescimento verde da OCDE - Organização para a Cooperação e Desenvolvimento Econômico.

Por meio de tarefas de clusterização de dados, este projeto teve como objetivo analisar os padrões entre países dos mesmos agrupamentos.
Para tanto, foram utilizados dados do <a href="https://www.oecd-ilibrary.org/environment/data/oecd-environment-statistics/green-growth-indicators_data-00665-en"> Green growth indicators </a> e os algoritmos de clusterização k-means e agrupamento hierárquico aglomerativo e a análise dos coeficientes de silhueta para escolha do número ideal de clusters.
  
A lógica para análise foi baseada:

<b> 1 - SELEÇÃO </b>  </br></br>
<b> 1.a - Importação das bibliotecas e do dataset. Pivoteamento do dataframe </b>  </br></br>

<b> 2 - PRÉ-PROCESSAMENTO  </b> </br></br>
<b> 2.a - Verificação dos dados faltantes e critérios de exclusão de instâncias e atributos  </b> </br></br>
<b> 2.b - Análise de correlação entre atributos pelo método de Pearson. Exclusão de correlações superiores a 0,7 ou inferiores a -0,7  </b> </br></br>
<b> 2.c - Estimação do valor do atributo CO2_AIRTRAGDP para os EUA com regressão linear  </b> </br></br>
<b> 2.d - Exclução das demais instâncias com dados faltantes  </b> </br></br>

<b> 3 - TRANSFORMAÇÃO  </b> </br></br>
<b> 3.a - Padronização dos dados  </b> </br></br>

<b> 4 - MINERAÇÃO DOS DADOS  </b> </br></br>
<b> 4.a - Método k-means  </b> </br></br>
<b> 4.b - Método agrupamento hierárquico aglomerativo  </b> </br></br>
<b> 4.c - Comparação entre os métodos e número de clusters para os dados padronizados através dos coeficientes de silhueta  </b> </br></br>
<b> 4.d - Construção do dendrograma do agrupamento hierárquico  </b> </br></br>
<b> 4.e - Plotagem dos clusters de paises no mapa mundi para ambos os métodos  </b> </br></br>

<b> 5 - INTERPRETAÇÃO/AVALIAÇÃO DOS RESULTADOS  </b> (apenas para k-means) </br></br>
<b> 5.a - Análise de balanceamento dos clusters  </b> </br></br>
<b> 5.b - Discussão dos resultados cluster a cluster  </b> </br></br>

---

## 🛠 Tecnologias

As análises foram desenvolvidos na linguagem Python, utilizando o Jupyter Notebook,  JSON, Pandas, Matplotlib, Seaborn, NumPy, Scikit-learn, SciPy e Plotly.
