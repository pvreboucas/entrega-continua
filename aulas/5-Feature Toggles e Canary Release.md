[<< AULA ANTERIOR](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-06/aulas/3-Blue-Green%20Deployment.md)



Aprendemos anteriormente sobre o Blue/Green Deployment, que oscila entre duas versões da aplicação: uma mais nova e outra mais antiga. Já o Canary Release executa ações parecidas, na verdade, podemos pensar que se trata de uma evolução.

Neste caso, as duas versões são utilizadas ao mesmo tempo, tanto azul quanto a verde, mas a nova versão não é acessada por todos os usuários. Uma parcela dos usuários que têm acesso a nova versão serão agentes de um teste.

O critério de direcionamento da nova versão em teste para alguns usuários varia, podemos usar 5% do nosso tráfego para a nova versão e monitorar o comportamento do sistema. Outro critério possível é o geográfico ou em estratégias de mercado, idade e assim por diante, isso vai variar de acordo com as necessidades do negócio e dados disponíveis sobre os usuários.

Uma vez que o teste for concluído, os usuários integralmente são direcionados para a nova versão. Esse metodologia também é utilizada para A/B Test.

O Canary Release é muito utilizado, e também é conhecido como "dark lauching" em tradução livre "lançamento no escuro", afinal nem todos os usuários sabem que existe um novo feature.

Outra estratégia com o mesmo objetivo é o Feature Toggles, também um dark lauching, mas neste caso trata-se de uma configuração no código que disponibiliza um switch de versões.

Um exemplo é quando é oferecida a consdição de "beta tester" para o usuário de alguma aplicação, caso a resposta seja positiva, alguma configuração no cadastro possibilitará o acesso à nova feature. Mas temos a mesma base de código, não são duas versões blue ou green.

Esta estratégia pode ser combinada ao Canary Release: uma parcela dos usuários que será direcionado para a versão nova utilizará o Feature Toggles habilitado. Há pessoas que defendem que toda a nova funcionalidade deve ser um Feature Toggles, mas para isso ser implementado de maneira correta deve-se elaborar uma estratégia para lidar com essa proposta.


[PRÓXIMA AULA >>](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-06/aulas/9-Conclus%C3%A3o.md)
