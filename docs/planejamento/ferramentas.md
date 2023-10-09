# Documentação das Ferramentas
Este documento tem como objetivo explicar as tecnologias que serão usadas no projeto GEROcuidado.


## React Native 

 - O React Native é um framework desenvolvido pelo Facebook que utiliza de JavaScript e a biblioteca React para desenvolvimento de aplicativos para IOS e Android. Sendo essa sua principal vantagem, executar o mesmo código em diversas plataformas diferentes. Em vez de renderizar elementos na Web o React utiliza componentes nativos o que resulta em um melhor desempenho. O React Native possui uma grande variadade de componentes em sua biblioteca o que simplifica o desenvolvimento de interfaces complexas.

<div align = "center">
    <img src = "/assets/imagens/React.png" alt = "React Native Logo" width = "100" height = "100" style = "margin: 15">
</div>

### Alguns dos principais components do React Native são:

|Component | Função |
|-----------|--------|  
|`<View>`    | É o Bloco de construção fundamental do React, usado para agrupar componentes e estilizá-los|
|`<Text>`|Usado para exibir texto na interface do usuário|
|`<TextInput>`|Usado para criar campos de entrada de texto|
|`<ScrollView>`|É uma barra de rolagem que pode ser adicionado à uma área que contém outros componentes|
|`<Button>`| Usado para criar botões interativos|
|`<TouchableOpacity>`| Torna qualquer elemento envolto nele clicável|
|`<FlatList>`  `<SectionList>`|Usados para renderizar listas|
|`<WebView>`|Usado para destacar páginas da web dentro do aplicativo|



  - O framework também inclui as chamadas "Hooks" que são funções que permitem adicionar <strong>estado</strong> e outras funcionalidades para componentes tornando o desenvolvimento mais simples e reutilizável.

### Algumas das principais Hooks disponíveis:

|Hook | Função|
|-----|-------|
|`useState`| É uma hook para adicionar estado aos componentes, o que permite reagir a mudanças e atualizar a interface do usuário|
|`useEffect` | Usada para executar efeitos colaterais em componentes, pode ser usado para buscar dados em uma API, por exemplo|
|`useContext`|Permite acessar o contexto de um componente pai, sem a necessidade de passar props para todos os níveis|
|`useRef` |Permite adicionar referência que pode ser usado para acessar o DOM ou outros elementos|
|Custom hooks|É possível criar suas próprias hooks personalizadas para abstrair lógicas em diferentes componentes|


>Documentação Oficial: [https://reactnative.dev/docs/getting-started](https://reactnative.dev/docs/getting-started)

## Expo 

- O expo é uma ferramenta de desenvolvimento de aplicativos usando React Native. Sua principal vantagem é a simplificação no processo de configuração de ambiente. Além disso ele também oferece um conjunto de ferramentas úteis à criação, execução e depuração de aplicativos. O Expo Go é um aplicativo  que permite a visualização em tempo real da aplicação em seu Aparelho pessoal, o que é bem mais fácil para testar o apliactivo durante o desenvolvimento.

<div align = "center">
    <img src = "/assets/imagens/logo-wordmark-light.png" alt = "Expo Logo" width = "150" style = "margin: 15">
</div>

- Para instalar o Expo basta utilizar o gerenciador de pacotes do NodeJs e executar o comando:
  
```bash
npm install expo
```

- E para iniciar um servidor:
  
```bash
npm expo start
```

>Documentação Oficial: [https://docs.expo.dev/more/expo-cli/](https://docs.expo.dev/more/expo-cli/)

## Nest JS

- O NestJS é um framework de desenvolvimento serverside (back-end) baseado em <b>Node.js</b>. O framework utiliza <b>TypeScript</b> (ainda permite que o desenvolvedor programe em JavaScript puro) e combina elementos da OOP (Object Oriented Programming), FP (Functional Programming) e FRP (Functional Reactve Programming). Por baixo dos panos ele também faz uso do <b>Express</b> que é outro framework web. Outra característica interessente que o Nest faz uso são as <b>injeções de dependências</b> para gerenciar a criação e vida de objetos usados no aplicativo.

<div align = "center">
    <img src = "/assets/imagens/nestjs-272666.png" alt = "NestJS Logo" width = "150" style = "margin: 15">
</div>

### Modules
- Uma das principais partes do Nest são os módulos, são usadas para organizar e estruturar a aplicação. Eles ajudam as dividir o código em diferentes partes o que ajuda a escalabilidade do projeto. Módulos possuem algumas propriedades, eles são: provedores, controladores, importadoes e exportadores.

### Middleware

- As Middlewares são funções intermediárias entre o cliente e o servidor. Representam um papel crítico em requisições HTTP, oferecem controle, flexibilidade e reusabilidade, permitindo executar ações antes ou depois de uma requisição.

### Controllers

- Os controladores são responsáveis por lidar com requisições retornar respostas para o cliente. Eles promovem uma organização modular e separação clara de responsabilidades.

### Microserviços

- O NestJS tem suporte nativo para a arquitetura de microserviços.
### Instalação

- Para instalar o Nest JS você pode criar o scaffold do projeto com o Nest CLI ou clonar um projeto inicial (ambos produzirão o mesmo resultado).
- Sendo assim, para estruturar o projeto com o Nest CLI digite os seguintes comandos. Isso criará um novo diretório de projeto e prencherá com os arquivos Nest JS principais iniciais:

```bash
$ npm i -g @nestjs/cli
$ nest new project-name
```
- Alternativamente, para instalar o projeto inicial TypeScript com Git :

```bash
$ git clone https://github.com/nestjs/typescript-starter.git project
$ cd project
$ npm install
$ npm run start
```
- Para instalar a versão JavaScript do projeto inicial, use na sequência dos comandos acima : 

```bash
javascript-starter.git
```

>Documentação Oficial: [https://docs.nestjs.com/](https://docs.nestjs.com/)

## Docker
 * Docker é uma plataforma aberta para desenvolvimento, envio e execução de aplicativos. A plataforma oferece a capacidade de empacotar, distribuir e executar aplicativos, de forma consistente, em um ambiente isolado chamado ***container***, que contêm tudo o que é necessário para executar o aplicativo.  
* Além disso, é possível compartilhar *containers* e garantir que todas as pessoas com quem você compartilha recebam o mesmo *container* que funciona da mesma maneira. Assim, o Docker evita inconsistências de ambiente, permite o desenvolvimento de um ambiente padronizado e facilita a colaboração.
* Dessa forma, o Docker é uma ferramenta fundamental para melhorar a eficiência no desenvolvimento e na implantação de software.

<div align = "center">
    <img src = "/assets/imagens/Docker_logo-700x588.png" alt = "Docker Logo" width = "150" style = "margin: 15">
</div>

### *Containers*
* Um *container* é uma instância executável de uma **imagem**. É uma unidade de software que empacota uma aplicação e todas as suas dependências, incluindo bibliotecas, configurações e arquivos, em um único pacote executável. Esses containers são projetados para serem portáteis e consistentes, permitindo que uma aplicação seja executada de forma confiável e isolada em qualquer ambiente que suporte a tecnologia de containers.
### Imagens
* As imagens Docker são usadas como base para criar instâncias de containers em tempo de execução. Elas são uma parte fundamental da tecnologia de containerização e contêm todas as informações necessárias para criar um container, como códigos, dependências, bibliotecas, variáveis ​​de ambiente e configurações. Por isso, desempenham um papel crucial na portabilidade e na consistência dos containers.
* Outro ponto importante é sobre a possibilidade de versionamento das imagens Docker, o que permite rastrear e controlar as diferentes versões de um aplicativo.

### Vantagens do Docker
* O Docker utiliza containers para isolar aplicativos e suas dependências. Isso garante que cada aplicativo seja executado de forma independente, evitando conflitos de versões e problemas de compatibilidade.
* Os containers Docker são leves e empacotam todos os componentes necessários para a execução de um aplicativo, tornando-o portátil.
* O Docker agiliza o ciclo de vida de desenvolvimento, permitindo que os desenvolvedores trabalhem em ambientes padronizados.
* Os containers Docker podem ser implantados rapidamente, reduzindo o tempo necessário para provisionar e escalar aplicativos. Isso é especialmente útil em ambientes de desenvolvimento ágil e DevOps.
* As imagens Docker podem ser versionadas, o que permite o controle preciso das versões de aplicativos e a reversão para versões anteriores, se necessário.

### Instalação
- Para instalar o Docker no <b>Linux</b>, acesse: 
> [https://docs.docker.com/desktop/install/linux-install/](https://docs.docker.com/desktop/install/linux-install/)

- Para instalar o Docker no <b>Windows</b>, acesse:
>[https://docs.docker.com/desktop/install/windows-install/](https://docs.docker.com/desktop/install/windows-install/)

- Para instalar o Docker no <b>MacOS</b>, acesse:
>[https://docs.docker.com/desktop/install/mac-install/](https://docs.docker.com/desktop/install/mac-install/)

- Para mais informações consulte:
>Documentação Oficial: [https://docs.docker.com/](https://docs.docker.com/)


## PostgreSQL
- PostgreSQL é um sistema de gerenciamento de banco de dados objeto-relacional (ORDBMS) baseado em POSTGRES, desenvolvido no Departamento de Ciência da Computação da Universidade da Califórnia em Berkeley.

- PostgreSQL é um descendente de código aberto deste código original de Berkeley. Suporta grande parte do Padrão SQL e oferece muitos recursos modernos:
    - consultas complexas
    - chaves estrangeiras
    - gatilhos
    - visualizações atualizáveis
    - integridade transacional
    - controle de simultaneidade multiversão
    - Item de lista principal

<div align="center">
<img src="/assets/imagens/postgresql-512.png" alt="PostgreSQL Logo" width="150">
</div>

- Além disso, o PostgreSQL pode ser estendido pelo usuário de várias maneiras, por exemplo, adicionando novos
    - tipos de dados
    - funções
    - operadores
    - funções agregadas

### Instalação
- A maioria das distribuições <b>Linux</b> incluem o PostgreSQL por padrão, sendo assim para instalá-lo basta digitar o seguinte comando: 

```bash
apt-get install postgresql-12
```
- Para o sistema <b>MacOS </b>existem diversas maneiras de instalar, consulte o link abaixo:
>[https://www.postgresql.org/download/macosx/](https://www.postgresql.org/download/macosx/)

- Para o <b>Windows</b> basta acessar o link abaixo. Tendo selecioando a versão desejada do postgreSQL será baixado o instalador e basta configurar da maneira como desejar
>[https://www.enterprisedb.com/downloads/postgres-postgresql-downloads](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads)

- Para mais informações de como instalar o postgreSQL acesse o seguinte link :
>h[ttps://www.postgresql.org/download/](ttps://www.postgresql.org/download/)

### Fundamentos da Arquitetura
- PostgreSQL usa um modelo cliente/servidor. Uma sessão PostgreSQL consiste nos seguintes processos (programas):
    - Um processo de servidor, que gerencia os arquivos do banco de dados, aceita conexões do Banco de Dados com os formulários do CLientes e executa ações de banco de dados em nome dos clientes. O programa servidor de banco de dados é chamado postgres.

    - A aplicação cliente(frontend) do usuário que deseja realizar operações de banco de dados.

- Como é comum em aplicações cliente/servidor, o cliente e o servidor podem estar em hosts diferentes. Nesse caso, eles se comunicam por meio de uma conexão de rede TCP/IP. É importante lembrar disso, pois os arquivos que podem ser acessados em uma máquina cliente podem não ser acessíveis (ou podem ser acessíveis apenas com um nome de arquivo diferente) na máquina do servidor de banco de dados.

- O servidor PostgreSQL pode lidar com várias conexões simultâneas de clientes. Para fazer isso, ele inicia ("cria cópias") um novo processo para cada conexão. A partir desse momento, o cliente e o novo processo do servidor se comunicam sem intervenção do processo original do PostgreSQL. Portanto, o processo de supervisão do servidor está sempre em execução, aguardando conexões de clientes, enquanto os processos do cliente e os processos de servidor associados vêm e vão. 

 - Para mais informações gerais sobre o postgreSQL acesse o seguinte link :
> Documentação Oficial: [https://www.postgresql.org/docs/](https://www.postgresql.org/docs/)

# Histórico de versões


| Versão | Data       | Descrição | Autores |
| ------ | ---------- | --------- | ------- |
| 1.0    | 09/10/2023 | Documentação React Native, Expo, NestJS, Docker e PostgreSQL | Guilherme Dutra<br>Guilherme Westphall<br>Lucas Martins Gabriel|