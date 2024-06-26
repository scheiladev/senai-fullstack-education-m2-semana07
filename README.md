# SENAI Fullstack [Education]

## Resolução dos exercícios da Semana 07 - Módulo 02

### M2S07 | Roteiro Projeto: Portal Educational - parte 1

Olá dev!

Nas próximas 2 semanas, as listas de exercícios serão contínuas, ou seja, começaremos um projeto único que será iniciado na semana 7 e finalizado na semana 8.

O projeto será um portal educacional, onde poderemos logar, visualizar o curso que estamos matriculados, consultar as matérias e outros serviços institucionais.

Ao longo dessa semana, essa lista de exercícios estará voltada para os conceitos de: Estruturação de um projeto Angular, Componentes, Formulários e Manipulação de Dados (interpolação, data binding, eventos).

### M2S07 | Ex. 01 - Criação do projeto

Nessa primeira tarefa, vamos criar o projeto Angular que servirá como base para os demais exercícios.

1. Crie um novo projeto angular para o projeto de portal educacional;
2. Coloque no comentário do card o comando utilizado para a criação do mesmo.

### M2S07 | Ex. 02- Estruturação dos componentes

Agora, vamos criar a estrutura dos componentes principais da aplicação. Utilizando o Angular CLI faça:

1. Crie uma pasta ‘shared’ e uma subpasta ‘components’ onde serão criados os componentes (não precisam de rotas):
   1. header
   2. sidebar
2. Crie os seguintes componentes/páginas na pasta 'app' (com rotas para acesso):
   1. login
   2. home
   3. alunos
   4. cadastro de aluno
   5. disciplinas

### M2S07 | Ex. 03- Criação da tela de login

Nesta atividade, vamos criar a estrutura da tela de login. Esta tela deverá conter:

- Os inputs:
  - E-mail (campo obrigatório)
  - Senha (campo obrigatório)
- Os botões:
  - Entrar
    - Quando clicado, caso ambos os campos do formulário estejam preenchidos, o usuário será redirecionado para a tela inicial/home.
  - Esqueci a Senha
    - Quando clicado, apresentará um alerta dizendo: “Processo de recuperação de senha enviado para o e-mail cadastrado”.

### M2S07 | Ex. 04- Criação da tela de cadastro de alunos

Neste exercício, vamos fazer a criação do componente de cadastro de alunos.

Esta tela irá conter um formulário com os seguintes elementos:

- Nome completo (input texto) (campo obrigatório)
- CPF (input texto) (campo obrigatório)
- E-mail (input texto) (campo obrigatório)
- Celular (input texto) (campo obrigatório)
- Curso (combo para seleção de um curso) (campo obrigatório)
- Botão Salvar:
  - Quando clicado, caso todos os campos obrigatórios estejam preenchidos, irá: salvar os dados inseridos, apresentar uma mensagem “Usuário salvo com sucesso” e redirecionar o usuário para a tela de listagem de usuários

### M2S07 | Ex. 05- Criação da tela de listagem de alunos

Aqui, vamos criar a funcionalidade onde iremos visualizar todos os alunos que temos em nosso sistema.

Esta tela irá conter:

- Um input para pesquisar alunos pelo nome OU email
- Um botão Pesquisar
- Uma tabela onde serão apresentados todos os alunos cadastrados. Ela possuirá as colunas:
  - Nome (do aluno)
  - CPF
  - E-mail
  - Curso (que ele está matriculado)
  - Ações (uma coluna com os botões):
    - Botão Editar
      - Quando clicado, redirecionará o usuário para a tela de cadastro de usuário com as informações do usuário selecionado já preenchidas para edição
    - Botão Excluir
      - Exibirá um alerta com a mensagem “Quer mesmo excluir este usuário?”, em caso positivo, o usuário será excluído e a listagem de usuários atualizada

### M2S07 | Ex. 06- Criação da tela de disciplinas

Aqui, vamos criar a funcionalidade onde os alunos irão visualizar todas as disciplinas que possuirão ao longo do curso escolhido.

Nela, deverão ser exibidos as disciplinas do curso que o usuário está inscrito, divididas por semestre.

Exemplo:

- Usuário inscrito no curso A, irá visualizar as disciplinas: Primeiro semestre: B e C, segundo semestre D e J, etc….
- Usuário inscrito no curso X, irá visualizar as disciplinas: Primeiro semestre: B e E, segundo semestre E e F, etc…

Esta tela será apenas para consulta, não havendo ações e, seu layout, é livre, podendo ser utilizado separadores, cards, tabelas ou quaisquer outros elementos visuais para representar os semestres e disciplinas.

### M2S07 | Ex. 07- Criação da tela inicial

Neste último exercício (dessa semana rs), vamos criar a tela inicial da nossa aplicação.

Nela, serão exibidas as sessões:

- Próximas atividades
  - Sessão onde serão exibidos cards com as próximas atividades a serem realizadas, ex.: Entrega de trabalho da disciplina X, Avaliação da disciplina Y, Chat com o mentor até a data Z, etc…
- Minhas disciplinas
  - Sessão onde serão exibidas as disciplinas do aluno para aquele semestre
- Cursos extras
  - Sessão onde mostrará cursos extras e ou matérias eletivas que o aluno poderá fazer para complementar sua grade curricular

As informações de cada sessão deverão ser apresentadas na forma de cards, porém, seu layout é livre e poderá variar de acordo com a sessão, curso escolhido, matéria apresentada, etc..

# SenaiFullstackEducationM2Semana07

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 18.0.5.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.
