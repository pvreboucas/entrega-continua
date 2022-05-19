[<< ANTERIOR](https://github.com/pvreboucas/entrega-continua-cd/tree/aula-02/aulas)

# O que Aprendemos?

Nesta aula, começamos a ver mais detalhes sobre o deployment pipeline. Vimos os stages (etapas) principais de um pipeline, que são:

* Build/Commit stage
* Automated Acceptance Testing Stage (Testes de aceitação)
* User Acceptance Testing Stage (Homologação)

As etapas build e AAT são totalmente automatizadas. UAT é manual.

As etapas existem pois queremos receber feedback o mais rápido possível, ou seja, executamos os testes rápidos bem no início do pipeline.

Também falamos sobre algumas boas práticas na construção e execução do pipeline:

* O pipeline é a única forma de deploy
* O desempenho do pipeline importa, ou seja, otimize-o
* Build do artefato no início e apenas uma vez
* O build deve ser independente do ambiente
* Ambientes deve ser iguais ou muito semelhantes ao de produção
* Use ambientes efêmeros (temporários) onde puder
* O deploy deve ser executado igual para qualquer ambiente


[PRÓXIMO >>](https://github.com/pvreboucas/entrega-continua-cd/tree/aula-04/aulas)
