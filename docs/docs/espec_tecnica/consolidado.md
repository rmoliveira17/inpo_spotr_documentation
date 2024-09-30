# Introdução

Os arquivos (formato .txt, .xlsx ou .csv) abaixo armazenam as informações resultantes da execução
do modelo de otimização da cadeia de suprimentos, após respectiva importação dos arquivos de entrada.

## Consolidado

Contém o resultado de roteirização de cada rota e informações detalhadas dos fluxos de
transporte, incluindo quilometragem rodada, tempo de rota, quantidade de carga transportada em
unidades, peso, volume e valor.

Campos:

| Campo              | Tipo               | Descrição                                                                                                                                                              |
|--------------------|--------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Grupo              | Texto              | Código único de identificação de uma instalação.                                                                                                                       |
| Id Rota            | Número Inteiro      | Código único de identificação de uma rota.                                                                                                                             |
| Veiculo            | Texto              | Código único de identificação de um veículo.                                                                                                                           |
| Qtd Veiculo        | Número Inteiro      | Quantidade de veículos utilizados em uma determinada rota.                                                                                                             |
| Custo Rota         | Número Decimal (6)  | Custo total de transporte de uma determinada rota.                                                                                                                     |
| KM Total           | Número Decimal (6)  | Quilometragem total percorrida em uma determinada rota.                                                                                                                |
| KM rodado          | Número Decimal (6)  | Quilometragem total percorrida em uma determinada rota.                                                                                                                |
| KM Interno         | Número Decimal (6)  | Quilometragem total percorrida internamente a um cliente.                                                                                                              |
| Tempo Total Rota   | Número Decimal (6)  | Tempo total gasto para percorrer uma determinada rota.                                                                                                                 |
| Tempo Parado       | Número Decimal (6)  | Tempo total gasto para descarregamentos e carregamentos de uma determinada rota.                                                                                        |
| Quantidade de Itens| Número Inteiro      | Quantidade transportada, em itens, associada a uma determinada rota.                                                                                                    |
| Peso               | Número Decimal (6)  | Quantidade transportada, em peso, associada a uma determinada rota.                                                                                                     |
| Volume             | Número Decimal (6)  | Quantidade transportada, em volume, associada a uma determinada rota.                                                                                                   |
| Valor              | Número Decimal (6)  | Quantidade transportada, em valor, associada a uma determinada rota.                                                                                                    |
| Quantidade         | Número Decimal (6)  | Quantidade transportada, dada em termos da Unidade de Medida Logística definida, associada a uma determinada rota.                                                      |
| Ocupação           | Número Decimal (6)  | Ocupação média de um determinado tipo de veículo associada à rota correspondente.                                                                                       |
| Rentabilidade      | Número Decimal (6)  | Diferença entre o custo do frete e o custo da rota. Quando esse valor é positivo, representa que houve redução do custo.                                                |


