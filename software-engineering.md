# Desafio Software Engineering

A marcação de ponto é um produto de HCM e é amplamente utilizado por empresas do Brasil para que seus colaboradores possam realizar a marcação de ponto diariamente para registrar sua jornada de trabalho. 

Uma característica desse sistema é que as marcações acontecem quase que em sua maioria em um intervalo de tempo muito pequeno, em torno de 5 minutos todos os colaboradores já fizeram sua marcação. Esse problema é potencializado pensando que milhares de colaboradores de centenas de empresas do Brasil todo fazem isso ao mesmo tempo por ser uma plataforma cloud. 

## Solução 

Para esse desafio, queremos que você modele uma aplicação que resolva esse problema do aspecto funcional e também não funcional. 

De uma forma bastante simples, uma marcação de ponto dispõe dos seguintes atributos:

* Código do funcionário 
* Código da empresa 
* Data e Hora da marcação 

A aplicação é apenas de backend e ela atende tanto dispositivos IoT, Mobile e Web. 

Considere que essa aplicação precisa integrar com um sistema legado para enviar as marcações e este sistema não possui um tempo de resposta muito adequado, em torno de 10 segundos para resposta. 

A URL que deve ser chamada do sistema legado é a seguinte: 
* https://api.mockytonk.com/proxy/ab2198a3-cafd-49d5-8ace-baac64e72222 

Payload de exemplo para a requisição: 

```json
{"includedAt":"2021-03-15 15:10:00", "employeeId": 123, "employerId": 999} 
```

Onde: 

* *includedAt* é a data e hora que ocorreu a marcação de ponto 
* *employeeId* é o código do funcionário que fez a marcação de ponto 
* *employerId* é o código da empresa em que o funcionário trabalha 

## Instruções e dicas

* Identifique os principais problemas encontrados e arquiteture uma solução eficiente.

* Desenvolva uma prova de conceito da modelagem do sistema que você fez.  
- - Não há preferência por linguagem de programação ou tecnologias que serão utilizadas para resolver o problema. É importante que seja reproduzível. 

* Será um diferencial se for possível executar em um **cloud provider**. 

* Nosso principal foco da avaliação é a arquitetura da aplicação, então queremos ver como ela pode ser de forma ideal. 