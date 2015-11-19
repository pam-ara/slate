Slate
------------------------------

### Pré-requisitos

Você vai precisar:

 - **Linux or OS X**
 - **Ruby, version 1.9.3 or newer**
 - **Bundler** — (gem install bundler).

### Executando

 1. Clone esse repositório `git clone https://github.com/pam-ara/slate.git`
 2. `cd slate`
 3. Instale [Docker](https://docs.docker.com/)
 4. `docker build -t slate .`
 5. `docker run -d -p 4567:4567 --name slate -v $(pwd)/source:/app/source slate`

*Sua doc estará disponível em `boot2docker ip:4567`


Atualizando a Doc
------------------------------

1. Criar a branch gh-pages `git checkout --orphan gh-pages`
2. Remova todos os arquivos `git rm -rf .`
3. Commitar e dar push das alterações no master
4. Executar a VM no docker
5. Compilar os HTMLs e dar push para a branch gh-pages `rake publish`
6. Docs disponível em http://yourusername.github.io/slate
