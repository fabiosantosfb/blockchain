# Blockchains

## Instalação

1. Verifique se o [Python 3.6+](https://www.python.org/downloads/) está instalado. 
2. Instale a [pipenv](https://github.com/kennethreitz/pipenv). 

```
$ pip install pipenv 
```
3. Requisitos de instalação 
```
$ pipenv install 
``` 

4. Execute o servidor:
    * `$ pipenv run python blockchain.py` 
    * `$ pipenv run python blockchain.py -p 5001`
    * `$ pipenv run python blockchain.py --port 5002`
    
## Docker

Outra opção para executar este programa blockchain é usar o Docker. Siga as instruções abaixo para criar um contêiner local do Docker:

1. Clonar este repositório
2. Construa o contêiner de janela

```
$ docker build -t blockchain .
```

3. Execute o contêiner

```
$ docker run --rm -p 80:5000 blockchain
```

4. Para adicionar mais instâncias, varie o número da porta pública antes dos dois pontos:
```
$ docker run --rm -p 81:5000 blockchain
$ docker run --rm -p 82:5000 blockchain
$ docker run --rm -p 83:5000 blockchain
```