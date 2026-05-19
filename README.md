# bases-pfp

### Fluxo de processamento e integração de bases de dados para geração de planilha estruturada sobre credenciamentos e descredenciamentos no **Programa Farmácia Popular do Brasil (PFP)** em escala nacional.

![License: GPLv3](https://img.shields.io/badge/license-GPLv3-bd0000.svg)
![License: CC BY--NC--SA 4.0](https://img.shields.io/badge/license-CC_BY--NC--SA_4.0-lightgrey.svg)
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-f2c230)
![Version](https://img.shields.io/badge/version-1.0-1d6f42)
![R](https://img.shields.io/badge/language-R-276DC3)
![Quarto](https://img.shields.io/badge/report-Quarto-39729E)
![Data](https://img.shields.io/badge/data-mar%C3%A7o%202026-6f42c1)


## O Projeto

O *geografia-pfp* reúne scripts, bases de dados e rotinas de processamento relacionados à pesquisa de mestrado **“Programa Farmácia Popular: dilemas do acesso público via locais privados”**, desenvolvida no Programa de Pós-Graduação em Geografia Humana da Universidade de São Paulo. O projeto investiga a distribuição territorial e os limites de acesso ao Programa Farmácia Popular do Brasil, com foco na dependência de farmácias privadas credenciadas e nas relações entre Estado, mercado e assistência farmacêutica no território brasileiro. Pesquisa com apoio da Coordenação de Aperfeiçoamento de Pessoal de Nível Superior (CAPES), protocolo 88887.311041/2026-00.

PENZ, C. *geografia-pfp: Geografia - Programa Farmácia Popular*. Disponível em: <osf.io/ptm5y>.

## Descrição

Este repositório reúne rotinas de tratamento, padronização e integração de dados provenientes de duas fontes principais:

- **Ministério da Saúde (MS)**: planilhas de farmácias credenciadas e descredenciadas no Programa Farmácia Popular;
- **Receita Federal do Brasil (RF)**: base pública do Cadastro Nacional da Pessoa Jurídica (CNPJ), utilizada para complementar informações cadastrais dos estabelecimentos.

O fluxo permite:

- leitura automatizada de arquivos `.xlsx` disponibilizados via Open Science Framework (OSF);
- padronização de identificadores CNPJ;
- tratamento de datas de credenciamento e descredenciamento;
- cálculo de estabelecimentos ativos por ano e unidade federativa;
- integração entre bases do Ministério da Saúde e Receita Federal;
- geração de base consolidada para análises espaciais, temporais e institucionais.

Os dados da Receita Federal utilizados neste projeto referem-se à competência de **março de 2026**.

---

## Fonte dos dados

### Ministério da Saúde

Dados de credenciamento e descredenciamento obtidos por consulta ao Portal da Transparência e armazenados em repositório auxiliar na OSF.

### Receita Federal do Brasil

Base pública do Cadastro Nacional da Pessoa Jurídica (CNPJ):

https://dados.receita.fazenda.gov.br/CNPJ/

Arquivos de estabelecimentos foram convertidos para formato `.parquet` para otimização de leitura e processamento.

---

---

# Citação

Para referenciar este trabalho, utilize o seguinte formato:

Penz, C. L. S. *bases-pfp: Fluxo de processamento de dados para gerar planilha estruturada de informações sobre credenciamentos no Programa Farmácia Popular a nível nacional (fevereiro de 2026)* \[Software\]. Universidade de São Paulo. <https://clarapenz.github.io/bases-pfp/>

Para usuários de LaTEX:

```latex
@software{penz_2025,
  title = {bases-pfp: Fluxo de processamento de dados para gerar planilha estruturada de informações sobre credenciamentos no Programa Farmácia Popular a nível nacional (fevereiro de 2026)},
  author = {Clara de Lima e Silva Penz},
  year = {2025},
  address = {São Paulo},
  institution = {Universidade de São Paulo},
  langid = {pt},
  url = {https://clarapenz.github.io/bases-pfp/}
}
```
# Licença

[![Licença: GPLv3](https://img.shields.io/badge/license-GPLv3-bd0000.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Licença: CC BY-NC-SA 4.0](https://img.shields.io/badge/license-CC_BY--NC--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

> As fontes de dados originais podem estar sujeitas a seus próprios termos e condições de licenciamento.

O código deste repositório está licenciado sob a [Licença Pública Geral GNU versão 3](https://www.gnu.org/licenses/gpl-3.0), enquanto o relatório está disponível sob a licença [Creative Commons Atribuição-NãoComercial-CompartilhaIgual 4.0 Internacional](https://creativecommons.org/licenses/by-nc-sa/4.0/).

```
Copyright (C) 2025 Clara L. S. Penz

The code in this report is free software: you can redistribute it and/or
modify it under the terms of the GNU General Public License as published by the
Free Software Foundation, either version 3 of the License, or (at your option)
any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with
this program. If not, see <https://www.gnu.org/licenses/>.
```

# Agradecimentos

Não seria possível organizar este fluxo de processamento sem o conhecimento compartilhado por pesquisadores e trabalhadores do Centro de Estudos da Metrópole, Universidade de São Paulo, Brasil.

Também destaco o papel do Departamento de Geografia da Universidade de São Paulo, bem como da Coordenação de Aperfeiçoamento de Pessoal de Nível Superior (CAPES), respectivamente pelo apoio e fomento a esta pesquisa.

# Referências

BRASIL. Ministério da Saúde. Dados de farmácias credenciadas ao Programa Farmácia Popular do Brasil. Consulta realizada por meio do Portal da Transparência. Brasília, DF, fev. 2026.

BRASIL. Secretaria Especial da Receita Federal do Brasil. **Dados abertos CNPJ – março 2026**. Brasília, DF: Receita Federal do Brasil, 2026. Disponível em: https://dados.receita.fazenda.gov.br/CNPJ/. Acesso em: 18 maio 2026.


