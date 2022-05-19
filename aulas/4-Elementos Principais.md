[<< AULA ANTERIOR](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-02/aulas/2-Princ%C3%ADpios.md)



Na aula passada aprendemos os princípios da entrega contínua e sua definição. Neste ponto, discutiremos os elementos que compõe essa metodologia, e temos três itens principais:

**1. Cultura DevOps.** Ela envolve: feedback, colaboração, confiança, melhoria e aprendizagem contínua.

**2. Patterns.** São os padrões de deploy, ou releases de baixo risco. Nós ainda discutiremos esse assunto ao longo do curso, alguns padrões são blue/green, canary, feature toggle e outros.

**3. Arquitetura.** A arquitetura é uma fase importante, pois quando falamos sobre arquitetura estamos mencionando a estrutura do sistema. As decisões estruturais são as mais difíceis dentro de um projeto, é necessário que ela seja estipulada no começo do trabalho. Quando pensamos na arquitetura queremos definir testabilidade, estabilidade, desempenho e outras propriedades como deployability.

Quanto melhor for a arquitetura do sistema, mais fácil será praticarmos entrega contínua. Se existem dificuldades em recriar o ambiente de produção isso influencia a testabilidade, afinal devemos criar um clone da produção para que o teste seja possível.

O mesmo se dá com o deployability. Se a base de código é muito grande, sentiremos dificuldade em inserir elementos na fase de produção. Nesta fase entram as boas práticas e os serviços e uma melhor base de dados.


[PRÓXIMA AULA >>](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-03/aulas/1-Etapas%20do%20Pipeline.md)
