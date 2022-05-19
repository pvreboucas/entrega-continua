[<< AULA ANTERIOR](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-03/aulas/1-Etapas%20do%20Pipeline.md)


Lembremos as etapas clássicas do pipeline: build unit test, AAT, UAT e Produção. A pipeline é a única forma de realizar o deploy, assim chegamos em um estado seguro para o ambiente de produção. Outro ponto importante é o que o pipeline deve ser ágil, isto é, o seu desempenho dever ser satisfatório na resolução de problemas.

O build é a primeira etapa do projeto, e deve ser executado apenas uma vez, e sempre devemos utilizar o artefato inicial para evitar incompatibilidades.

O build em si deveria ser independente do ambiente, ou seja, o software não deve levar configurações hardcode. Já mencionamos também que os ambientes de homologação devem ser semelhantes ao ambiente de produção.

Os ambientes devem ser efêmeros, isto é, temporários. Não é uma ação sempre fácil de ser realizada em todos os projetos, mas é algo interessante, pois podemos criar cenários limpos para novos testes, afinal quando executamos um teste devemos criar um cenário para ele, e então analisar o comportamento do software.

Devemos garantir que o deploy para ambientes sempre seja igual, e esse escript que dará segurança ao pipeline. Idealmente devemos sempre utilizar a mesma maneira de deploy para cada fase do projeto.

Essas são algumas boas práticas da entrega contínua.


[PRÓXIMA AULA >>](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-04/aulas/1-Commit%20Stage.md)
