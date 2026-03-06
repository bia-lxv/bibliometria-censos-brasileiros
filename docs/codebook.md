# Codebook — Dicionário de Variáveis

**Projeto:** Análise bibliométrica sobre o uso dos Censos brasileiros no século XXI  
**Autora:** Bianca Louzada Xavier Vasconcellos e Georges Gérard Flexor

---

## 1. SciELO (`scielo.csv`)

Exportação direta da plataforma SciELO. Formato CSV com separador vírgula.

| Variável | Descrição |
|---|---|
| `ID` | Identificador único do registro na base SciELO |
| `Title` | Título do artigo |
| `Author(s)` | Lista de autores, separados por vírgula |
| `Source` | Fonte completa da publicação (revista, volume, páginas) |
| `Journal` | Nome do periódico |
| `Language(s)` | Idioma(s) do artigo |
| `Publication year` | Ano de publicação |
| `Fulltext URL` | URL para acesso ao texto completo na plataforma SciELO |

---

## 2. Scopus (`scopus.csv`)

Exportação direta da plataforma Scopus. Formato CSV com separador vírgula.

| Variável | Descrição |
|---|---|
| `Authors` | Autores em formato abreviado (Sobrenome Iniciais) |
| `Author full names` | Nomes completos dos autores com ID Scopus |
| `Author(s) ID` | Identificadores únicos dos autores na base Scopus |
| `Title` | Título do artigo |
| `Year` | Ano de publicação |
| `Source title` | Nome do periódico ou fonte |
| `Volume` | Volume da publicação |
| `Issue` | Número/fascículo da publicação |
| `Art. No.` | Número do artigo (quando aplicável) |
| `Page start` | Página inicial |
| `Page end` | Página final |
| `Page count` | Total de páginas |
| `Cited by` | Número de citações recebidas (na data de extração) |
| `DOI` | Digital Object Identifier |
| `Link` | URL para o registro na Scopus |
| `Affiliations` | Afiliações institucionais dos autores |
| `Authors with affiliations` | Autores associados às suas respectivas afiliações |
| `Abstract` | Resumo do artigo |
| `Author Keywords` | Palavras-chave definidas pelos autores |
| `Index Keywords` | Palavras-chave indexadas pela Scopus |
| `Funding Details` | Informações sobre financiamento da pesquisa |
| `Language of Original Document` | Idioma do documento original |
| `Document Type` | Tipo de documento (Article, Review, etc.) |
| `Source` | Base de dados de origem (Scopus) |
| `EID` | Identificador único do documento na Scopus |

---

## 3. Web of Science (`savedrecs.txt` e `savedrecs-2.txt`)

Exportação direta da plataforma Web of Science. Formato de texto estruturado proprietário da Clarivate Analytics, com campos identificados por tags de dois caracteres.

> Os dois arquivos (`savedrecs.txt` e `savedrecs-2.txt`) correspondem à mesma busca, dividida em dois lotes pela plataforma devido ao limite de exportação.

### Principais tags WoS

| Tag | Campo | Descrição |
|---|---|---|
| `PT` | Publication Type | Tipo de publicação (J = Journal article) |
| `AU` | Authors | Autores (formato: Sobrenome, Iniciais) |
| `AF` | Author Full Name | Nomes completos dos autores |
| `TI` | Title | Título do artigo |
| `SO` | Source | Nome do periódico |
| `LA` | Language | Idioma do artigo |
| `DT` | Document Type | Tipo de documento |
| `DE` | Author Keywords | Palavras-chave dos autores |
| `ID` | Keywords Plus | Palavras-chave adicionais geradas pelo WoS |
| `AB` | Abstract | Resumo |
| `C1` | Author Address | Afiliação institucional |
| `RP` | Reprint Address | Endereço do autor correspondente |
| `EM` | Email Address | E-mail do(s) autor(es) |
| `FU` | Funding Agency | Agência(s) financiadora(s) |
| `FX` | Funding Text | Texto completo sobre financiamento |
| `CR` | Cited References | Referências citadas pelo artigo |
| `TC` | Times Cited | Número de vezes citado na base WoS |
| `PY` | Publication Year | Ano de publicação |
| `VL` | Volume | Volume da publicação |
| `IS` | Issue | Número/fascículo |
| `BP` | Beginning Page | Página inicial |
| `EP` | Ending Page | Página final |
| `DI` | DOI | Digital Object Identifier |
| `UT` | Unique Article Identifier | Identificador único do artigo no WoS |
| `ER` | End of Record | Marca o fim de cada registro |

---

## Notas

- Os dados brutos **não foram modificados** em relação às exportações originais das plataformas.
- A data de extração foi **[inserir data]**.
- Possíveis inconsistências entre bases (variação no nome de autores, periódicos, etc.) são inerentes às fontes e foram tratadas na etapa de limpeza — ver `data/clean/`.
