# desafio-devops-pigz
Repositório da solução do desafio referente ao cargo devops

# Conclusão
Consegui fazer rodar a aplicação completa, na minha resolução tem dois Dockerfile um para a configuração do php fpm com symfony e o outro para a configuração padrão do nginx. 
Foi modificado tambem o arquivo default.conf para executar um projeto symfony.
Ambos estão sendo chamado em um arquivo docker-compose que especifica a criação das imagens.
Foi feita tambem a configuração do Github Actions para o build do docker e enviar para o docker hub em um repositorio a cada push na branch main.

# Como executar
- Git clone na maquina local
- Acessar a pasta backend, e no terminal executar o comando `docker-compose up -d --build` 
- ir no navegador e acessar http://localhost:8080/

