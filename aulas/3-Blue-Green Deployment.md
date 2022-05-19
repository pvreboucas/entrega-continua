[<< AULA ANTERIOR](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-06/aulas/1-Releases%20de%20baixo%20risco.md)



Anteriormente, mencionamos alguns princípios para deploys de baixo risco. Para garantir a segurança do nosso deploy, devemos aplicar algumas estratégias de release.

Temos duas questões principais:

* Como evitar que a aplicação fique offline durante o deploy (zero downtime)?

* Como voltar para a versão anterior (rollback) em caso de erro?

Começaremos por conhecer o **Blue/Green Deployment**. Tecnicamente, o deploy já foi realizado, mas temos duas versões: uma antiga(azul) e a nova(verde) que já está em ambiente de produção.

Entre as versões há um roteador, então em algum momento podemos modificar o fluxo para o novo ambiente, a nova versão. O ambiente velho (blue) fica no ar ainda um bom tempo caso algum problema surja. As conexões que existiam para o azul ficarão disponíveis até que realmente apenas a versão verde esteja totalmente funcional.



[PRÓXIMA AULA >>](https://github.com/pvreboucas/entrega-continua-cd/blob/aula-06/aulas/5-Feature%20Toggles%20e%20Canary%20Release.md)
