[<< AULA ANTERIOR](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-04/aulas/1-Commit%20Stage.md)



Continuaremos nosso curso de entrega contínua, e lembraremos que nosso foco é o pipeline de deploy. Neste vídeo estudaremos a etapa de testes de aceitação automatizados. Nesta fase queremos testar a aplicação inteira e avaliar se ela preenche os requisitos de negócio. Esta é uma etapa essencial para chegar ao deploy contínuo e inserir a aplicação na fase de produção de maneira segura.

Diferente dos testes de unidade, esse tipo de teste garante que as funcionalidades em conjunto estejam plenamente operantes e antederão o requisito do cliente. Tais testes são caros e trabalhosos, portanto é fácil de pular esta etapa devido ao seu custo e dificuldade.

Vamos utilizar um exemplo concreto: imagine que façamos uma refatoração na base do código e vários pontos são modificados. Neste momento, vários testes irão quebrar, por isso que a base de testes também deve ser atualizada, e neste momento como podemos garantir que um novo bug não foi criado?

Os testes de aceitação acessam a interface do software, como seria a experiência de usuário, e a ferramenta clássica para esta etapa é o Selenium. O teste de aceitação fornece uma garantia maior do ponto de vista do usuário.

Neste teste, a primeira fase é nosso artefato está disponibilizado em um repositório, e caso tudo tenha ocorrido certo o pipeline é notificado e sistemas como Jekings fazem o papel necessário nesta fase.

O ambiente precisa ser todo configurado, e ele precisa ser o similar ao ambiente de produção. Esta etapa é fundamental, porque se não ocorrem erros aqui a chance de algum imprevisto se dar na etapa de produção é muito reduzida.

Antes de executarmos todos os testes - já que são demorados - faremos o que é conhecido como smoke tests, testes menores que garantirão que as partes fundamentais da aplicação estão operantes.

O resultado dessa operação é um relatório que notificará a equipe do status da aplicação. Esta é uma etapa muito importante, afinal é a última fase dos testes automatizados, em seguida teremos uma maior presença humana.

Em resumo:

* equipe define as especificações (analistas,qa,dev)
* responsabilidade a equipe
* smoke tests para o ambiente
* mock de sistemas externos
* bons requisitos
* boas práticas no design e implementação de testes
* desempenho não é o mais importante

A responsabilidade da definição do teste é divida entre toda equipe, assim como a correção de erros. Para garantir que o ambiente está adequado, devemos realizar um conjunto de pequenos testes dos rescursos principais. Precisamos de bons resiqusitos para escrever as especificações e o teste na aplicação final real. Testes de aceitação são caros de escrever e manter, por isso desde o início devemos utilizar boas práticas no momento de criá-los. O desempenho importa,claro, mas não é o mais importante, geralmente são lentos.


[PRÓXIMA AULA >>](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-05/aulas/1-Stage%20de%20Homologa%C3%A7%C3%A3o.md)
