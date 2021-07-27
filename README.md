# Desafio de Ciência de Dados

## Contexto do Problema

XPTO é uma plataforma de e-commerce com milhões de produtos e milhares de vendedores e lojas. Um dos grandes desafios enfrentados por este marketplace é identificar produtos idênticos vendidos por lojas diferentes na internet.

Dado que um vendedor (ou loja) cadastrado deseja adicionar uma nova oferta de produto na plataforma, o sistema deve ser capaz de automaticamente determinar se esta oferta já se encontra no catálogo ou não. Note que se esta tarefa não for realizada de forma adequada, o usuário poderá obter resultados duplicados na página de busca após realizar uma pesquisa por produtos, o que causaria uma experiência ruim dentro da plataforma.

A nível de métricas de negócio, a preocupação de serem exibidos resultados com maior acurácia para o usuário, poderão gerar impacto em: 
- Aumento da taxa de conversão em compras.
- Aumento de comissão.

Portanto, o objetivo deste desafio é gerar um modelo preditivo, que seja capaz de identificar se, dada duas ofertas de vendedores diferentes, com seus respectivos atributos (ids, títulos, preços e imagens), correspondem ou não ao mesmo produto. 

## Etapas de desenvolvimento

### Etapa 1

Desenvolver o modelo preditivo em um notebook python utilizando o ambiente Colab do Google (https://colab.research.google.com), o qual é análogo ao Jupyter Notebook. Para o desenvolvimento do modelo, serão disponibilizados os arquivos de treino (rotulado) e de teste (a ser classificado):
- arquivo de treino: train.csv
- arquivo de teste: test.csv

obs: Tais arquivos estão localizados na raiz do repositório.

### Etapa 2

Gerar um arquivo de resultados em formato CSV, chamado “predictions_matching_your_name.csv”, o qual deverá conter como cabeçalho as colunas “offer_id_1”, “offer_id_2” e “matching”. Após a primeira linha de cabeçalho, as subsequentes estarão associadas aos resultados de predição do modelo para o par de ofertas apresentado. Os possíveis valores assumidos pela coluna matching serão “1” ou “0”, para para produtos iguais ou diferentes, respectivamente. Como separador entre os campos deverá se utilizar “vírgula”. Exemplo:

    id_1,id_2,matching
    434907,434908,1
    434909,434910,0

## Entrega

Compartilhar o notebook desenvolvido no Colab bem como o arquivo de resultado gerado, “predictions_matching_your_name.csv”, com o email vagas.engenharia.dados@meliuz.com.br.

obs: Não utilizar frameworks ou libs de AutoML, como por exemplo, auto-sklearn.

## O que será avaliado?
Com base no arquivo submetido “predictions_matching_your_name.csv” contendo as classificações feitas pelo modelo desenvolvido, será medida a acurácia dos resultados obtidos. Além disso, também será analisada a organização, estruturação lógica e eventuais comentários inseridos no notebook, com o objetivo de entender a linha de raciocínio tomada para desenvolver a solução.
