# Documento de Arquitetura

## Introdução

Esse documento tem a finalidade de explicar sobre as decisões arquiteturais do projeto, nesse documento o foco será entender mais sobre como funcionará o sistema como um todo, ou seja, como é feita a interação do usuário com o produto, quais são os microsserviços e de que forma eles foram definidos, entre outras possíveis dúvidas que possam surgir.

## Escopo

O GEROcuidado é um aplicativo projetado para auxiliar seus usuários, que incluem cuidadores formais e informais, idosos autônomos e familiares, na organização e acompanhamento da saúde dos idosos, seja como parte de suas responsabilidades de cuidador ou de sua própria família, como um pai ou uma mãe. No caso dos idosos autônomos, esse acompanhamento é realizado de si mesmo.

Nesse semestre a proposta do MVP focou nas funcionalidades de crud de usuário, crud de publicação, perfil de moderação nas publicações, crud de rotina, crud de idosos, cadastrar notificações, linkar notificações a uma agenda/calendário, crud das informações de saúde do idoso (métricas de saúde), como incremento teremos a interação com a publicação, através de likes e comentários, e foco na política de senhas e na capacidade de recuperar senha. Logo a arquitetura assim implementada, tem como intuito abarcar todas essas funcionalidades.

## Arquitetura

A arquitetura abaixo ilustra a forma como irá funcionar todas as partes, sendo elas o Frontend, onde ocorre o input através da interface de usuário, após esse input é encaminhado para o microsserviço especificado, sendo eles o Microsserviço Usuário atrelado as funcionalidades de CRUD quanto aos usuários e perfis de usuário, Microsserviço Fórum associado a parte do fórum, publicações, like e comentário e finalmente o  Microsserviço Saúde, responsável pelas informações de saúde do idoso, como pressão, oxigenação do sangue, entre outros. Além disso temos os bancos de cada microsserviços, responsável por armazenar todas essas informações. Abaixo a arquitetura ilustrando todos esses pedaços:

![Arquitetura](../assets/imagens/Arquitetura.png)

## Frontend

## Microsserviço Usuário

O microsserviço de Usuário no aplicativo GEROcuidado desempenha um papel fundamental na gestão e autenticação de usuários, que podem ser cuidadores formais, cuidadores informais, idosos autônomos ou familiares de idosos. Este microsserviço é projetado para fornecer funcionalidades relacionadas à gestão de contas e acesso de usuários ao sistema. As principais funcionalidades desse microsserviço incluem:

1. **CRUD de Usuário (Create, Read, Update, Delete):** Os usuários podem se cadastrar no sistema, fornecendo informações pessoais, como nome, endereço de e-mail, senha segura e outros dados relevantes. Além disso, eles podem atualizar ou excluir suas informações de perfil conforme necessário.

2. **CRUD de Idosos:** Os cuidadores formais, cuidadores informais e familiares têm a capacidade de gerenciar o cadastro de idosos no sistema. Isso inclui adicionar informações detalhadas sobre os idosos, como nome, idade, condições de saúde, preferências e outras informações essenciais para o acompanhamento de sua saúde e bem-estar. 

Além disso, o microsserviço de Usuário desempenha um papel importante na autenticação dos usuários e na gestão de permissões de acesso, garantindo que apenas os usuários autorizados tenham acesso às funcionalidades específicas do aplicativo.

Em resumo, o microsserviço de Usuário é essencial para a identificação, autenticação e gestão das informações dos usuários do aplicativo GEROcuidado, garantindo que os cuidadores formais, cuidadores informais e familiares possam acessar e gerenciar informações relacionadas aos idosos de forma segura e eficaz.

## Microsserviço Fórum 

O microsserviço de Fórum no aplicativo GEROcuidado desempenha um papel crucial na interação e comunicação entre os usuários, que incluem cuidadores formais, cuidadores informais, idosos autônomos e familiares. Este microsserviço é projetado para fornecer funcionalidades relacionadas ao compartilhamento de informações, discussões e interações no fórum do aplicativo. Suas principais funcionalidades incluem:

1. **CRUD de Publicação no Fórum:** Os usuários, que podem ser cuidadores formais, cuidadores informais, idosos autônomos ou familiares, têm a capacidade de criar, ler, atualizar e excluir (CRUD) publicações no fórum. Isso permite que os usuários compartilhem informações, façam perguntas, forneçam dicas ou discutam tópicos relacionados ao cuidado de idosos.

2. **Moderação de Publicações:** O microsserviço de Fórum também inclui funcionalidades de moderação. Os moderadores, designados para garantir a qualidade e o respeito no fórum, têm a capacidade de revisar e moderar as publicações. Isso inclui a capacidade de aprovar, editar ou excluir publicações para evitar informações imprecisas ou conteúdo inadequado.

3. **Interação com Publicações:** Além das funcionalidades CRUD, os usuários têm a capacidade de interagir com as publicações no fórum. Eles podem "curtir" publicações (likes) e deixar comentários para criar discussões e promover a interação entre os membros da comunidade.

Este microsserviço também pode incluir recursos de notificação para alertar os usuários sobre novas publicações, respostas a comentários e moderações de publicações. *(Rever este parágrafo)*

Através do microsserviço de Fórum, o aplicativo GEROcuidado promove uma comunidade de usuários onde cuidadores formais, cuidadores informais, idosos autônomos e familiares podem trocar informações, apoio e experiências, promovendo um ambiente de aprendizado e colaboração. O foco na moderação garante que o fórum permaneça informativo e respeitoso.

## Microsserviço Saúde

O microsserviço de Saúde no aplicativo GEROcuidado tem como foco principal o acompanhamento e gerenciamento das informações de saúde relacionadas aos idosos e aos usuários, incluindo cuidadores formais, cuidadores informais e familiares. Este microsserviço engloba várias funcionalidades para garantir um acompanhamento eficaz e organizado da saúde dos idosos, bem como a gestão das rotinas diárias. Suas principais funcionalidades incluem:

**1. CRUD de Informações de Saúde do Idoso:**
- Cuidadores formais, cuidadores informais e familiares podem registrar, atualizar, visualizar e apagar informações de saúde dos idosos ou de si mesmos. Isso inclui métricas de saúde como frequência cardíaca, oxigenação do sangue e outras informações relevantes. Os usuários podem criar métricas de saúde, especificando a categoria e o valor máximo (opcional), além de atualizá-las através de novos cadastros.

**2. CRUD de Rotina:**
- Este microsserviço também abrange a gestão da rotina dos idosos. Os cuidadores, tanto formais como informais, têm a capacidade de cadastrar, visualizar, editar e remover informações sobre a rotina dos idosos. Isso inclui horários para medicamentos, atividades físicas e alimentação, permitindo que os cuidadores acompanhem e garantam o cumprimento das necessidades específicas de cada idoso.

- Além disso, os idosos autônomos também podem utilizar essa funcionalidade para cadastrar, visualizar, editar e remover informações sobre sua própria rotina, proporcionando um lembrete dos horários das atividades.

**3. Criação de Notificações:**
- Os usuários têm a capacidade de receber notificações do aplicativo para lembrá-los de realizar as atividades cadastradas, como tomar medicamentos ou realizar exercícios. Isso ajuda a manter a disciplina e garantir que as tarefas de saúde sejam cumpridas de maneira adequada.

**4. Adição de Agenda/Calendário:**
- Os cuidadores podem criar agendas e calendários para agendar tarefas específicas relacionadas à saúde e rotina dos idosos. Esses agendamentos ajudam os cuidadores a serem notificados das atividades planejadas, garantindo que nada seja esquecido.

O microsserviço de Saúde é essencial para a promoção de um cuidado eficaz e organizado da saúde dos idosos, permitindo que cuidadores e idosos autônomos acompanhem e gerenciem informações de saúde, bem como suas rotinas diárias. A adição de notificações e calendários torna mais fácil para os usuários lembrarem-se de suas tarefas e manterem o controle de suas atividades diárias.

## Documentos complementares

Como o foco desse documento é a arquitetura em si, foram criados outros dois documentos que tem como objetivo explicar mais profundamente sobre as ferramentas utilizadas e uma explicação no funcionamento do banco de dados, ambos os documentos podem ser acessados pelos seguintes links:

- [Documento de ferramentas](ferramentas.md)

- [Documento do banco de dados]()

## Histórico de versão

| Versão | Data       | Descrição | Autores |
| ------ | ---------- | --------- | ------- |
| 1.0    | 15/10/2023 | Abertura do documento | Pedro Cella|