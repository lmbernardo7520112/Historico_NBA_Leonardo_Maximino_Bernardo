## 🏀 Desvendando o Legado Estatístico da NBA

Desenvolvido por: Leonardo Maximino Bernardo


Este repositório, de autoria de Leonardo Maximino Bernardo, oferece acesso aos dados por trás de um registro histórico completo e interativo da NBA. Mantido com atualizações frequentes, este conjunto de dados se baseia nas informações de jogos meticulosamente coletadas do site Basketball-Reference.com.

No centro deste acervo encontra-se o arquivo `nbaallelo.csv`, um compêndio detalhado que encapsula a história da liga através de uma série de variáveis cuidadosamente selecionadas. Abaixo, você encontrará uma descrição concisa de cada coluna e seu significado dentro deste contexto estatístico:

| Cabeçalho        | Definição                                                                                                                      |
|-----------------|---------------------------------------------------------------------------------------------------------------------------------|
| 🔢 `gameorder`      | Ordem cronológica do jogo na história da NBA.                                                                                  |
| 🆔 `game_id`        | ID único para cada jogo.                                                                                                         |
| 🏀 `lg_id`          | Liga em que o jogo foi disputado.                                                                                                |
| 📑 `_iscopy`        | Indica se o registro do jogo é uma "cópia" da perspectiva do time adversário.                                                  |
| 📅 `year_id`        | Ano em que a temporada terminou.                                                                                                 |
| 🗓️ `date_game`      | Data em que o jogo ocorreu.                                                                                                    |
| 🏆 `is_playoffs`    | Indicador para jogos de playoff (1 para playoff, 0 para temporada regular).                                                       |
|  `team_id`       | Código de três letras para o nome do time (do Basketball Reference).                                                            |
| 🏛️ `fran_id`       | ID da franquia (vários `team_id` podem pertencer ao mesmo `fran_id` devido a mudanças de nome ou transferências).           |
| 🎯 `pts`            | Pontos marcados pelo time.                                                                                                       |
| 💪 `elo_i`          | Classificação Elo do time antes do jogo.                                                                                        |
| 📈 `elo_n`          | Classificação Elo do time após o jogo.                                                                                           |
| 🏆 `win_equiv`     | Número equivalente de vitórias em uma temporada de 82 jogos para um time da qualidade `elo_n`.                                   |
|  `opp_id`        | ID do time adversário (código de três letras).                                                                                   |
|  `opp_fran`      | ID da franquia do adversário.                                                                                                    |
|  `opp_pts`       | Pontos marcados pelo adversário.                                                                                                 |
|  `opp_elo_i`      | Classificação Elo do adversário antes do jogo.                                                                                   |
|  `opp_elo_n`      | Classificação Elo do adversário após o jogo.                                                                                    |
| 🏟️ `game_location`  | Localização do jogo: Casa (H), Fora (A) ou Neutro (N).                                                                            |
| ✅ `game_result`   | Resultado do jogo para o time: Vitória (W) ou Derrota (L).                                                                       |
| 🔮 `forecast`      | Probabilidade de vitória baseada no Elo para o time, considerando a localização do jogo.                                        |
| 📝 `notes`         | Notas adicionais sobre o jogo.                                                                                                 |

## 📼 Momentos Eletrizantes da NBA

Para ilustrar a emoção presente nestes dados,  apresentamos um GIF que captura a intensidade do Jogo 7 das Finais da NBA de 2013:

![Finais NBA 2013 - Jogo 7](https://i.imgur.com/G5n088.gif)

Convidamos você a explorar este repositório e utilizar este conjunto de dados rico para aprofundar seu conhecimento sobre a história da NBA. 🏀

**Observação:** O link original direcionava para um GIF hospedado em um site externo. Para garantir a estabilidade e acessibilidade a longo prazo, substituímos o link pelo GIF embutido diretamente no texto. 

## 🏀🏀🏀  Análise Conclusiva: Desvendando as Dinastias e a Consistência na História da NBA

Nossa jornada exploratória pelos anais da NBA, guiada por dados abrangentes e visualizações elucidativas, chega ao fim com uma compreensão mais profunda da dinâmica da liga ao longo das décadas.  

**Principais Insights:**

* **Evolução do Rating Elo:** 📈 Observamos um crescimento inicial acentuado do Rating Elo médio da liga, indicando um desenvolvimento acelerado das habilidades e estratégias. Após uma fase de adaptação, a liga se estabilizou, sugerindo um equilíbrio competitivo, mas com indícios de uma nova era de alta performance nos anos 2000.

* **Disparidade entre Franquias:** 🏆 O gráfico de boxplot revelou uma clara disparidade entre as franquias.  Enquanto algumas se destacaram com históricos de  sucesso consistente, como Lakers, Celtics, Spurs e Bulls, outras oscilaram entre altos e baixos.

* **Consistência x Média:** 📊  A análise conjunta da consistência e da média do Rating Elo proporcionou uma visão mais completa da performance histórica das franquias, revelando  quem dominou de forma consistente e quem brilhou em momentos específicos.

* **Visualização da Dominância dos Anos 90:** 🕸️ A rede de confrontos dos anos 90 ilustrou a supremacia do Chicago Bulls, evidenciada por seu alto "win-equiv" e  confrontos frequentes com outras equipes de elite.  A baixa variância no Rating Elo do Bulls solidificou sua imagem de  força dominante e consistente da década.

**🏀🏀🏀  Um Legado de Dados para Entender a NBA**

Este repositório, cuidadosamente elaborado por Leonardo Maximino Bernardo,  oferece uma plataforma valiosa para fãs, analistas e entusiastas  mergulharem na rica história da NBA. À medida que a liga avança, este conjunto de dados continuará a crescer,  proporcionando uma base sólida para  desvendar novas  histórias e  perspectivas sobre o basquete.
