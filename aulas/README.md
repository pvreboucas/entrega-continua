[<< ANTERIOR](https://github.com/pvreboucas/entrega-continua-cd/tree/aula-03/aulas)

# O que Aprendemos?

Nesta aula, definimos as etapas/stages de commit e de testes de aceitação automatizados (AAT):

* Ambas as etapas executam os testes de maneira automatizada
* O stage de commit foca nos testes de unidade e integração.
* O stage AAT foca nos testes funcionais, que testam o sistema todo, baseado em um requisito
* O commit stage deve executar rápido (menos de 10 minutos) e iniciar a cada commit
* O stage AAT inicia quando commit stage foi executado com sucesso
* O stage AAT é mais demorado

Os testes de aceitação são mais caros de escrever e manter, mas trazem muito valor, pois testam o sistema todo. Os testes de aceitação são escritos pela equipe inteira (analista, desenvolvedor, etc).

Quando um build quebra, todos são responsáveis. Consertar o problema é prioridade da equipe.


[PRÓXIMO >>](https://github.com/pvreboucas/entrega-continua-cd/tree/aula-05/aulas)
