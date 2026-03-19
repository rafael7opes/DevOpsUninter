# Atividade Prática de DevOps: Conteinerização com Docker

Este repositório contém um projeto prático desenvolvido para a disciplina de DevOps. 

O foco deste trabalho não foi o desenvolvimento do código-fonte, mas sim a criação da **infraestrutura** necessária para rodar a aplicação. O sistema base (desenvolvido em Java) foi fornecido pelo professor, e o meu objetivo foi aplicar os conceitos de DevOps para "empacotar" esse sistema usando Docker.

## O que eu fiz neste projeto:
* **Criação do `Dockerfile`:** Escrevi as instruções passo a passo para montar o ambiente do zero.
* **Conteinerização:** Gerei a imagem da aplicação, garantindo que ela tenha tudo o que precisa (dependências, versão correta do Java, etc) para rodar isolada da máquina local.
* **Versionamento:** Subi a estrutura completa para o GitHub usando comandos do Git.

## Tecnologias Envolvidas
* **Docker:** Para a criação da imagem e do container.
* **Java:** Linguagem base da aplicação fornecida.
* **Git e GitHub:** Para versionamento e documentação do repositório.

## Como testar a infraestrutura

Para rodar este container na sua máquina, você só precisa ter o [Docker](https://www.docker.com/) instalado. Não é necessário instalar o Java nem configurar variáveis de ambiente localmente.

**1. Clone o repositório:**
`git clone https://github.com/rafael7opes/DevOpsUninter.git`

**2. Entre na pasta:**
`cd DevOpsUninter`

**3. Construa a imagem Docker:**
`docker build -t app-java-devops .`

**4. Execute o container:**
`docker run -p 8080:8080 app-java-devops`

*(Nota: a porta pode variar dependendo da configuração original da aplicação).*
