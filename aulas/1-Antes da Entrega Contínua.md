[<< AULA ANTERIOR](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-01/aulas/6-Entrega%20Cont%C3%ADnua%20vs%20Deploy%20Cont%C3%ADnuo.md)



Definimos a entrega contínua e definimos seu elemento mais importante: o pipeline ue garante a entrega de valor para o cliente.

Descobriremos qual é a base para começar a implementar esta metodologia em nosso ambiente de trabalho. Quais são os princípios e fundamentos da entrega contínua?

Primeiramente precisamos começar com a integração contínua, que já estudamos no curso anterior, e as regras de outro desse processo são:

* Build automatizado
* Testes contínuos
* Gerenciamento de configuração

Devemos realizar builds automatizados a fim de minimizar erros no processo, além de realizar testes contínuos de escalas diferentes que sejam claros e significativos e criar ambientes fáceis de reproduzir em qualquer máquina.

Antes de pensarmos em entrega contínua já teremos várias etapas anteriores que devem ser respeitados. Devemos lembrar que integração contínua não é o uso de uma ferramenta de gestão específica ou geração de relatórios, mas uma metodologia ágil que envolve alguns pressupostos, como master "deployavel".

Feito isso a equipe pode tentar estender o servidor de integração em uso e criar uma pipeline, mas neste caso existem alguns princípios arquiteturais que devemos aplicar.


[PRÓXIMA AULA >>](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-02/aulas/2-Princ%C3%ADpios.md)
