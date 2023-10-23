# Plano de qualidade

## Introdução

A qualidade é uma pedra angular em qualquer projeto de software. Para garantir que o nosso projeto atenda aos mais altos padrões de qualidade, estabelecemos um plano que utiliza tecnologias e práticas eficazes para aprimorar a qualidade do código, a robustez da aplicação e a confiabilidade do software. Neste plano de qualidade, detalharemos como planejamos as métricas e tecnologias de suporte para garantia de qualidade.

## Ferramentas

| Ferramenta  | Descrição                       |
| ----------- | ------------------------------- |
| Sonar Cloud | Ferramenta de análise de código |
| Jest        | Framework de teste JavaScript   |

## Sonnar Cloud

O SonarCloud é uma ferramenta de análise de código estática que fornece insights detalhados sobre a qualidade do código, destacando problemas, vulnerabilidades e áreas de melhoria. Para garantir a qualidade do nosso projeto, planejamos integrar o SonarCloud ao processo de desenvolvimento de software.

### Detalhes do uso do SonarCloud:

- Análise de Código Contínua: A integração contínua com o SonarCloud permite que a cada commit, pull request ou build, que ative o trigger definido no repositório, uma análise de código estática seja executada automaticamente.

- Avaliação de Vulnerabilidades e Bugs: Identifica vulnerabilidades de segurança, bugs e problemas de qualidade no código.

- Acompanhamento de Métricas de Código: Acompanhamento de métricas essenciais, como a cobertura de código, a complexidade e a duplicação de código, para manter o código limpo e eficiente.

- Integração com Fluxo de Trabalho de Desenvolvimento: Integraremos o SonarCloud com nossos fluxos de trabalho de desenvolvimento, permitindo a revisão e correção de problemas de qualidade durante o ciclo de desenvolvimento.

## Jest

O Jest é um framework de teste JavaScript amplamente utilizado para testar aplicações front-end e back-end. Planejamos utilizar o Jest para garantir a funcionalidade correta e a integridade do nosso software.

### Detalhes do uso do Jest:

- Testes Unitários e de Integração: Criaremos testes unitários e de integração utilizando o Jest para avaliar a funcionalidade dos componentes do React no front-end e dos controladores, serviços e módulos no back-end Nest.

- Testes Automatizados: Configuraremos uma suíte de testes automatizados que será executada em um ambiente de integração contínua sempre que houver alterações no código.

- Cobertura de Testes: Monitoraremos a cobertura de testes para garantir que a maioria do código seja testada, identificando áreas não testadas que requerem atenção.

- Testes de Desempenho: Implementaremos testes de desempenho para garantir que o software seja responsivo e eficiente, especialmente em cenários de carga elevada.


## Testes Unitarios

Os testes unitários são realizados para avaliar o comportamento das menores unidades em uma aplicação. Isso implica, tecnicamente, examinar o desempenho de entidades individuais, que podem ser representadas por classes em linguagens orientadas a objetos, ou até mesmo métodos de classe, no contexto de linguagens orientadas a objetos. Em linguagens de programação processuais e funcionais, as menores unidades podem se referir a procedimentos ou funções independentes.

## Testes De Integração

Os testes de integração são uma parte essencial do processo de garantia de qualidade de software. Eles têm como objetivo avaliar como diferentes componentes de um sistema interagem entre si. Em contraste com os testes unitários, que se concentram na avaliação do comportamento de unidades individuais de código, os testes de integração abordam a funcionalidade do sistema como um todo. Eles são projetados para identificar problemas que podem surgir quando módulos ou componentes independentes são combinados e operam juntos. Os testes de integração ajudam a verificar se as partes do sistema se comunicam e colaboram corretamente, garantindo que a aplicação funcione de maneira harmoniosa e cumpra os requisitos de negócios. Eles desempenham um papel fundamental na identificação de possíveis falhas, inconsistências ou incompatibilidades que podem surgir nas interfaces entre os componentes, proporcionando uma visão abrangente da robustez e da integridade do software.

## Testes E2E

Além dos testes unitários e de integração, incorporaremos testes E2E (End to end) em Node.js, os testes E2E s para garantir que todo o fluxo de aplicação, desde a interface do usuário até o banco de dados, funcione de maneira integrada e sem problemas. Usaremos bibliotecas e ferramentas disponíveis junto ao node para realizar testes E2E. O objetivo dessa ferramenta de teste é validar a experiência do usuário final e identificar problemas em cenários do mundo real.

## Referências

> SONNAR CLOUD, <https://www.sonarsource.com/products/sonarcloud/>. Acesso em: 17 de Out. 2023.

> JEST, <https://jestjs.io/pt-BR/> Acesso em: 17 de Out. 2023.
