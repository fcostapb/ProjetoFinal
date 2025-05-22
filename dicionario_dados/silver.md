# Dicionário de Dados - Camada Silver

## Tabela: players_enhanced

| Coluna               | Tipo     | Descrição                                      |
|----------------------|----------|------------------------------------------------|
| player_api_id        | long     | ID único do jogador                           |
| player_name          | string   | Nome completo do jogador                      |
| height               | double   | Altura em cm                                  |
| weight               | double   | Peso em kg                                   |
| birth_date           | date     | Data de nascimento                            |
| birth_year           | int      | Ano de nascimento                             |
| position_category    | string   | Categoria de posição (Goalkeeper/Defender/Midfielder/Forward) |
| overall_rating       | double   | Avaliação geral do jogador                    |
| potential            | double   | Potencial futuro                              |
| ... (outros atributos) | ...    | Atributos técnicos do FIFA                    |

## Tabela: matches_cleaned

| Coluna               | Tipo     | Descrição                                      |
|----------------------|----------|------------------------------------------------|
| match_id             | long     | ID único da partida                           |
| match_date           | date     | Data da partida                               |
| season_start_year    | int      | Ano de início da temporada                    |
| league_id            | long     | ID da liga                                    |
| home_team_id         | long     | ID do time da casa                            |
| away_team_id         | long     | ID do time visitante                          |
| home_team_goal       | int      | Gols do time da casa                          |
| away_team_goal       | int      | Gols do time visitante                        |
| match_result         | string   | Resultado (Home Win/Away Win/Draw)            |
| total_goals          | int      | Total de gols na partida                      |
| avg_home_odds        | double   | Média das odds para vitória da casa           |