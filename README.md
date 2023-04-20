<h1>Docker Todo List</h1>

> Status do Projeto: :heavy_check_mark: :warning: (concluído)

## 💻 Objetivo do projeto 

<p align="justify">
  Conteinerizar a aplicação Full Stack permitindo ao usuário criar sua própria lista de tarefas adicionando, editando e removendo items. O principal desafio desse projeto foi dockerizar a aplicação, criando as imagens e orquestrando seu funcionamento via docker-compose. 
</p>

## 🛠 Tecnologias

<div>
    <img src='https://img.shields.io/badge/eslint-3A33D1?style=for-the-badge&logo=eslint&logoColor=white' alt='ESlint' />
    <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="NodeJS"/>
    <img src="https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white" alt="Docker"/>
</div>

### Alinhamento de código
- [ESlint](https://eslint.org/)

**Obs.:** Os arquivos presentes na pasta todo-app foram disponibilizados pela [Trybe](https://www.betrybe.com/) para a realização deste projeto.

## :warning: Dependências

```bash
npm install
cd docker
``` 

## 🚀 Como executar o projeto

Para executar a aplicação inicie realizando o clone deste repositório com o comando abaixo.

    git clone git@github.com:marcellsa/docker-todo-list.git
    
Navegue até o diretório **docker** do projeto.

    cd docker-todo-list/docker

<details>
   <summary><strong>Rodando a aplicação com o Docker</strong></summary> 
  </br>
  
  <strong>Obs:</strong> Para rodar a aplicação dessa forma você deve ter o [Docker](https://www.docker.com/) instalado na sua máquina.
  
  </br>
  
  Instale as depedências do projeto na pasta back-end, fornt-end e tests rodando o comando abaixo em cada pasta

        npm install
  
  Na pasta docker do projeto, suba o container <strong>todofront</strong>, <strong>todoback</strong> e <strong>todotests</strong> utilizando o docker-compose.yml. Utilize o comando abaixo.

        docker-compose up -d

Entre no terminal do container de back-end

        docker exec -it todoback bash

Dentro do terminal, inicie o servidor

        npm run dev
        
 Entre no terminal do container de front-end
    
        docker exec -it todofront bash
        
 Inicie a aplicação react com o comando abaixo dentro do terminal do container
    
        npm start

</details>

---

Desenvolvido por [Marcel Albuquerque](www.linkedin.com/in/marcellsa), © 2022.
