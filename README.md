# desafio-devops-pigz
Repositório da solução do desafio referente ao cargo devops

# Conclusão
Consegui fazer rodar a aplicação completa, na minha resolução tem dois Dockerfile um para a configuração do php fpm com symfony e o outro para a confuguração padrão do nginx.
Ambos estão sendo chamado em um arquivo docker-compose que especifica a criação das imagens.
Foi feita tambem a configuração do Github Actions para o build do docker e enviar para o docker hub em um repositorio a cada commit na branch main.

# Como executar
- Git clone na maquina local
- Acessar a pasta backend, e no terminal executar o comando `docker-compose up -d --build` 
- ir no navegador e acessar http://localhost:8080/
