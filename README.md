# Pipeline Github Compartilhados

__[descrição do repositório: ]__ Repositório que compartilha fluxos de trabalho do github com os demais repositórios/projetos.

## Identificadores da Aplicação

| Sigla | Descrição do Projeto | Nome Aplicativo |
| --- | --- | --- |
| PGC | Pipeline Github Compartilhados | bzn-pgc-infra |

## Versões

__[relação das versões de aplicativos externos: ]__ A aplicação utiliza as seguintes versões: *NÃO SE APLICA.*

## Estrutura do projeto

__[descrição da estrutura do diretório: ]__

``` text

├── .github
│   └── workflows
│       └── script
│           └── manifest.sh
│       └── identifier.yml
│       └── pipeline-deploy.yml
│       └── tag.yml
├── docs
│   └── CONTRIBUTING.md
│   └── CODE_OF_CONDUCT.md
│   └── PULL_REQUEST_TEMPLATE.md
│   └── SECURITY.md
└── README.md
```

### Tabela Branch x Ambiente

| Branch | Evento | Ambiente |
| --- | --- | --- |
| develop | Pull Request | Aplica no ambiente __DSV__ |
| release/** | Pull Request | Aplica no ambiente __HMG__ |
| pre-release/** | Pull Request | Aplica no ambiente __STG__ |
| main | Pull | Aplica no ambiente __PRD__ |

## Funções dos Pipelines

Cada um dos pipelines compartilhados tem uma finalidade em comum com os outros, abaixo uma breve descrição de cada um deles.

### Pipeline Identifier

Esse fluxo tem como objetivo identificar qual ambiente alvo.

### Pipeline Deploy

Esse pipeline executa um deploy de aplicação.

### Pipeline Tag

Esse gera um identificador de imagem docker.

## Licença

> [!IMPORTANT]
> *O código fonte neste projeto não possui licença de uso.*

É terminantemente proibido reproduzir, distribuir, alterar, utilizar engenharia reversa ou valer-se de qualquer tentativa de reverter ao seu código-fonte qualquer dos componentes que compõem o SOFTWARE, bem como utilizar subterfúgios para burlar a quantidade de usuários licenciados.
