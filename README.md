# House Rocket - Parte I
A House Rocket é uma plataforma digital que tem como modelo de negócio, a compra e a venda de imóveis usando tecnologia.

Sua principal estratégia é comprar boas casas em ótimas localizações com preços baixos e depois revendê-las posteriormente à preços mais altos. Quanto maior a diferença entre a compra e a venda, maior o lucro da empresa e portanto maior sua receita.
<p align="center">
  <img src="https://www.shopise.com/wp-content/uploads/ngg_featured/Tips-to-sell-your-property-fast-and-easy.jpg">
</p>


# Problema de Negócio
O CEO da House Rocket gostaria de maximizar a receita da empresa encontrando boas oportunidades de negócio mas apesar da estratégia mencionada acima, as casas possuem muitos atributos que as tornam mais ou menos atrativas aos compradores e vendedores e a localização e o período do ano também podem influenciar os preços.

Nós fomos contratados para analisar os dados disponíveis e ajudar o CEO da House Rocket a maximar o lucro respondendo as seguintes perguntas:

- Quais casas o CEO da House Rocket deveria comprar e por qual preço de compra?
- Uma vez a casa em posse da empresa, qual o melhor momento para vendê-las e qual seria o preço da venda?
- A House Rocket deveria fazer uma reforma para aumentar o preço da venda? Quais seriam as sugestões de mudanças? Qual o incremento no preço dado por cada opção de reforma?


# Planejamento do Projeto
Utilizei o canvas abaixo canvas para melhor organizar o projeto.

<p align="center">
  <img src="https://github.com/leorviana/imoveis_house_rocket/blob/main/canvas_ds.png">
</p>

# Ferramentas
 - Python 3.8
 - Jupyter Notebook
 - Método CRISP-DM para gerenciamento de projeto de dados.

# Regras de Negócio

### Quais casas o CEO da House Rocket deveria comprar e por qual preço de compra?
1. Imóveis que estão abaixo do preço médio de sua região e em boas condições.


### Uma vez a casa em posse da empresa, qual o melhor momento para vendê-las e qual seria o preço da venda?
1. Qual trimestre do ano é o melhor para se vender um imóvel a partir do bairro que se encontra.
2. O valor de venda deve ser o valor de compra + a diferença para a média + 15%.


### A House Rocket deveria fazer uma reforma para aumentar o preço da venda? Quais seriam as sugestões de mudanças? Qual o incremento no preço dado por cada opção de reforma?
1. Uma reforma deve ser realizada caso a condição da casa seja inferior a 3 ou o lucro esperado seja abaixo de 10%.
2. Partimos do pressuposto que reformas podem agregar 30% ao valor do imóvel e que o gasto será de 5% sobre o preço de compra.
3. As mudanças sugeridas de acordo com alguns artigos são:
- Concertos simples, por exemplo troca de partes velhas e desgastadas como fiação. (Depende da condição da casa, caso a casa seja bem nova, não acrescentaria muito)
- Reformas na estrutura basica, melhorando o design interior.(ROI mínimo de 75%)
- Transformar espaços vazios em espaços utilizaveis como escritórios, sala de jogos, entre outros. (O incremento no preço depende do quê será construído no lugar)
- Reforma da cozinha. (Você pode recuperar de 53% a 72% na reforma da cozinha)
- Paisagismo. (ROI esperado de 150% a 1000%)
- Reforma do espaço externo, o deixando mais acessível e útil. (ROI mínimo esperado de 64%)


# Insights
Por meio da análise exploratória de dados, adquirimos alguns insights de negócios:

- **Poucos são os imóveis com vista para o mar, menos de 1%.**
<p align="left">
  <img src="https://github.com/leorviana/imoveis_house_rocket/blob/main/images/hist_waterfront.png">
</p>



- **93% dos imóveis não possuem vista ou possuem uma vista péssima.**
<p align="left">
  <img src="https://github.com/leorviana/imoveis_house_rocket/blob/main/images/hist_view.png">
</p>



- **Menos de 1% dos imóveis estão em condições péssimas, a grande maioria, 65% se encontra em condições razoáveis.**
<p align="left">
  <img src="https://github.com/leorviana/imoveis_house_rocket/blob/main/images/hist_condicao.png">
</p>



- **Apenas 3% dos imóveis já foram reformados.**
<p align="left">
  <img src="https://github.com/leorviana/imoveis_house_rocket/blob/main/images/hist_ja_reformado.png">
</p>



- **Imóveis com estruturas e designs mais elaboradas são bem mais caros.**
<p align="left">
  <img src="https://github.com/leorviana/imoveis_house_rocket/blob/main/images/grade.png">
</p>



- **Imóveis próximos ao lago Washington possuem os valores mais elevados e Imóveis em Seattle são mais caros.**
<p align="center">
  <img src="https://github.com/leorviana/imoveis_house_rocket/blob/main/images/mapa_kc.png">
</p>



- **Os 5 atributos que mais influenciam o preço dos imóveis são, em ordem:**
<p align="center">
  <img src="https://github.com/leorviana/imoveis_house_rocket/blob/main/images/correlacao.png">
</p>

    1. O nível de estrutura e design da casa.
    2. O tamanho do imóvel.
    3. A localização(Latitude).
    4. O nível da vizinhança.
    5. O numéro de banheiros.



# Resultados

#### - Com a sugestão de adquirir apenas imóveis abaixo do preço médio da região e em bom estado de conservação, a House Rocket deixa de comprar imóveis supervalorizados e em mau estado que provavelmente não seriam vendidos facilmente, podendo até passar por uma reforma, o que aumentaria ainda mais o custo.
<p align="center">
  <img src="https://github.com/leorviana/imoveis_house_rocket/blob/main/images/df_1.png">
</p>


#### - O melhor período do ano para se realizar negociações de imóveis em King County é no 2° trimestre do ano, seguido do 3°, 1° e 4°.
<p align="center">
  <img src="https://github.com/leorviana/imoveis_house_rocket/blob/main/images/melhor_epoca.png">
</p>


#### - Como visto na seção *Regras de Negócio*, nos estipulamos algumas regras para decidir quais imóveis comprar e por qual valor vender. Seguindo este caminho, a empresa podera faturar aproximadamente R$1,149,236,965.70
<p align="center">
  <img src="https://github.com/leorviana/imoveis_house_rocket/blob/main/images/df_2.png">
</p>


#### - Também estipulamos regras para reformar alguns imóveis, com este plano a empresa iria reformar cerca de 2845 casas e o retorno esperado com a valorização dos imóveis pela reforma é de aproximadamente R$272,456,178.42
<p align="center">
  <img src="https://github.com/leorviana/imoveis_house_rocket/blob/main/images/df_ref.png">
</p>


#### - No total, o lucro esperado com este plano é de aproximadamente R$1,421,693,144.12, com um ROI de 30%.
<p align="center">
  <img src="https://github.com/leorviana/imoveis_house_rocket/blob/main/images/retorno_esperado.png">
</p>


# Conclusão
Ao final deste projeto foi possível chegar a um número muito bom para maximizar os lucros da 'House Rocket', o CEO agora tem em mãos quais casas devem ou não comprar, o preço de venda e se precisam ou não de reforma, sendo assim é correto afirmar que o objetivo principal deste projeto foi alcançado com sucesso.


# Próximos passos
Construir um modelo de precifiação com aprendizado de máquina que irá retornar o valor esperado para um imóvel a partir de suas características, assim melhorando nossas escolhas de quais imóveis comprar, pois estamos atualmente utilizando um modelo de taxa base com a média do valor apenas.


# Referências
House Sales in King County, USA. Kaggle. Disponível em : <https://www.kaggle.com/harlfoxem/housesalesprediction>.

Blog “Seja um DataScientist - Meigarom”. Disponível em: <https://sejaumdatascientist.com/>.

FOSTER, Brittany. "10 Home Improvement Projects That Add Value to Your Property". **moneycrashers**. Disponível em: <https://www.moneycrashers.com/7-home-improvements-to-increase-its-value/>.

GERHARDT, Nick. "20 Home Renovations That Instantly Increase Your Home Value". **familyhandyman**. Disponível em: <https://www.familyhandyman.com/list/home-renovations-that-instantly-add-value-to-your-home/>.

"Reformar para vender vale a pena?". **entendaantes**. Disponível em: <https://entendaantes.com.br/reformar-para-vender-vale-a-penaentenda-antes/>.
