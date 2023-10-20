# <strong> Documento de Banco de Dados </strong>

## <strong> 1. Introdução </strong>
<p>
Este documento tem por objetivo reunir os principais documentos produzidos referentes ao banco de dados da aplicação. O intuito disso é proporcionar transparência e organização quanto ao que acreditamos ser a maneira mais adequada de contextualizar, diagramar e modelar os dados associados à problemática na qual o projeto GEROcuidado, bem como o produto de software a ele vinculado, está inserido.
</p>

## <strong> 2. Documentos criados </strong>

### <strong> 2.1 MER </strong>
<P> O Modelo Entidade-Relacionamento (MER) é uma abordagem conceitual usada no projeto de banco de dados para representar entidades, seus atributos e relacionamentos. Isso permite visualizar como os dados estão organizados e como as entidades se relacionam no sistema de informações. O MER é a base conceitual sobre a qual os Diagramas Entidade-Relacionamento (DER) são criados para representar graficamente essa estrutura.</P>

**<strong> 2.1.1 Entidades </strong>**

![MER_ENTIDADES](/docs/assets/imagens/banco_de_dados/MER/MER_ENTIDADES.png)

**<strong> 2.1.2 Descrição das Entidades </strong>**

![MER_DESCRICAO_ENTIDADE](/docs/assets/imagens/banco_de_dados/MER/DESCRICAO_ENTIDADE.png)

**<strong> 2.1.3 Relacionamentos </strong>**

![RELACIONAMENTOS 1](/docs/assets/imagens/banco_de_dados/MER/RELACIONAMENTOS1.png)
![RELACIONAMENTOS 2](/docs/assets/imagens/banco_de_dados/MER/RELACIONAMENTOS2.png)

### <strong> 2.2 DER </strong>

<p>O Diagrama Entidade-Relacionamento (DER) é uma representação gráfica amplamente utilizada no projeto de bancos de dados. Ele descreve as entidades (objetos), seus atributos (características) e os relacionamentos entre as entidades. Os retângulos representam as entidades, as elipses indicam os atributos e as linhas conectam as entidades para mostrar como elas se relacionam. O DER é uma ferramenta fundamental para visualizar e planejar a estrutura de um banco de dados antes da implementação, ajudando a definir como os dados são armazenados e acessados </p>

![DER](/docs/assets/imagens/banco_de_dados/DER.png)

### <strong> 2.3 DLD </strong>

<p> 
O Diagrama Lógico de Dados (DLD) é uma representação gráfica que ilustra a estrutura lógica de um banco de dados. Nesse diagrama, são exibidas informações cruciais, como os tipos de atributos associados a cada entidade, bem como as chaves estrangeiras e restrições, como a chave única (unique key). Seu propósito fundamental é fornecer uma representação estruturada e específica da maneira como o banco de dados deve ser implementado. Em resumo, o DLD funciona como uma representação visual que orienta a implementação efetiva do banco de dados.</p>

![DLD](/docs/assets/imagens/banco_de_dados/DLD.png)

### <strong> 2.4 Dicionário de Dados </strong>

<p>
Um Dicionário de Dados é uma referência essencial em gerenciamento de dados. Ele é um documento ou repositório que descreve detalhadamente os elementos de um banco de dados, como tabelas, campos, relacionamentos e regras de negócios associadas. O Dicionário de Dados serve como uma fonte confiável de informações para desenvolvedores, analistas e outros stakeholders, garantindo a compreensão e a consistência dos dados dentro de um sistema. Ele fornece informações cruciais sobre a estrutura e a semântica dos dados, auxiliando na manutenção, integração e uso eficaz das informações em um contexto organizacional.
</p>

### <strong> 2.4.1 Entidades </strong>
### Usuário
![USUARIO](/docs/assets/imagens/banco_de_dados/dicionario_de_dados/USUARIO.png)

### Paciente
![Paciente](/docs/assets/imagens/banco_de_dados/dicionario_de_dados/PACIENTE.png)

### Métricas de saúde
![METRICA](/docs/assets/imagens/banco_de_dados/dicionario_de_dados/METRICA_SAUDE.png)

### Valor das métricas de saúde
![VALOR_METRICA](/docs/assets/imagens/banco_de_dados/dicionario_de_dados/VALOR_METRICA.png)

### Rotina
![ROTINA](/docs/assets/imagens/banco_de_dados/dicionario_de_dados/ROTINA.png)

### Publicação
![PUBLICACAO](/docs/assets/imagens/banco_de_dados/dicionario_de_dados/PUBLICACAO.png)

### Like ![LIKE](/docs/assets/imagens/banco_de_dados/dicionario_de_dados/LIKE.png)

### Comentário ![COMENTARIO](/docs/assets/imagens/banco_de_dados/dicionario_de_dados/COMENTARIO.png)


**<strong> 2.4.2 Relacionamentos </strong>**
### Publicação tem comentário
![PUB_TEM_COMENTARIO](/docs/assets/imagens/banco_de_dados/dicionario_de_dados/RELACIONAMENTO_COMENTARIO.png)

### Publicação tem like
![PUB_TEM_LIKE](/docs/assets/imagens/banco_de_dados/dicionario_de_dados/RELACIONAMENTO_LIKE.png)

### <strong> 2.5 Link </strong>

O link contendo todos os documentos apresentados pode ser encontrado [aqui](https://docs.google.com/document/d/1Xqe3WFQjvw8OYEYdntZAu6HedWevR1Rj66IXbBPaCsA/edit).
