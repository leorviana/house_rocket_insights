# House Rocket - Parte I

A House Rocket é uma plataforma digital que tem como modelo de negócio, a compra e a venda de imóveis usando tecnologia.

Sua principal estratégia é comprar boas casas em ótimas localizações com preços baixos e depois revendê-las posteriormente à preços mais altos. Quanto maior a diferença entre a compra e a venda, maior o lucro da empresa e portanto maior sua receita.

# Problema de Negócio

O CEO da House Rocket gostaria de maximizar a receita da empresa encontrando boas oportunidades de negócio mas apesar da estratégia mencionada acima, as casas possuem muitos atributos que as tornam mais ou menos atrativas aos compradores e vendedores e a localização e o período do ano também podem influenciar os preços.

Nós fomos contratados para analisar os dados disponíveis e ajudar o CEO da House Rocket a maximar o lucro respondendo as seguintes perguntas:

- Quais casas o CEO da House Rocket deveria comprar e por qual preço de compra?
- Uma vez a casa em posse da empresa, qual o melhor momento para vendê-las e qual seria o preço da venda?
- A House Rocket deveria fazer uma reforma para aumentar o preço da venda? Quais seriam as sugestões de mudanças? Qual o incremento no preço dado por cada opção de reforma?


# Planejamento do Projeto

Utilizei o canvas abaixo canvas para melhor organizar o projeto.

<p align="center">
  <img src="Imagens/.jpg">
</p>

## Ferramentas

 - Python 3.8
 - Jupyter Notebook
 - Método CRISP-DM para gerenciamento de projeto de dados.

## Regras de Negócio

### Quais casas o CEO da House Rocket deveria comprar e por qual preço de compra?

1. Imóveis que estão abaixo do preço médio de sua região e em boas condições.

### Uma vez a casa em posse da empresa, qual o melhor momento para vendê-las e qual seria o preço da venda?

1. Qual trimestre do ano é o melhor para se vender um imóvel a partir do bairro que se encontra.
2. Se o valor de compra do imóvel for **maior** que a média do trimestre pela região, o valor de venda deve ser 15% maior que o valor de compra.
3. Se o valor de compra do imóvel for **menor** que a média do trimestre pela região, o valor de venda deve ser o valor de compra + a diferença para a média + 15%.

### A House Rocket deveria fazer uma reforma para aumentar o preço da venda? Quais seriam as sugestões de mudanças? Qual o incremento no preço dado por cada opção de reforma?

1. Uma reforma deve ser realizada caso a condição da casa seja inferior a 3.
2. As mudanças sugeridas de acordo com alguns artigos são:
- Concertos simples, por exemplo troca de partes velhas e desgastadas como fiação. (Depende da condição da casa, caso a casa seja bem nova, não acrescentaria muito)
- Reformas na estrutura basica, melhorando o design interior. ()
- Transformar espaços vazios em espaços utilizaveis como escritórios, sala de jogos, entre outros. (O incremento no preço depende do quê será construído no lugar)
- Reforma da cozinha. (Você pode recuperar de 53% a 72% na reforma da cozinha)
- Adição de banheiros. () 
- Paisagismo. (ROI esperado de 150% a 1000%)
- Reforma do espaço externo, o deixando mais acessível e útil. (ROI mínimo esperado de 64%)

## Insights Chave

Por meio da análise exploratória de dados, adquirimos alguns insights de negócios, que são os seguintes:

## Resultados Financeiros



## Conclusão



## Próximos passos

Construir um modelo de precifiação com aprendizado de máquina que irá retornar o valor esperado para um imóvel a partir de suas características.

## Referências

House Sales in King County, USA. Kaggle. Disponível em : <https://www.kaggle.com/harlfoxem/housesalesprediction>.

Blog “Seja um DataScientist - Meigarom”. Disponível em: <https://sejaumdatascientist.com/>.

FOSTER, Brittany. "10 Home Improvement Projects That Add Value to Your Property". **moneycrashers**. Disponível em: <https://www.moneycrashers.com/7-home-improvements-to-increase-its-value/>.

GERHARDT, Nick. "20 Home Renovations That Instantly Increase Your Home Value". **familyhandyman**. Disponível em: <https://www.familyhandyman.com/list/home-renovations-that-instantly-add-value-to-your-home/>.
