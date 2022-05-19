[<< AULA ANTERIOR](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-02/aulas/4-Elementos%20Principais.md)

Nesta aula entraremos de fato no deployment pipeline. No curso anterior sobre integração contínua utilizamos a metáfora do "botão de integração" que é acionado e o código sincronizado com qualidade e sem problemas.

Agora não queremos apenas integrar, mas mostrar a alteração para o cliente, por isso seria interessante um botão de "release". Mas para essa lógica funcionar devemos ter cuidado, devemos garantir por meio de etapas a qualidade do nosso produto.

Conheceremos as etapas clássicas do deploy.

**1. Build**

O começo de tudo é a build, isto é o desenvolvedor vai construir o software.

**2. Testes de aceitação automatizados**

Depois da construção do software são executados os testes necessários. Por meio dos testes criamos relatórios sobre a qualidade do sistema. Se alguma etapa falhar ela é congelada por aqui e o artefato não é promovido.

**3. Homologação UAT**

A próxima etapa - caso tudo ocorra como o esperado - é a promoção do artefato. Este é o ambiente classico de User Acceptance Testing, ou simplesmente homologação. Nesta fase não executamos os testes mais complexos e que não podem ser automatizados.

**4. Produção**

Depois da aprovação manual, iremos para o ambiente de produção, em que o artefato será de fato produzido de maneira segura.

Cada etapa citada constrói mais confiança no produto. Os testes não garantem tudo, mas diminuímos muito a probabilidade de erros. O ambiente de homologação deve ser o mais parecido possível com o de produção para garantirmos a eficiência do deploy.

Nesse processo podem ter outras etapas. Abaixo teremos um exemplo um pouco mais sofisticado de pipeline, com unit tests, analysis AAT, homologação, testes de performance e produção.

![01](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-03/aulas/imagens/1-1-pipe.png)

O pipeline representa o processo de produção específico de uma equipe ou empresa, portanto não temos um padrão rígido.

Temos outro exemplo de pipeline que exibe o que acontece no momento em que é detectada uma falha no software. Além das etapas clássicas, temos a equipe (chamada delivery team) e o controle de versão. '

![02](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-03/aulas/imagens/1-2-wiki.png)

O processo de pipeline se inicia a cada comit que é testado separadamente. Nesta etapa os desenvolvedores utilizam ferramentas como Slack ou Telegram para se comunicarem sobre o estado do build, e se acontece algum problema toda a equipe é responsável.



[PRÓXIMA AULA >>](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-03/aulas/4-Boas%20Pr%C3%A1ticas.md)
