Contém o resultado de roteirização de cada rota, sendo elas segmentadas em trechos que, por
sua vez, são compostos de segmentos que conectam cada par Origem-Destino pertencente à rota em
questão. Para cada trecho, tem-se informações como quilômetros rodados, volume transportado e tempo
gasto.

| Campo               | Tipo               | Descrição                                                                                                                                                              |
|---------------------|--------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Grupo               | Texto              | Código único de identificação de uma instalação.                                                                                                                       |
| Id Rota             | Número Inteiro      | Código único de identificação de uma rota.                                                                                                                             |
| Ordem               | Texto              | Ordem sequencial de um trecho Origem-Destino dentro de uma mesma rota.                                                                                                  |
| Origem              | Texto              | Código único de identificação de uma origem.                                                                                                                           |
| Destino             | Número Decimal (6)  | Código único de identificação de um destino.                                                                                                                           |
| Pedido              | Número Decimal (6)  | Código único de identificação de um pedido.                                                                                                                            |
| Volume              | Número Decimal (6)  | Quantidade transportada, dada em termos da Unidade de Medida Logística definida, associada a um determinado trecho de uma rota.                                          |
| KM                  | Número Decimal (6)  | Quilometragem percorrida em um determinado trecho de uma rota.                                                                                                          |
| Tempo               | Número Decimal (6)  | Tempo gasto para percorrer um determinado trecho de uma rota.                                                                                                           |
| PrioridadeDestino   | Número Decimal (6)  | Opção que permite priorizar a entrega de acordo com critérios internos.                                                                                                |
