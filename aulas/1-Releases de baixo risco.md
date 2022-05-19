[<< AULA ANTERIOR](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-05/aulas/3-Stage%20de%20Teste%20de%20Carga.md)



Nesta aula conversaremos sobre a última fase do pipeline: a produção. Mesmo nesta fase, ainda pensaremos em como inserir nossa aplicação com o menor risco possível, mesmo tendo passado por diversas etapas que irão ampliar a segurança e estabilidade do sistema ao longo do processo.

Era comum no meio dos desenvolvedores utilizar alguns "carimbos" de qualidade do software, como o Pré-Alpha, Alpha, Beta, Release Candidate e Release. Hoje em dia utilizamos o pipeline, com etapas sofisticadas com releases durante o desenvolvimento do projeto.

Já aprendemos ao longo do curso que a tarefa de redução de riscos deve começar ao início do projeto, lembremos de:

* deploy e pipeline desde a primeira interação em ambientes similares.

* automação, one-click deploy e smoke test ambiente

* aspectos arquiteturais: testability e deployability

Além desses pontos,temos o "The twelve-factor app", são 12 boas práticas documentadas que nos fornecerem uma referência de como a aplicação deve se comportar dentro de um ambiente de nuvem. Ainda tempos outras medidas para deixar o sistema ainda mais confiável na última fase do pipeline.

Já mencionamos que os deploys devem ser realizados de maneira contínua, este é o tema do nosso curso. Devemos realizar *releases incrementais *, mesmo que a funcionalidade seja grande devemos realizar a implementação e realizar o deploy, assim chegamos mais perto do estado final do sistema.

Sabemos eventualmente não podemos inserir o módulo de maneira parcial, por isso existe a técnica "Brench by Abstraction" que já discutimos no curso anterior. Criamos uma abstração dentro do código com dois caminho, em fase de desenvolvimento ele pode ser testado, embora na fase de produção ele não exista ainda.

A entrega contínua faz a diferença entre o deploy e o release, e até agora utlizamos essas duas palavras como se fossem a mesma coisa, e na verdade não o são.

Deploy é criar um ambiente, garantir que ele exista de maneira correta, instalar o software e configurá-lo. Já o release é a publicação de fato, o momento em que o cliente utiliza o produto.

Devemos desacoplar o deploy do release, e para isso existem estratégias como:

* Blue/Green Deployment
* Canary Releases
* Feature Toggles (Feature Flags)

Estudaremos mais detalhadamente cada uma dessas possibilidades adiante.


[PRÓXIMA AULA >>](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-06/aulas/3-Blue-Green%20Deployment.md)
