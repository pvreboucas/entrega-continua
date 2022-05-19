[<< AULA ANTERIOR](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-01/aulas/3-Diminuindo%20Risco.md)

Comentamos sobre o coração da entrega contínua, o pipeline de deploy. Existem muitos formatos possíveis, mas ao observarmos essa representação gráfica, notaremos que existem uma série de etapas na construção de um projeto e cada uma delas possui complexidade específica.

![01](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-01/aulas/imagens/5-1-etapa.png)

O deploy é complexo, existem diversos componentes arquiteturais envolvidos que precisam ser escolhidos, configurados e alterados para que o software seja funcional.

É natural que um processo tão minucioso tenda a apresentar problemas, e o conceito de entrega contínua demandou muitas observações e meditações sobre esses infortúnios de projeto.

Discutiremos primeiramente quais são as más práticas ou "antipatterns" e então apresentar as alternativas.

**1. Gerenciamento manual de ambientes**

Cada ambiente precisa ser configurado e reconfigurado, e temos vários. Deveria ser fácil destruir o pipeline e reconstruí-lo com a mesma facilidade. Se etapas que já são complexas forem executadas manualmente teremos a presença de erros e inconsistências. Há casos em que o deploy funcionou em ambiente de homologação, mas não de produção, e é importante mencionar que são ambientes muito similares.

O mesmo pode ocorrer dentro do ambiente de produção, por exemplo o cluster, que possui várias máquinas envolvidas. Se as máquinas não forem idênticas a medida que o software se expande complexifica, teremos problemas. Isso ocorreu porque algo foi aplicado manualmente.

A regra de ouro é: Todos os ambientes são tratados como código, versionados e criados de maneira automatizada.

**2. Deploy manual**

Geralmente temos um manual que define as etapas de um deploy, mas geralmente a aplicação evolui e a documentação não é mais precisa e real. Há desenvolvedores que não sabem como o deploy é de fato realizado, afinal é um fazer delegado a poucas pessoas dentro da empresa em algumas configurações de equipe. Os deploys podem ser lentos e durarem horas ou dias. Nessa configuração teremos um deploy vagaroso, sujeito a erros e não confiável.

A regra de ouro é: apenas duas tarefas devem ser executadas manualmente: escolher a versão do release e o clique em "deploy buttom.

Dessa maneira qualquer pessoa da equipe pode realizar o deploy, o resto é automatizado, encapsulado e seguro.

**3. Deploy apenas no fim do ciclo**

Por exemplo, os desenvolveremos em aplicações estáveis e grandes focam em testes de criação de novas features e não interagem com a equipe de produção. Dessa maneira não sabemos se as novas features serão de fato funcionais e estáveis em produção.

Desse modo, teremos como resultado uma equipe pouco integrada, os problemas serão avistados apenas no dia da plubicação, e isso torna o processo mais lento.

A regra neste caso é: deployment faz parte do desenvolvimento desde a primeira interação, todos definem um delivery team.

Conhecemos três antipatterns clássicos que atrapalham a agilidade da construção de um projeto confiável. Devemos portanto ter:

* Gerenciamento automatizado de ambientes
* Deploy automatizado
* Deploy frequente em cada ciclo de desenvolvimento

[PRÓXIMA AULA >>](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-01/aulas/6-Entrega%20Cont%C3%ADnua%20vs%20Deploy%20Cont%C3%ADnuo.md)
