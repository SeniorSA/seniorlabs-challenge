# Desafio Data Science

A quantidade de spams (mensagens não solicitadas) que recebemos diariamente, não para de crescer. Os tipos de spam são diversos: anúncios de produtos / web sites, esquemas para ganhar dinheiro rápido, correntes, pornografia e etc.

## Input

O arquivo [sms_senior.csv](sms_senior.csv) contém vários exemplos de mensagens comuns (4827 unidades) e
mensagens spams (747 unidades). As mensagens foram submetidas a uma etapa de mineração de
texto, com o objetivo de identificar as palavras mais frequentes na base de dados. 

Seguem as informações dos atributos do arquivo:
* 1 coluna contendo a mensagem original (Full_Text);
* 149 colunas com valores inteiros que indicam a frequência de uma determinada palavra na
mensagem ("got"... "wan");
* 1 coluna contendo a quantidade de palavras frequentes na mensagem
(Common_Words_Count);
* 1 coluna contendo a quantidade total de palavras da mensagem (Word_Count);
* 1 coluna contendo a data de recebimento da mensagem (Date);
* 1 coluna que identifica se a mensagem é spam ou não (IsSpam).

## Primeira Etapa

A primeira etapa do seu trabalho consiste em extrair estatísticas desta base de dados:

1. Exibir gráfico as palavras mais frequentes em toda a base de dados (Ex.: gráfico de barras,
nuvem de palavras, etc).
2. Exibir gráfico com as quantidades de mensagens comuns e spams para cada mês;
3. Calcular o máximo, o mínimo, a média, a mediana, o desvio padrão e a variância da quantidade
total de palavras (Word_Count) para cada mês;
4. Exibir o dia de cada mês que possui a maior **sequência** de mensagens comuns (não spam).

## Segunda etapa

A segunda etapa consiste em aplicar um método capaz de classificar automaticamente as mensagens
como “comum” e “spam”. Como você considera os resultados encontrados? Justifique.

## Output

Você pode utilizar qualquer linguagem de programação e ferramentas de software para extrair as informações das duas etapas do trabalho. Por fim, descreva o trabalho realizado em um artigo.

Lembre-se de apontar as estatísticas extraídas e de explicar
o método de classificação utilizado, como a etapa de treinamento e classificação foram executadas,
além dos resultados que foram encontrados.

O modelo parece grande, mas você pode ser bem objetivo. Os códigos fontes ou arquivos utilizados
no trabalho deverão ser postados no github, onde o README deve explicar como proceder para
executar sua solução.