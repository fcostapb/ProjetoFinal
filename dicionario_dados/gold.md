# Dicionário de Dados - Camada Gold

## Tabela: player_performance_trends

| Coluna               | Tipo     | Descrição                                      |
|----------------------|----------|------------------------------------------------|
| player_api_id        | long     | ID único do jogador                           |
| player_name          | string   | Nome completo do jogador                      |
| birth_year           | int      | Ano de nascimento                             |
| position_category    | string   | Categoria de posição                          |
| avg_overall_rating   | double   | Média da avaliação geral                      |
| avg_potential        | double   | Média do potencial                            |
| position_rank        | int      | Ranking na posição                            |
| ... (outras médias)  | ...      | Médias dos atributos técnicos                 |

## Tabela: team_season_stats

| Coluna               | Tipo     | Descrição                                      |
|----------------------|----------|------------------------------------------------|
| season_start_year    | int      | Ano de início da temporada                    |
| league_id            | long     | ID da liga                                    |
| team_id              | long     | ID do time                                    |
| team_name            | string   | Nome do time                                  |
| total_matches        | int      | Total de partidas jogadas                     |
| wins                 | int      | Vitórias                                      |
| draws                | int      | Empates                                       |
| losses               | int      | Derrotas                                      |
| points               | int      | Pontos (3 por vitória, 1 por empate)          |
| goal_difference      | int      | Saldo de gols                                 |
| league_rank          | int      | Posição na liga                               |

## Tabela: player_attribute_evolution

| Coluna               | Tipo     | Descrição                                      |
|----------------------|----------|------------------------------------------------|
| player_api_id        | long     | ID único do jogador                           |
| player_name          | string   | Nome completo do jogador                      |
| season_start_year    | int      | Ano da temporada                              |
| avg_rating           | double   | Média da avaliação na temporada               |
| avg_potential        | double   | Média do potencial na temporada               |
| ... (outras médias)  | ...      | Médias dos atributos por temporada            |