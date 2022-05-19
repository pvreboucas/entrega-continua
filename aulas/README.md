[<< ANTERIOR](https://github.com/pvreboucas/entrega-continua-cd/tree/aula-05/aulas)

# Para saber mais: The Twelve-Factor App

**The Twelve-Factor App** é um site (ou metodologia) que define 12 boas práticas para construir software na era de nuvem. Muitas das boas práticas discutidas no curso aparecem no Twelve-Factor, assim como gerenciamento de configuração, portabilidade entre ambientes ou implantação contínua. Vale conferir!

* [The Twelve-Factor App](https://12factor.net/pt_br/)

# O que Aprendemos?


Nesta aula, falamos sobre estratégias ou patterns de implantação. Foi importante mencionar que o __*deploy*__ e o __*release*__ são duas operações distintas. Ou seja, podemos fazer deploy da aplicação, mas mesmo assim ainda não publicar as novas features.

Ter features invísiveis para o cliente também é chamado de __*dark launching*__, quando já implantamos o novo software, mas o cliente ainda não tem acesso (ou só alguns clientes).

Resumindo:

* Vimos a diferença entre *deploy* (implantação) e *release* (publicação)
   * *Deploy* é colocar as alterações em produção (provisionar, configurar, instalar)
   * *Release* é deixar as alterações visíveis

Os padrões para o *release* do software são:

* *Blue-Green Deployment*
* *Canary Release*
* *Feature Toggles*

