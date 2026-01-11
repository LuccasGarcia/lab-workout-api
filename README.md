## Projeto - API de Centro de Treinamento

Aplicação em Python utilizando FastAPI para gerenciar centro de treinamento de CrossFit vinculando o atleta à uma categoria.

### Preparando o ambiente
- Utilizar pyenv
````bash
pyenv virtualenv lab-workout-api
pyenv activate lab-workout-api
pip install -r requirements.txt
````

- Para subir o banco de dados, caso não tenha o docker-compose instalado, faça a instalação e logo em seguida, execute:

````bash
make run-docker
````
- Para criar uma migration nova, execute:

````bash
make create-migrations d="nome_da_migration"
````

- Para criar o banco de dados, execute:

````bash
make run-migrations
````

- Os comando do **make** estão configurados no arquivo **Makefile**.

### Executando a aplicação

- Para subir a API, execute:
````bash
make run
````
- Acesse: http://127.0.0.1:8000/docs
