[<< AULA ANTERIOR](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-05/aulas/1-Stage%20de%20Homologa%C3%A7%C3%A3o.md)



A todo tempo falamos das quatro etapas do pipeline de deploy e que uma boa prática é não permitir que ela cresça demais horizontalmente, isto é, devemos focar nestas 4 etapas.

Em paralelo a homologação, podemos executar o "Capacity Testing Stage". A pergunta que queremos responder é: como garantir que o software realmente suporta a quantidade de requisições, transações e acessos de usuários?

Criar esses cenários é algo complexo, existem ferramentas disponíveis e este é um conteúdo para um curso específico. O cenário de produção é algo dinâmico, pois precisamos pensar e reproduzir o comportamento dos usuários.

Os testes de carga buscam descobrir qual é a real capacidade do nosso sistema, ou seja, seu baseline. Conhecendo nosso sistema, devemos estabelecer metas claras e utilizar ferramentas de monitoração para descobrir as modificações arquiteturais que são necessárias.

Estes testes são mais caros devido a sua complexidade. Na fase de homologação não precisamos rodar a cada commit ou build, mas que o projeto seja monitorado desde o início. Podemos começar pelos testes de aceitação e criar um cenário, para elaborar os testes de carga ou fazer um replay dos dados de reprodução: gravamos o comportamento das requisições e realizamos um replay desses dados. Algumas ferramentas que podemos utilizar para isto são JMeter, Getling, Webbload, Apache Bench, LoadNinja.

Mesmo depois de passarmos para a produção, ainda existem riscos possíveis, e este problema trabalharemos nas próximas aulas.


[PRÓXIMA AULA >>](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-06/aulas/1-Releases%20de%20baixo%20risco.md)
