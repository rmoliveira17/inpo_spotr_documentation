O arquivo 04-MatrizOD contém informações sobre as distâncias e tempos de percurso, a partir
das origens para os destinos.

| Campo           | Tipo               | Descrição                                                                                                                                                         | Obrigatório |
|-----------------|--------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------|
| Instancia       | Texto              | Descrição de uma instância ou conjunto de origens/destinos.                                                                                                       | Não         |
| IDOrigem        | Texto              | Código único de identificação de uma origem.                                                                                                                     | Não         |
| IDDestino       | Texto              | Código único de identificação de um destino.                                                                                                                     | Não         |
| Distancia       | Número Decimal (6)  | Distância da origem até o destino em km. (campo obrigatório no caso de o usuário querer considerar a Tabela de Frete no modelo).                                   | Não         |
| Tempo           | Número Decimal (6)  | Tempo da origem até o destino em horas.                                                                                                                          | Não         |
