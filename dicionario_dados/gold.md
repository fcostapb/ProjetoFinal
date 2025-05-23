# Dicionário de Dados - Camada Gold

## Tabela: matches
| Coluna          | Tipo    | Descrição                              | Fonte Silver           |
|-----------------|---------|----------------------------------------|------------------------|
| match_id        | BIGINT  | ID único da partida                    | matches_cleaned.id     |
| season          | STRING  | Temporada no formato YYYY/YYYY         | matches_cleaned.season_formatted |
| match_date      | DATE    | Data da partida                        | matches_cleaned.match_date |
| home_team_id    | BIGINT  | ID do time da casa                     | matches_cleaned.home_team_api_id |
| away_team_id    | BIGINT  | ID do time visitante                   | matches_cleaned.away_team_api_id |
| home_score      | INTEGER | Gols do time da casa                   | matches_cleaned.home_team_goal |
| away_score      | INTEGER | Gols do time visitante                 | matches_cleaned.away_team_goal |
| league_id       | BIGINT  | ID da liga/competição                  | matches_cleaned.league_id |
| season_start_year | INTEGER | Ano de início da temporada           | matches_cleaned.season_start_year |
| match_result    | STRING  | Resultado (Home Win, Away Win, Draw)   | matches_cleaned.match_result |
| total_goals     | INTEGER | Total de gols na partida               | matches_cleaned.total_goals |
| avg_home_odds   | DOUBLE  | Média das odds para vitória da casa    | matches_cleaned.avg_home_odds |
| avg_draw_odds   | DOUBLE  | Média das odds para empate             | matches_cleaned.avg_draw_odds |
| avg_away_odds   | DOUBLE  | Média das odds para vitória visitante  | matches_cleaned.avg_away_odds |

## Tabela: players
| Coluna          | Tipo    | Descrição                              | Fonte Silver           |
|-----------------|---------|----------------------------------------|------------------------|
| player_id       | BIGINT  | ID único do jogador                    | players_enhanced.player_api_id |
| player_name     | STRING  | Nome do jogador                        | players_enhanced.player_name |
| birth_date      | DATE    | Data de nascimento                     | players_enhanced.birth_date |
| birth_year      | INTEGER | Ano de nascimento                      | players_enhanced.birth_year |
| height_m        | DOUBLE  | Altura em metros                       | players_enhanced.height_m |
| weight_kg       | DOUBLE  | Peso em kg                             | players_enhanced.weight_kg |
| bmi             | DOUBLE  | Índice de Massa Corporal               | players_enhanced.bmi |
| position_category | STRING | Posição principal (Goleiro, Defensor, etc) | players_enhanced.position_category |
| overall_rating  | INTEGER | Avaliação geral do jogador             | players_enhanced.overall_rating |
| potential       | INTEGER | Potencial do jogador                   | players_enhanced.potential |
| preferred_foot  | STRING  | Pé preferido (right/left)              | players_enhanced.preferred_foot |
