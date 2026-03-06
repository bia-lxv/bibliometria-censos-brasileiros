# Análise bibliométrica sobre o uso dos Censos brasileiros no século XXI

## Sobre este repositório

Este repositório contém os dados brutos utilizados no artigo **"Análise bibliométrica sobre o uso dos Censos brasileiros no século XXI"**. O objetivo é garantir a transparência e a reprodutibilidade da pesquisa, disponibilizando os dados de forma aberta à comunidade científica.

---

## Artigo

> **Título:** Análise bibliométrica sobre o uso dos Censos brasileiros no século XXI  
> **Autores:** Bianca Louzada Xavier Vasconcellos e Georges Gérard Flexor 
> **Instituição:** CPDA/UFRRJ (Grupo de Pesquisa sobre o Censo 2022) - Liderado por Ana Célia Castro  
> **Status:** [Revista Brasileira de Estudos de População/ aceito]  
> **DOI:** [ --- ]

---

## Estrutura do repositório

```
.
├── README.md
├── data/
│   ├── raw/                        ← dados brutos exportados das bases
│   │   ├── scielo.csv              ← exportação da base SciELO
│   │   ├── scopus.csv              ← exportação da base Scopus
│   │   ├── savedrecs.txt           ← exportação da Web of Science (parte 1)
│   │   └── savedrecs-2.txt         ← exportação da Web of Science (parte 2)
│   └── clean/                      ← dados após limpeza e deduplicação
│       └── [adicionar arquivos]
├── code/
│   └── analise.R                   ← script de análise em R
└── docs/
    └── codebook.md                 ← dicionário de variáveis
```

---

## Dados brutos

Os dados foram coletados em **[mês/ano da coleta]** a partir de três bases de dados bibliográficas:

| Arquivo | Base | Formato | Registros |
|---|---|---|---|
| `scielo.csv` | SciELO | CSV | ~1.462 |
| `scopus.csv` | Scopus | CSV | ~2.655 |
| `savedrecs.txt` | Web of Science | formato WoS (.txt) | parte 1 |
| `savedrecs-2.txt` | Web of Science | formato WoS (.txt) | parte 2 |

### Estratégia de busca

A busca foi realizada com os seguintes termos e filtros:

- **Termos de busca:** [descrever os termos utilizados, ex: "Censo Demográfico", "IBGE", "Brazilian Census"...]
- **Período:** [ex: 2000–2023]
- **Tipos de documento:** [ex: artigos, artigos de revisão]
- **Idiomas:** [ex: português, inglês, espanhol]

> ⚠️ Os dados brutos são exportados diretamente das plataformas, sem qualquer modificação. Podem conter duplicatas e registros fora do escopo, que foram tratados na etapa de limpeza.

---

## Dados limpos

Os dados limpos, após deduplicação entre as três bases e aplicação dos critérios de inclusão e exclusão, estão disponíveis na pasta `data/clean/`.

[Descrição dos critérios de inclusão/exclusão utilizados]

---

## Como usar

### Requisitos

- **R** (versão ≥ 4.0)
- Pacotes R: `bibliometrix`, `tidyverse`, `ggplot2` *(adicionar conforme necessário)*

### Reproduzindo a análise

```r
# Instalar pacotes necessários
install.packages(c("bibliometrix", "tidyverse"))

# Executar a análise
source("code/analise.R")
```

---

## Citação

Se você utilizar estes dados, por favor cite:

```
VASCONCELLOS, Bianca Louzada Xavier; FLEXOR, Georges Gérard. Análise bibliométrica sobre o uso dos 
Censos brasileiros no século XXI. REBEP, 2026. 
DOI: [ ---- ]
```

---

## Licença

Os dados estão disponibilizados sob a licença [Creative Commons CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.pt_BR), que permite uso, distribuição e adaptação, desde que a autoria seja devidamente citada.

---

## Contato

Dúvidas ou sugestões? Entre em contato:  
🔗 [https://www.linkedin.com/in/bianca-louzada-xavier-vasconcellos-45b258169/]  
🔗 [https://lattes.cnpq.br/6522952293111002]
