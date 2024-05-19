# ToDoList Application 📝

## Descrição

Este é um projeto de uma aplicação de lista de tarefas (ToDoList) desenvolvida em Spring Boot. Ele permite aos usuários adicionar, remover e marcar como concluídas as tarefas em sua lista. 

Eu originalmente desenvolvi ele para que as pessoas que moram comigo possam contribuir em uma mesma lista de compras, assim utilizei uma conexão com o banco de dados Supabase e fiz o deploy da aplicação no site Render usando uma imagem com a aplicação que subi no DockerHub.😁

Agora a ideia é desenvolver um aplicativo apra consumir essa API e todos poderem visualizar a mesma lista.🤩

## Arquitetura

O projeto segue um padrão arquitetural em camadas, com as seguintes camadas:

- **Controller:** Responsável por receber as requisições HTTP e chamar os métodos apropriados do serviço.
- **Service:** Contém a lógica de negócios da aplicação, processando os dados recebidos dos controllers e interagindo com o repositório.
- **Repository:** Fornece uma interface para interagir com o banco de dados, executando as consultas SQL.

## Endpoints

- **GET /getList:** Retorna todas as tarefas da lista.
- **POST /addItem:** Adiciona uma nova tarefa à lista.
- **DELETE /delete:** Remove uma tarefa da lista.
- **PUT /checkItem:** Marca ou desmarca uma tarefa como concluída.

## Tecnologias Utilizadas

- **Spring Boot:** Framework para o desenvolvimento de aplicações Java.
- **Lombok:** Biblioteca para redução de código boilerplate.
- **H2 Database:** Banco de dados em memória para desenvolvimento.
- **Docker:** Utilizado para o empacotamento da aplicação em contêiner.
- **Render:** Plataforma de hospedagem utilizada para o deployment da aplicação.

## Instalação e Uso

1. Clone este repositório: `git clone https://github.com/seu-usuario/todo-list.git`
2. Certifique-se de ter o Docker instalado em sua máquina.
3. Navegue até o diretório do projeto.
4. Execute o seguinte comando para iniciar a aplicação: `docker-compose up`
5. Acesse a aplicação em `http://localhost:8080`.

## Contribuição

Qualquer contribuições é bem-vinda!😉 Sinta-se à vontade para abrir uma issue ou enviar um pull request.

Obrigada! 😄
