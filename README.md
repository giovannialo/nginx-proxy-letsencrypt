# Nginx Proxy + Let's Encrypt

Automação de proxy reverso usando Nginx com o Let's Encrypt para Docker.

## Dependências

* Docker Compose;
* Rede **venus**.

## Instalação

Siga as etapas abaixo para um correto funcionamento do sistema.

### Rede venus

Para efetivar uma comunicação entre os serviços que utilizarão o proxy reverso, é preciso que todos os containers
estejam utilizando a mesma rede. Execute o comando abaixo para criar a rede **venus**.

```docker
docker network create --driver bridge venus
```

### Containers

Execute o comando abaixo para criar e iniciar os containers.

```docker
docker-compose up -d
```

## Credits

* [Giovanni Alves de Lima Oliveira](https://github.com/giovannialo) (Developer)
