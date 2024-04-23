# DevOps Challenge

## Requisitos

- Git
- Docker
- Curl ou Postman

## Instruções de Execução

### Passo 1: Clonar o Repositório

Clone o repositório no seu ambiente local e navegue até o diretório do projeto:

```bash
git clone https://github.com/anextbr/devops-challenge.git
cd devops-challenge
```

### Passo 2: Construir a Imagem Docker

Construa a imagem Docker a partir do Dockerfile fornecido:

```bash
docker build -t <nome_da_imagem> .
```

### Passo 3: Executar o Container de forma interativa

Execute o container a partir da imagem que você construiu:

```bash
docker run -it <nome_da_imagem>
```

### Passo 4: Acessar o Shell do Container

Se precisar interagir com o ambiente interno do container, use o seguinte comando, substituindo <nome_do_container> pelo nome ou ID do container em execução:

```bash
docker exec -it <nome_do_container> /bin/bash
```

### Passo 5: Limpeza

Ao concluir os testes, não se esqueça de parar e remover os containers e imagens criados para evitar uso desnecessário de recursos:

```bash
docker stop <nome_do_container>
docker rm <nome_do_container>
docker rmi <nome_da_imagem>
```