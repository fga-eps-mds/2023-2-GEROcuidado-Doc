# Relatório de Encerramento

## Introdução

O presente documento tem como objetivo realizar uma análise comparativa entre o planejado e o efetivamente executado durante o desenvolvimento do projeto. Essa análise sintetiza alguns aspectos essenciais, a saber: backlog, custo, qualidade e riscos. Esse paralelo é fundamental para ilustrar a perspectiva inicial da equipe e o que foi efetivamente concluído ao longo da execução do projeto. Além disso, serve como um guia para futuros mantenedores do projeto, fornecendo insights cruciais sobre o planejamento e execução da solução apresentada.

---

## Backlog

### Planejado

#### MVP

- [[US-01] CRUD de Usuário](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/88)
- [[US-02] CRUD de publicação do fórum](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/111)
- [[US-03] Criação da moderação](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/107)
- [[US-04] CRUD de rotina](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/114)
- [[US-05] CRUD de Idosos](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/112)
- [[US-06] Criação das notificações](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/110)
- [[US-07] Adição da agenda calendário](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/177)
- [[US-08] CRUD de informações de saúde do idoso](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/116)

#### Incremento

- [[US-09] Criação da interação com o fórum](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/109)
- [[US-10] Senha (recuperação e indicadores)](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/113)

### Executadas e Aceitas pelo Cliente

- [[US-01] CRUD de Usuário](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/88)
- [[US-02] CRUD de publicação do fórum](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/111)
- [[US-03] Criação da moderação](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/107)
- [[US-04] CRUD de rotina](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/114)
- [[US-05] CRUD de Idosos](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/112)
- [[US-07] Adição da agenda calendário](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/issues/177)

---

## Custo

---

## Qualidade

Com a finalidade de assegurar a qualidade do produto, em suas diversas nuances, foram tomadas diversas providências, como a validação semanal das entregas junto aos clientes, a validação dos protótipos, implementação de testes e claro os quesitos de qualidade estabelecidos na disciplina e detalhados no [notebook de análise](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/blob/main/Analytics/analytics.ipynb). Foi estabelecido como objetivo pelo time atingir 80% de cobertura de testes em todos os repositórios do projeto, 0 bugs e 0 falhas de segurança.

O time atingiu essa meta, com exceção do repositório de frontend, tal fato se deve à falta de experiência prévia dos membros com testes de frontend e com a tecnologia escolhida para o mesmo, além de algumas falhas ao executar desde a primeira sprint os testes de frontend de maneira correta.

Os demais repositórios atingiram e até superaram a expectativa de testes e qualidade proposta pela equipe.

### Resumo da análise em 10/12/23

| Repositório | Cobertura | Duplicações | Bugs | Code Smells |
|-------------|-----------|-------------|------|-------------|
| Front       | 60.9%     | 15.08%      | 1    | 23          |
| APIForum    | 99.4%     | 0.0%        | 0    | 7           |
| APISaude    | 99.3%     | 0.0%        | 0    | 7           |
| APIUsuario  | 99.2%     | 0.0%        | 0    | 9           |

---

## Risco

### Riscos Planejados

#### Externos 

- Falta de cliente real

- Mudança dos responsáveis pelo projeto

- Indisponibilidade do cliente 

- Projeto cancelado

- Ausência do professor na disciplina por motivos de saúde

#### Organizacional

- Divergência de horários dos membros da equipes

- Desistências da disciplina 

- Dependências de atividades

#### Técnicos 

- Dificuldades com as tecnologias 

- Alterações das tecnologias 

#### Gerencia

- Alterações de escopo

- Presenças dos membros nas reuniões

- Baixa produtividade dos membros 

- Problemas de comunicação 

- Cronograma

### Riscos Enfrentados

- Desistência de um membro da equipe

- Dificuldade da equipe com novas tecnologias, resultando em uma participação mais ativa no frontend

- Divergência de horários, resultando em dificuldades para realizar pareamentos

- Dificuldade na comunicação entre os membros do grupo, resultando na centralização das comunicações em apenas 1 pessoa

---

## Histórico de Versão

| Versão | Data       | Descrição             | Autores         |
| ------ | ---------- | --------------------- | --------------- |
| 1.0    | 10/12/2023 | Abertura do documento | Gustavo Afonso  |