# Padrão de Criação de Arquivo para Reuniões

Para manter a organização e o registro eficaz das reuniões, adotamos o seguinte padrão de criação de pastas e nomes de arquivos.

## Estrutura de Pastas

Criaremos uma pasta para cada semana, seguindo o formato `Semana_Numero_Semana`, onde o número da semana começa em 1 e aumenta a cada semana subsequente.

Por exemplo:
- `Semana_1`
- `Semana_2`
- `Semana_3`

Dentro de cada pasta da semana, armazenaremos os arquivos de reunião.

## Nomes de Arquivos

Os arquivos de reunião seguirão o formato `reuniao_data_da_reuniao.md`, onde a data será representada pelo dia e mês da reunião, sucessivamente, no formato `DD_MM`.

Por exemplo, para uma reunião realizada em 15 de setembro, o nome do arquivo seria `reuniao_15_09.md`.

## Exemplo de Estrutura de Pastas e Nomes de Arquivos

Suponhamos que estamos na semana 3 e tivemos uma reunião em 15 de setembro. A estrutura de pastas e nomes de arquivos ficaria assim:

- `Semana_1`
- `Semana_2`
- `Semana_3`
  - `reuniao_15_09.md`

Esta padronização ajuda a organizar nossos documentos de reunião de maneira clara e eficiente, tornando mais fácil localizar e referenciar informações específicas de cada encontro.

Lembre-se de seguir este padrão ao criar e armazenar arquivos de reunião para garantir a consistência e acessibilidade das informações.

## Modelo para Conteúdo dos Arquivos de Reunião

Ao escrever o conteúdo dos arquivos das reuniões, siga este modelo:

```markdown

## ATA de Reunião (DD/MM):

## Pauta

| <b>Presentes na Reunião (DD/MM)</b> | <b>Equipe Pertencente</b> | <b>Info</b> |
| --- | --- | --- |
| Duração |  |

```

Como resultado temos:

## ATA de Reunião (04/09):

## Pauta

- Pauta 1
- Pauta 2
- Pauta 3

| <b>Presentes na Reunião (04/09)</b> | <b>Equipe Pertencente</b> | <b>Info</b> |
| --- | --- | --- |
| Membro 1 | EPS | Presente |
| Membro 2 | EPS | Presente |
| Membro 3 | EPS | Ausente |
| Membro 4 | MDS | Presente |
| Membro 5 | MDS | Presente |
| Duração | 00:21:45 |

