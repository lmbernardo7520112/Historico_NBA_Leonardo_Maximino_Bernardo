# 🏀 Desvendando o Legado Estatístico da NBA 📊

**Uma análise histórica e interativa da NBA usando dados do Basketball-Reference.com.**

<div align="center">

<!-- Badges -->
[![License][License-shield]][License-url]
[![Contributors][Contributors-shield]][Contributors-url]
[![Forks][Forks-shield]][Forks-url]
[![Stargazers][Stars-shield]][Stars-url]
[![Issues][Issues-shield]][Issues-url]

[![Python][Python-shield]][Python-url]
[![Pandas][Pandas-shield]][Pandas-url]
[![Matplotlib][Matplotlib-shield]][Matplotlib-url]
[![Seaborn][Seaborn-shield]][Seaborn-url]
[![NetworkX][NetworkX-shield]][NetworkX-url]

*Desenvolvido por: Leonardo Maximino Bernardo*

</div>

<!-- Accordion Navigation -->
<details open>
<summary>📜 Tabela de Conteúdos</summary>
<ol>
  <li><a href="#-sobre-o-projeto">Sobre o Projeto</a></li>
  <li><a href="#-dicionário-de-dados">Dicionário de Dados (`nbaallelo.csv`)</a></li>
  <li><a href="#-momentos-eletrizantes-da-nba">Momentos Eletrizantes da NBA</a></li>
  <li><a href="#-principais-insights-da-análise">Principais Insights da Análise</a></li>
  <li><a href="#%EF%B8%8F-tecnologias-utilizadas">Tecnologias Utilizadas</a></li>
  <li><a href="#-como-usar-os-dados">Como Usar os Dados</a>
    <ul>
      <li><a href="#-pré-requisitos">Pré-requisitos</a></li>
      <li><a href="#-acesso-aos-dados">Acesso aos Dados</a></li>
    </ul>
  </li>
  <li><a href="#-contribuição">Contribuição</a></li>
  <li><a href="#-licença">Licença</a></li>
  <li><a href="#-contato">Contato</a></li>
</ol>
</details>

---

## 📖 Sobre o Projeto

Este repositório oferece acesso a um registro histórico completo e interativo da NBA, ideal para análises estatísticas e exploração de dados. Mantido com atualizações frequentes (baseado na fonte original), o conjunto de dados principal (`nbaallelo.csv`) provém de informações meticulosamente coletadas do renomado site [Basketball-Reference.com](https://www.basketball-reference.com/).

O objetivo é fornecer uma base rica para fãs, analistas e entusiastas mergulharem na história da liga, desvendando padrões, comparando eras e compreendendo a dinâmica<a href="#-sobre-o-projeto">Sobre o Projeto</a></li>
  <li><a href="#-dicionário-de-dados">Dicionário de Dados (`nbaallelo.csv`)</a></li>
  <li><a href="#-momentos-eletrizantes-da-nba">Momentos Eletrizantes da NBA</a></li>
  <li><a href="#-principais-insights-da-análise">Principais Insights da Análise</a></li>
  <li><a href="#%EF%B8%8F-tecnologias-utilizadas">Tecnologias Utilizadas</a></li>
  <li><a href="#-como-usar-os-dados">Como Usar os Dados</a>
    <ul>
      <li><a href="#-pré-requisitos">Pré-requisitos</a></li>
      <li><a href="#-acesso-aos-dados">Acesso aos Dados</a></li>
    </ul>
  </li>
  <li><a href="#-contribuição">Contribuição</a></li>
  <li><a href="#-licença">Licença</a></li>
  <li><a href="#-contato">Contato</a></li>
</ol>
</details>

---

## 📖 Sobre o Projeto

Este repositório oferece acesso a um registro histórico completo e interativo da NBA, ideal para análises estatísticas e exploração de dados. Mantido com atualizações frequentes (baseado na fonte original), o conjunto de dados principal (`nbaallelo.csv`) provém de informações meticulosamente coletadas do renomado site [Basketball-Reference.com](https://www.basketball-reference.com/).

O objetivo é fornecer uma base rica para fãs, analistas e entusiastas mergulharem na história da liga, desvendando padrões, comparando eras e compreendendo a dinâmica das equipes e jogadores ao longo do tempo.

---

## 📑 Dicionário de Dados (`nbaallelo.csv`)

No centro deste acervo encontra-se o arquivo `nbaallelo.csv`, um compêndio detalhado que encapsula a história da liga através de uma série de variáveis cuidadosamente selecionadas. Abaixo, você encontrará uma descrição concisa de cada coluna:

| Cabeçalho        | Definição                                                                                                                      |
| :--------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| 🔢 `gameorder`   | Ordem cronológica do jogo na história da NBA.                                                                                  |
| 🆔 `game_id`     | ID único para cada jogo.                                                                                                         |
| 🏀 `lg_id`       | Liga em que o jogo foi disputado.                                                                                                |
| 📑 `_iscopy`     | Indica se o registro do jogo é uma "cópia" da perspectiva do time adversário (0 ou 1).                                              |
| 📅 `year_id`     | Ano em que a temporada terminou.                                                                                                 |
| 🗓️ `date_game`   | Data em que o jogo ocorreu.                                                                                                    |
| 🏆 `is_playoffs` | Indicador para jogos de playoff (1 para playoff, 0 para temporada regular).                                                       |
| 👕 `team_id`     | Código de três letras para o nome do time (do Basketball Reference).                                                            |
| 🏛️ `fran_id`    | ID da franquia (vários `team_id` podem pertencer ao mesmo `fran_id` devido a mudanças de nome ou transferências).           |
| 🎯 `pts`         | Pontos marcados pelo time.                                                                                                       |
| 💪 `elo_i`       | Classificação Elo do time antes do das equipes e jogadores ao longo do tempo.

---

## 📑 Dicionário de Dados (`nbaallelo.csv`)

No centro deste acervo encontra-se o arquivo `nbaallelo.csv`, um compêndio detalhado que encapsula a história da liga através de uma série de variáveis cuidadosamente selecionadas. Abaixo, você encontrará uma descrição concisa de cada coluna:

| Cabeçalho        | Definição                                                                                                                      |
| :--------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| 🔢 `gameorder`   | Ordem cronológica do jogo na história da NBA.                                                                                  |
| 🆔 `game_id`     | ID único para cada jogo.                                                                                                         |
| 🏀 `lg_id`       | Liga em que o jogo foi disputado.                                                                                                |
| 📑 `_iscopy`     | Indica se o registro do jogo é uma "cópia" da perspectiva do time adversário (0 ou 1).                                              |
| 📅 `year_id`     | Ano em que a temporada terminou.                                                                                                 |
| 🗓️ `date_game`   | Data em que o jogo ocorreu.                                                                                                    |
| 🏆 `is_playoffs` | Indicador para jogos de playoff (1 para playoff, 0 para temporada regular).                                                       |
| 👕 `team_id`     | Código de três letras para o nome do time (do Basketball Reference).                                                            |
| 🏛️ `fran_id`    | ID da franquia (vários `team_id` podem pertencer ao mesmo `fran_id` devido a mudanças de nome ou transferências).           |
| 🎯 `pts`         | Pontos marcados pelo time.                                                                                                       |
| 💪 `elo_i`       | Classificação Elo do time antes do jogo.                                                                                        |
| 📈 `elo_n`       | Classificação Elo do time após o jogo.                                                                                           |
| ✨ `win_equiv`   | Número equivalente de vitórias em uma temporada de 82 jogos para um time da qualidade `elo_n`.                                   |
| 🆚 `opp_id`     | ID do time adversário (código de três letras).                                                                                   |
| 🏛️ `opp_fran`   | ID da franquia do adversário.                                                                                                    |
| 🥅 `opp_pts`    | Pontos marcados pelo adversário.                                                                                                 |
| 💪 `opp_elo_i`   | Classificação Elo do adversário antes do jogo.                                                                                   |
| 📈 `opp_elo_n`   | Classificação Elo do adversário após o jogo.                                                                                    |
| 🏟️ `game_location`| Localização do jogo: Casa (H), Fora (A) ou Neutro (N).                                                                            |
| ✅ `game_result`| Resultado do jogo para o time: Vitória (W) ou Derrota (L).                                                                       |
| 🔮 `forecast`   | Probabilidade de vitória baseada no Elo para o time, considerando a localização do jogo.                                        |
| 📝 `notes`      | Notas adicionais sobre o jogo.                                                                                                 |

---

## 📼 Momentos Eletrizantes da NBA

Para ilustrar a emoção presente nestes dados, apresentamos um GIF que captura a intensidade do Jogo 7 das Finais da NBA de 2013:

<div align="center">
  <img src="https://i.imgur.com/G5n088.gif" alt="Finais NBA 2013 - Jogo 7" width="600"/>
</div>

---

## 💡 Principais Insights da Análise

Nossa jornada exploratória pelos anais da NBA, guiada por este conjunto de dados e visualizações (potencialmente geradas a partir dele), revela aspectos importantes da dinâmica da liga:

*   📈 **Evolução do Rating Elo:** Observa-se um crescimento inicial acentuado do Rating Elo médio da liga, indicando um desenvolvimento acelerado. Após uma fase de adaptação, a liga tende a uma estabilização, sugerindo equilíbrio competitivo, com possíveis novas eras de alta performance surgindo periodicamente.
*   🏆 **Disparidade entre Franquias:** Os dados mostram uma clara diferença histórica entre as franquias. Algumas, como Lakers, Celtics, Spurs e Bulls, demonstram históricos de sucesso mais consistentes, enquanto outras apresentam maior variabilidade.
*   📊 **Consistência vs. Média:** Analisar a média do Rating Elo junto com sua variância (consistência) oferece uma visão mais completa, distinguindo domínios duradouros de picos momentâneos de performance.
*   🕸️ **Visualização de Dominância (Ex: Anos 90):** A análise de confrontos e métricas como "win-equiv" pode ilustrar períodos de supremacia, como a do Chicago Bulls nos anos 90, destacando sua força e consistência frente aos rivais da época.

---

## 🛠️ Tecnologias Utilizadas (na Análise)

A análise dos dados neste repositório (ou análises típicas feitas com ele) geralmente envolve:

*   [![Python][Python-shield]][Python-url]
*   [![Pandas][Pandas-shield]][Pandas-url] (Para manipulação e análise dos dados tabulares)
*   [![Matplotlib][Matplotlib-shield]][Matplotlib-url] / [![Seaborn][Seaborn-shield]][Seaborn-url] (Para visualização de dados)
*   [![NetworkX][NetworkX-shield]][NetworkX-url] (Potencialmente usado para análise de redes de confronto)

---

## 🚀 Como Usar os Dados

Este repositório foca em fornecer o conjunto de dados. Para utilizá-lo:

### 💧 Pré-requisitos

*   Um ambiente Python (3.7+) instalado.
*   Bibliotecas de análise de dados como Pandas (altamente recomendado):
    ```bash
    pip install pandas
    ```
*   Outras bibliotecas como Matplotlib, Seaborn, etc., dependendo da sua análise.

### 💧 Acesso aos Dados

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_Bernardo.git
    cd Historico_NBA_Leonardo_Maximino_Bernardo
    ```
2.  **Localize o arquivo:** O principal conjunto de dados é o `nbaallelo.csv`.
3.  **Carregue e explore:** Use o Pandas ou sua ferramenta preferida para carregar e analisar o CSV.
    ```python
    import pandas as pd

    df = pd.read_csv('nbaallelo.csv')
    print(df.head())
    print(df.info())
    # Comece sua análise!
    ```

---

## 🤝 Contribuição

Contribuições são bem-vindas! Se você tem sugestões para melhorar a organização dos dados, adicionar novas análises ou corrigir informações, por favor:

1.  Faça um Fork do projeto.
2.  Crie uma Branch para sua Feature (`git checkout -b feature/NovaAnalise`).
3.  Fazer Commit de suas alterações (`git commit -m 'Adiciona NovaAnalise'`).
4.  Fazer Push para a Branch (`git push origin feature/NovaAnalise`).
5.  Abrir um Pull Request.

Consulte o arquivo `CONTRIBUTING.md` (se disponível) para mais detalhes.

---

## 📜 Licença

Distribuído sob a Licença MIT. Veja `LICENSE` para mais informações. *(Certifique-se de que um arquivo LICENSE existe e corresponde a MIT)*

---

<!-- MARKDOWN LINKS & IMAGES -->
<!-- URLs atualizadas com o repositório correto -->
[License-shield]: https://img.shields.io/github/license/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_ jogo.                                                                                        |
| 📈 `elo_n`       | Classificação Elo do time após o jogo.                                                                                           |
| ✨ `win_equiv`   | Número equivalente de vitórias em uma temporada de 82 jogos para um time da qualidade `elo_n`.                                   |
| 🆚 `opp_id`     | ID do time adversário (código de três letras).                                                                                   |
| 🏛️ `opp_fran`   | ID da franquia do adversário.                                                                                                    |
| 🥅 `opp_pts`    | Pontos marcados pelo adversário.                                                                                                 |
| 💪 `opp_elo_i`   | Classificação Elo do adversário antes do jogo.                                                                                   |
| 📈 `opp_elo_n`   | Classificação Elo do adversário após o jogo.                                                                                    |
| 🏟️ `game_location`| Localização do jogo: Casa (H), Fora (A) ou Neutro (N).                                                                            |
| ✅ `game_result`| Resultado do jogo para o time: Vitória (W) ou Derrota (L).                                                                       |
| 🔮 `forecast`   | Probabilidade de vitória baseada no Elo para o time, considerando a localização do jogo.                                        |
| 📝 `notes`      | Notas adicionais sobre o jogo.                                                                                                 |

---

## 📼 Momentos Eletrizantes da NBA

Para ilustrar a emoção presente nestes dados, apresentamos um GIF que captura a intensidade do Jogo 7 das Finais da NBA de 2013:

<div align="center">
  <img src="https://i.imgur.com/G5n088.gif" alt="Finais NBA 2013 - Jogo 7" width="600"/>
</div>

---

## 💡 Principais Insights da Análise

Nossa jornada exploratória pelos anais da NBA, guiada por este conjunto de dados e visualizações (potencialmente geradas a partir dele), revela aspectos importantes da dinâmica da liga:

*   📈 **Evolução do Rating Elo:** Observa-se um crescimento inicial acentuado do Rating Elo médio da liga, indicando um desenvolvimento acelerado. Após uma fase de adaptação, a liga tende a uma estabilização, sugerindo equilíbrio competitivo, com possíveis novas eras de alta performance surgindo periodicamente.
*   🏆 **Disparidade entre Franquias:** Os dados mostram uma clara diferença histórica entre as franquias. Algumas, como Lakers, Celtics, Spurs e Bulls, demonstram históricos de sucesso mais consistentes, enquanto outras apresentam maior variabilidade.
*   📊 **Consistência vs. Média:** Analisar a média do Rating Elo junto com sua variância (consistência) oferece uma visão mais completa, distinguindo domínios duradouros de picos momentâneos de performance.
*   🕸️ **Visualização de Dominância (Ex: Anos 90):** A análise de confrontos e métricas como "win-equiv" pode ilustrar períodos de supremacia, como a do Chicago Bulls nos anos 90, destacando sua força e consistência frente aos rivais da época.

---

## 🛠️ Tecnologias Utilizadas (na Análise)

A análise dos dados neste repositório (ou análises típicas feitas com ele) geralmente envolve:

*   [![Python][Python-shield]][Python-url]
*   [![Pandas][Pandas-shield]][Pandas-url] (Para manipulação e análise dos dados tabulares)
*   [![Matplotlib][Matplotlib-shield]][Matplotlib-url] / [![Seaborn][Seaborn-shield]][Seaborn-url] (Para visualização de dados)
*   [![NetworkX][NetworkX-shield]][NetworkX-url] (Potencialmente usado para análise de redes de confronto)

---

## 🚀 Como Usar os Dados

Este repositório foca em fornecer o conjunto de dados. Para utilizá-lo:

### 💧 Pré-requisitos

*   Um ambiente Python (3.7+) instalado.
*   Bibliotecas de análise de dados como Pandas (altamente recomendado):
    ```bash
    pip install pandas
    ```
*   Outras bibliotecas como Matplotlib, Seaborn, etc., dependendo da sua análise.

### 💧 Acesso aos Dados

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_Bernardo.git
    cd Historico_NBA_Leonardo_Maximino_Bernardo
    ```
2.  **Localize o arquivo:** O principal conjunto de dados é o `nbaallelo.csv`.
3.  **Carregue e explore:** Use o Pandas ou sua ferramenta preferida para carregar e analisar o CSV.
    ```python
    import pandas as pd

    # Ajuste o caminho se o CSV não estiver na raiz após clonar
    df = pd.read_csv('nbaallelo.csv') 
    print(df.head())
    print(df.info())
    # Comece sua análise!
    ```

---

## 🤝 Contribuição

Contribuições são bem-vindas! Se você tem sugestões para melhorar a organização dos dados, adicionar novas análises ou corrigir informações, por favor:

1.  Faça um Fork do projeto.
2.  Crie uma Branch para sua Feature (`git checkout -b feature/NovaAnalise`).
3.  Fazer Commit de suas alterações (`git commit -m 'Adiciona NovaAnalise'`).
4.  Fazer Push para a Branch (`git push origin feature/NovaAnalise`).
5.  Abrir um Pull Request.

Consulte o arquivo `CONTRIBUTING.md` (se disponível) para mais detalhes.

---

## 📜 Licença

Distribuído sob a Licença MIT. Veja `LICENSE` para mais informações. *(Certifique-se de que um arquivo LICENSE existe e corresponde a MIT)*

---

## 📧 Contato

Leonardo Maximino Bernardo

*   GitHub: [@lmbernardo7520112](https://github.com/lmbernardo7520112)
*   Email: <leonardo.bernardo@professor.pb.gov.br> ou <lmbernardo752011@gmail.com>

Link do Projeto: [https://github.com/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_Bernardo](https://github.com/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_Bernardo)

---

<!-- MARKDOWN LINKS & IMAGES -->
[License-shield]: https://img.shields.io/github/license/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_Bernardo?style=flat-square&color=informational
[License-url]: https://github.com/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_Bernardo/blob/main/LICENSE
[Contributors-shield]: https://img.shields.io/github/contributors/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_Bernardo?style=flat-square&color=informational
[Contributors-url]: https://github.com/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_Bernardo/graphs/contributors
[Forks-shield]: https://img.shields.io/github/forks/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_Bernardo?style=flat-square&color=informational
[Forks-url]: https://github.com/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_Bernardo/network/members
[Stars-shield]: https://img.shields.io/github/stars/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_Bernardo?style=flat-square&color=informational
[Stars-url]: https://github.com/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_Bernardo/stargazers
[Issues-shield]: https://img.shields.io/github/issues/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_Bernardo?style=flat-square&color=informational
[Issues-url]: https://github.com/lmbernardo7520112/Historico_NBA_Leonardo_Maximino_Bernardo/issues

[Python-shield]: https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white
[Python-url]: https://www.python.org/
[Pandas-shield]: https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white
[Pandas-url]: https://pandas.pydata.org/
[Matplotlib-shield]: https://img.shields.io/badge/Matplotlib-11557C?style=flat-square&logo=matplotlib&logoColor=white
[Matplotlib-url]: https://matplotlib.org/
[Seaborn-shield]: https://img.shields.io/badge/Seaborn-882255?style=flat-square&logo=seaborn&logoColor=white
[Seaborn-url]: https://seaborn.pydata.org/
[NetworkX-shield]: https://img.shields.io/badge/NetworkX-2A78B8?style=flat-square&logo=networkx&logoColor=white
[NetworkX-url]: https://networkx.org/
