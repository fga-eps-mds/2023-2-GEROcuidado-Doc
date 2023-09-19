# Guia de Git para Iniciantes

## Introdução ao Git e Plataformas de Hospedagem

### O que é o Git?

- Git é um sistema de controle de versão amplamente utilizado para rastrear alterações em projetos de software. Ele permite que você acompanhe o histórico de alterações, colabore com outros desenvolvedores e reverta para versões anteriores do seu código.

### Git e Plataformas de Hospedagem

É importante observar que o Git, por si só, é um sistema de controle de versão distribuído e local. No entanto, você pode aproveitar ao máximo suas capacidades colaborativas usando plataformas de hospedagem como o GitHub e o GitLab. Essas plataformas oferecem recursos adicionais para gerenciamento de repositórios, rastreamento de problemas, colaboração em equipe e integração contínua.

- **GitHub:** É uma das plataformas de hospedagem mais populares para projetos Git. Ele oferece uma interface amigável e é amplamente utilizado para projetos de código aberto e privados. O GitHub também fornece ferramentas de gerenciamento de problemas (issues) e integração contínua.

- **GitLab:** Semelhante ao GitHub, o GitLab é uma plataforma que oferece hospedagem de repositórios Git. Uma diferença notável é que o GitLab é mais flexível em termos de implantação, permitindo que você hospede sua própria instância em servidores internos ou na nuvem. Isso o torna uma opção atraente para empresas que precisam de controle sobre a infraestrutura.


Independentemente da plataforma de hospedagem que você escolher, os comandos e conceitos do Git discutidos neste guia podem ser aplicados a qualquer repositório Git. O uso de uma plataforma de hospedagem facilita a colaboração, o acompanhamento de problemas e a automação de processos, tornando-o essencial para projetos de desenvolvimento de software em equipe.

## Configuração Inicial

- Antes de começar a usar o Git, configure seu nome de usuário e endereço de email:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

## Criando um Repositório

### Inicializando um Repositório Local

1. Navegue até a pasta do seu projeto:

```bash
cd /caminho/para/seu/projeto
```

2. Inicialize um repositório Git:

```bash
git init
```

### Clonando um Repositório Remoto

- Se você estiver trabalhando em um projeto existente:
```bash
git clone URL_DO_REPOSITÓRIO
```

## Trabalhando com Arquivos

### Adicionando Arquivos ao Stage

- Antes de fazer commit das alterações, você precisa adicionar os arquivos ao stage:

```bash
git add nome-do-arquivo
```

- Para adicionar todos os arquivos alterados ou novos:

```bash
git add .
```

## Branches

### Listando Branches

- Para listar todas as branches no seu repositório e visualizar qual é a atual:

```bash
git branch
```

### Criando uma Nova Branch

- Para criar uma nova branch a partir da branch atual e mudar para ela:

```bash
git checkout -b nome-da-branch
```

- Isso é equivalente a executar os comandos em duas etapas separadas:

```bash
git branch nome-da-branch
git checkout nome-da-branch
```

### Mudando de Branch

- Para mudar de uma branch para outra:

```bash
git checkout nome-da-branch
```

### Fazendo Merge entre Branches

- Para fazer merge de uma branch de volta à branch principal:

```bash
git checkout branch-destino
git merge nome-da-branch
```

### Resolvendo Conflitos de Merge

- Em caso de conflitos durante o merge, edite os arquivos conflitantes e depois faça commit:

```bash
git status  # Verifique os arquivos com conflitos
# Edite os arquivos com conflitos
git add nome-do-arquivo
git commit -m "Resolver conflitos"
```

## Trabalhando com Repositórios Remotos

### Adicionando um Repositório Remoto

- Para adicionar um repositório remoto:

```bash
git remote add origin URL_DO_REPOSITÓRIO
```

### Enviando Alterações para o Repositório Remoto

- Para enviar suas alterações para o repositório remoto:

```bash
git push origin nome-da-branch
```

### Atualizando o Repositório Local

- Para atualizar seu repositório local com as alterações do repositório remoto:

```bash
git pull origin nome-da-branch
```

## Pull Requests

- Pull Requests (PRs) são uma parte fundamental do fluxo de trabalho colaborativo no Git, especialmente ao trabalhar com plataformas de hospedagem de código como o GitHub. Eles permitem que você proponha suas alterações para um repositório e solicite que os mantenedores revisem e incorporem suas contribuições.

### Criando um Pull Request

1. Primeiro, certifique-se de que você tenha uma branch onde fez suas alterações. Se você não tiver, crie uma nova branch para suas alterações usando o comando:

```bash
git checkout -b nome-da-sua-branch
```

2. Faça commit das suas alterações na sua branch.

3. Navegue até a página do repositório no GitHub onde deseja criar o Pull Request.

4. Clique no botão "New Pull Request" (GitHub)

5. Selecione a branch de onde suas alterações estão vindo (geralmente sua branch) e a branch de destino (geralmente a main).

6. Dê um título e uma descrição descritiva para o seu Pull Request. Explique o que suas alterações fazem e por que são necessárias (Utilizar template).

7. Clique em "Create Pull Request" (GitHub)

### Revisando e Comentando

- Os revisores (ou mantenedores do projeto) podem revisar suas alterações diretamente no Pull Request. Eles podem deixar comentários, sugerir alterações e discutir as alterações propostas com você.

### Atualizando o Pull Request

- Se os revisores solicitarem alterações ou se você precisar atualizar suas alterações, siga estas etapas:

- Faça as alterações necessárias nos seus arquivos locais e faça um novo commit.

- As alterações serão automaticamente adicionadas ao Pull Request existente.

### Mergeando um Pull Request

- Uma vez que seus Pull Requests tenham sido revisados e aprovados, eles podem ser mergeados na branch de destino.

- Clique no botão "Merge" (GitHub).

- Suas alterações serão mergeadas na branch de destino.

### Fechando um Pull Request

- Após um merge bem-sucedido do Pull Request, ele pode ser fechado.

- Clique no botão "Close" (GitHub) no seu Pull Request para marcá-lo como concluído.

- Os Pull Requests são uma maneira eficaz de colaborar em projetos Git e garantir que as alterações sejam revisadas e testadas antes de serem incorporadas ao código principal.

## Git Stash

- O comando `git stash` é uma ferramenta útil para salvar temporariamente as alterações não confirmadas em seu diretório de trabalho, permitindo que você limpe o seu ambiente de trabalho atual e volte a ele mais tarde. Isso é especialmente útil quando você está no meio de uma tarefa, mas precisa mudar de branch ou lidar com outra emergência.

### Salvando Alterações com Git Stash

- Para salvar as alterações não confirmadas em um stash, use o seguinte comando:

```bash
git stash save "Mensagem do Stash"
```

- Isso criará um stash com um nome descritivo para que você possa identificar facilmente suas alterações mais tarde.

### Listando Stashes

- Você pode listar todos os stashes disponíveis no repositório usando o comando:

```bash
git stash list
```

### Aplicando Alterações do Stash

- Para aplicar as alterações de um stash de volta ao seu diretório de trabalho, use o seguinte comando:

```bash
git stash apply stash@{n}
```

### Removendo Stashes

- Para remover um stash após aplicar suas alterações, use o seguinte comando:

```bash
git stash drop stash@{n}
```

- Para remover todos os stashes de uma vez:

```bash
git stash clear
```

- O comando git stash é uma ferramenta útil para gerenciar suas alterações temporárias e pode ser especialmente valioso quando você precisa alternar rapidamente entre tarefas ou lidar com problemas inesperados.

## Rebase

### Realizando um Rebase

- O rebase é uma operação que reescreve o histórico do seu projeto. Ele permite que você pegue todas as alterações de uma branch e aplique-as como se fossem feitas diretamente na branch em que você está. Isso pode criar um histórico mais linear e limpo.

- Para fazer um rebase de uma branch sobre a outra:

```bash
git checkout nome-da-branch
git rebase branch-destino
```

### Resolvendo Conflitos de Rebase

- Assim como no merge, durante o rebase, podem ocorrer conflitos. Resolva-os da mesma maneira:

```bash
git status  # Verifique os arquivos com conflitos
# Edite os arquivos com conflitos
git add nome-do-arquivo
git rebase --continue
```

### Usando o Rebase com Cuidado

- O rebase é uma ferramenta poderosa, mas deve ser usado com cuidado, especialmente em branches compartilhadas. Reescrever o histórico pode causar problemas para outros colaboradores. Portanto, é recomendável usá-lo principalmente em suas branches pessoais.

## Link repositório treinamento

https://github.com/HenriqueAmorim20/2023-2-GEROcuidado-treinamento-git.git

## Link plano de contribuição

https://github.com/fga-eps-mds/2023-2-GEROcuidado-Doc/blob/main/docs/planejamento/plano_de_contribuicao.md

## Link gravação

https://drive.google.com/file/d/10-qd7qyaap0q5aRotCIWm-ssIk4AG288/view?usp=sharing