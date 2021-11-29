# Senior Labs Challenge

O Senior Labs é o laboratório de pesquisa aplicada da Senior Sistemas. Neste laboratório, trabalhamos com as tecnologias que são tendência no Brasil e no Mundo.
As pessoas que trabalham no laboratório tem como característica uma boa base acadêmica, a vontade de explorar novos desafios e a determinação para encontrar o caminho para a aplicação destas pesquisas nos produtos e serviços.
Trabalhamos com tecnologias como IA, IoT, Cloud Computing, Computer Vision e muito mais.
Se identifica com tudo isso? Realize um de nossos desafios técnicos e você estará habilitada a participar de nossas vagas.

## Desafios

Temos 2 (dois) desafios diferentes. Um deles é focado em Data Science e outro em Software Engineering.

Você pode escolher aquele que mais se identifica ou até mesmo aquele que gostaria de trabalhar. Fique a vontade também para realizar ambos. :)

### Desafio Data Science

A quantidade de spams (mensagens não solicitadas) que recebemos diariamente, não para de crescer. Os tipos de spam são diversos: anúncios de produtos / web sites, esquemas para ganhar dinheiro rápido, correntes, pornografia e etc.

#### Input

O arquivo sms_senior.csv contém vários exemplos de mensagens comuns (4827 unidades) e
mensagens spams (747 unidades). As mensagens foram submetidas a uma etapa de mineração de
texto, com o objetivo de identificar as palavras mais frequentes na base de dados. 

Segue as informações dos atributos do arquivo:
* 1 coluna contendo a mensagem original (Full_Text);
* 149 colunas com valores inteiros que indicam a frequência de uma determinada palavra na
mensagem ("got"... "wan");
* 1 coluna contendo a quantidade de palavras frequentes na mensagem
(Common_Words_Count);
* 1 coluna contendo a quantidade total de palavras da mensagem (Word_Count);
* 1 coluna contendo a data de recebimento da mensagem (Date);
* 1 coluna que identifica se a mensagem é spam ou não (IsSpam).

#### Primeira Etapa

A primeira etapa do seu trabalho consiste em extrair estatísticas desta base de dados:
1. Exibir gráfico as palavras mais frequentes em toda a base de dados (Ex.: gráfico de barras,
nuvem de palavras, etc).2. Exibir gráfico com as quantidades de mensagens comuns e spams para cada mês;
3. Calcular o máximo, o mínimo, a média, a mediana, o desvio padrão e a variância da quantidade
total de palavras (Word_Count) para cada mês;
4. Exibir o dia de cada mês que possui a maior sequência de mensagens comuns (não spam).

#### Segunda etapa

A segunda etapa consiste em aplicar um método capaz de classificar automaticamente as mensagens
como “comum” e “spam”. Como você considera os resultados encontrados? Justifique.

#### Output

Você pode utilizar qualquer linguagem de programação e ferramentas de software para extrair as informações das duas etapas do trabalho. Por fim, descreva o trabalho realizado em um artigo com
duas ou três páginas no modelo anexo.

Lembre-se de apontar as estatísticas extraídas e de explicar
o método de classificação utilizado, como a etapa de treinamento e classificação foram executadas,
além dos resultados que foram encontrados.

O modelo parece grande, mas você pode ser bem objetivo. Os códigos fontes ou arquivos utilizados
no trabalho deverão ser postados no github, onde o README deve explicar como proceder para
executar sua solução

### Desafio Software Engineering

A marcação de ponto é um produto de HCM e é amplamente utilizado por empresas do Brasil para que seus colaboradores possam realizar a marcação de ponto diariamente para registrar sua jornada de trabalho. 

Uma característica desse sistema é que as marcações acontecem quase que em sua maioria em um intervalo de tempo muito pequeno, em torno de 5 minutos todos os colaboradores já fizeram sua marcação. Esse problema é potencializado pensando que milhares de colaboradores de centenas de empresas do Brasil todo fazem isso ao mesmo tempo por ser uma plataforma cloud. 

#### Solução 

Para esse desafio, queremos que você modele uma aplicação que resolva esse problema do aspecto funcional e também não funcional. 

De uma forma bastante simples, uma marcação de ponto tem:
* Código do funcionário 
* Código da empresa 
* Data e Hora da marcação 

A aplicação é apenas de backend e ela atende tanto dispositivos IoT, Mobile e Web. 

Considere que essa aplicação precisa integrar com um sistema legado para enviar as marcações e este sistema não possui um tempo de resposta muito adequado, em torno de 10 segundos para resposta. 

A URL que deve ser chamado do sistema legado é: https://api.mockytonk.com/proxy/ab2198a3-cafd-49d5-8ace-baac64e72222 

Payload de exemplo para a requisição: 

```json
{"includedAt":"2021-03-15 15:10:00", "employeeId": 123, "employerId": 999} 
```

Onde: 

* includedAt é a data e hora que ocorreu a marcação de ponto 
* employeeId é o código do funcionário que fez a marcação de ponto 
* employerId é o código da empresa em que o funcionário trabalha 

Desenvolva uma prova de conceito da modelagem do sistema que você fez. Não há preferência por linguagem de programação ou tecnologias que serão utilizadas para resolver o problema. É importante que seja reproduzível. 

Será um diferencial se for possível executar em um cloud provider. 

Nosso principal foco da avaliação é a arquitetura da aplicação, então queremos ver como ela pode ser de forma ideal. 

#### O que deve entregar 

* Artigo de até 5 páginas explicando o projeto, onde nesse artigo são esperados os seguintes tópicos 
    * Introdução: contextualização sobre o problema 
    * Desenvolvimento: a solução e o processo para chegar nela 
    * Conclusões 
* Código fonte em um repositório do GitHub 

#### Preparação 

Nosso pesquisador Leonardo Fiedler preparou um material onde dá várias dicas para se sair bem em desafios técnicos como este. Faça a leitura através do endereço abaixo: 

https://dev.to/leonardofiedler/dicas-para-mandar-bem-em-testes-tecnicos-231k 

## Regras

* Queremos que realize o desafio com um espaço de tempo limitado, para que possamos ter um *baseline*. Por isso, utilize apenas 1 (um) final de semana ou 3 (três) noites para realizar o desafio
* Caso queira evoluir no desafio, fique a vontade, mas documente isso de maneira isolada para nossa análise
