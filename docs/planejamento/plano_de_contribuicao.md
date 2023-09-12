# Contribuições

## Introdução
Este documento determina as regras para submissão de códigos para este repositório.

## Issues

Toda e qualquer contribuição deve estar vinculada a uma e tão somente uma issue. Toda issue deve ser preenchida obrigatoriamente conforme o [template _feature_](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/blob/main/.github/ISSUE_TEMPLATE/template-das-issues.md) ou [_bug_](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/blob/main/.github/ISSUE_TEMPLATE/template-de-bug-report.md) e deve representar uma contribuição clara, objetiva e independente de outras issues, dentro do possível.

Se uma issue _feature_ precisar de mais de um pull request ou se o prazo de conclusão for maior que uma sprint, essa issue deve ser quebrada em issues menores. As issues possuirão dois perfis de responsáveis:

1. Assignees: pessoa(s) responsáveis por desenvolver a issue, seja de código, seja de design, seja de documentação. Em caso de código, o pull request será vinculado. Em caso de outros tipos de artefato, eles devem ser linkados ou anexados na issue como prova de conclusão.
2. Reviewers: pessoa(s) responsáveis por verificar a conclusão da issue. Em caso de código, eles devem executar a funcionalidade ou correção de bug para verificar a conclusão.

---

## Pull Requests

Os pull requests devem estar obrigatoriamente vinculados a uma issue, e os passos obrigatórios presentes no [template](https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/blob/main/.github/template-dos-pull-requests.md).

---

## Commits

Por questões de padronização e rastreabilidade, os commits devem seguir as seguintes regras:

- Deve começar indicando a issue com uma "#"
- Utilize a língua portuguesa na mensagem do commit
- Deve conter um título curto e objetivo do que foi feito naquele _commit_
- Deve começar com um verbo no presente do indicativo (corrige, adiciona, retira, melhora, etc.)
- Caso o commit seja resultado de um trabalho em equipe, utilize *Co-authored-by:*

__Exemplo Trabalhando Sozinho:__
    
    $ (#43) Corrige erro na autenticação do perfil x de usuário


__Exemplo Trabalhando em grupo:__
    
    (#43) Corrige erro na autenticação do perfil x de usuário


    Co-authored-by: Outra Pessoa <pessoa@email.com>

---

# Branches

Tendo como meta manter a integralidade e confiabilidade do código do projeto foi proposta a utilização de política de branches. Essa Política de Branches deverá guiar os desenvolvedores na forma de organização de suas contribuições ao repositório.

__OBS__: A política de _branchs_ foi idealizada para trabalhar em conjunto com a ferramenta do _git flow_, sua documentação e mais informações podem ser acessadas [aqui](https://github.com/nvie/gitflow).

### Branches Principais

* __main__ - Branch principal do repositório onde será permitida somente a integração de software consolidado e testado. Essa branch será exclusiva para a entrega de Realeases, ou seja, um conjunto maior de funcionalidades que integram o software, aqui estará a versão _**estável**_ do software.

* __develop__ - Branch para integração de novas funcionalidades, onde será permitido a entrega das features desenvolvidas e que estão em um estágio avançado de desenvolvimento. Será a branch base para o início do desenvolvimento das features e da correção de bugs. Aqui também serão mergeadas as releases.

### Branches para Desenvolvimento

* __feature/<nome-da-feature>__ - Branch utilizada para o desenvolvimento de novas features do _backlog_. Caso a feature tenha sido proposta por uma _issue_ do repositório e aceita no _backlog_ o nome deverá conter o número da _issue_. **Ex**: feature/1-\<nome-da-nova-feature> (Considerando que a feature tenha sido solicitada na _issue_ #1)

* __bugfix/<nome-do-bug>__ - Branch utilizada para corrigir bugs de **baixa/média urgência** e que não estão presentes na branch __master__. Caso o bug tenha sido reportado por uma _issue_ do repositório o nome deverá conter o número da _issue_. **Ex**: bugfix/1-\<descrição-do-bug> (Considerando que o bug tenha sido reportado na _issue_ #1)

* __hotfix/<nome-do-bug>__ - Branch utilizada para corrigir bugs de **alta urgência** e que estão presentes na branch __master__. Caso o bug tenha sido reportado por uma _issue_ do repositório o nome deverá conter o número da _issue_. **Ex**: hotfix/1-<descrição-do-bug> (Considerando que o bug tenha sido reportado na _issue_ #1)

* __release/<versão-da-release>__ - Branch onde será feito os ajustes finais/build antes da entrega de uma versão do produto de software. Constará no nome da branch a versão da release a ser entregue.

* __doc/<tema-ou-natureza>__ - Branch onde serão executadas tarefas de suporte relacionadas ao software, como elaboração de documentações, correções de natureza de gerência de configuração, etc.


| Versão | Data       | Descrição | Autores |
| ------ | ---------- | --------- | ------- |
| 1.0    | 06/09/2023 | Abertura do documento | Pedro Cella |

---