O arquivo 03-Veículo deve conter Informações sobre os veículos utilizados e seus respectivos
custos.

| Campo                  | Tipo               | Descrição                                                                                                                                                                                                                             | Obrigatório |
|------------------------|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------|
| Instancia              | Texto              | Descrição de uma instância ou conjunto de instalações.                                                                                                                                                                                | Sim         |
| CustoFixo              | Número Decimal (6)  | Custo fixo do veículo por viagem.                                                                                                                                                                                                     | Sim         |
| CustoVariavel          | Número Decimal (6)  | Custo variável do veículo associado à distância percorrida.                                                                                                                                                                           | Sim         |
| IDVeiculo              | Texto              | Código único de identificação de um veículo.                                                                                                                                                                                          | Sim         |
| TempoDisponivel        | Número Decimal (6)  | Tempo total disponível de rota em horas.                                                                                                                                                                                              | Sim         |
| TipoVeiculo            | Texto              | Tipo do veículo utilizado: <ul><li>Passeio/Leve</li><li>Comercial/Leve</li><li>Leves</li><li>Semileves</li><li>Médios</li><li>Semipesado</li><li>Pesados</li></ul>                                                                     | Não         |
| Capacidade             | Número Decimal (6)  | Limitação máxima (dada em termos da Unidade de Medida Logística) que o veículo pode operar.                                                                                                                                            | Não         |
| CapacidadePeso         | Número Decimal (6)  | Limitação máxima de peso que o veículo pode operar.                                                                                                                                                                                   | Não         |
| CapacidadeQtdDeItens   | Número Decimal (6)  | Limitação máxima de itens que o veículo pode operar.                                                                                                                                                                                  | Não         |
| CapacidadeValor        | Número Decimal (6)  | Limitação máxima de valor agregado que o veículo pode operar.                                                                                                                                                                         | Não         |
| CapacidadeVolume       | Número Decimal (6)  | Limitação máxima de volume que o veículo pode operar.                                                                                                                                                                                 | Não         |
| FatorVelocidade        | Número Decimal (6)  | Coeficiente para que será multiplicado pelo tempo, caso o campo "Tempo" do arquivo 04-MatrizOD tenha sido importado.                                                                                                                   | Não         |
| TempoDescargaFixo      | Número Decimal (6)  | Tempo de descarregamento fixo em um veículo por cliente (dado em termos da unidade de medida logística definida pelo modelo).                                                                                                          | Não         |
| TempoDescargaVariavel  | Número Decimal (6)  | Tempo de descarregamento variável associado a um veículo por cliente, em horas.                                                                                                                                                       | Não         |
| Velocidade             | Número Decimal (6)  | Velocidade média de deslocamento do veículo em “km/h”.                                                                                                                                                                                | Não         |
| VelocidadeCruzeiro     | Número Decimal (6)  | Velocidade cruzeiro do veículo, definida como o valor de galão por milha e o ponto ótimo de utilização do veículo.                                                                                                                     | Não         |
| VolumeMinimo       | Número Decimal (6)  | Limitação mínima de carga (dada em termos da Unidade de Medida Logística) que o veículo pode operar.                                                                     | Não         |
| TipoVeiculoMOPEC   | Texto              | Tipo de veículo para cálculo de emissão de CO2, cada veículo desse arquivo pode ter uma dessas classificações: <ul><li>Passeio/Leve</li><li>Comercial/Leve</li><li>Leves</li><li>Semileves</li><li>Médios</li><li>Semipesados</li><li>Pesados</li></ul> Campo obrigatório para o cálculo de emissão de CO2. | Não         |

Os parâmetros veiculares do campo “TipoVeiculoMOPEC” são exclusivos para o cálculo de
emissões de CO² do Módulo MOPEC.

O MOPEC é o Módulo Multiplataforma de Otimização da Pegada de Carbono da nossa plataforma
de soluções e é integrado com o SPOT.R de modo a permitir o cálculo e otimização das emissões totais
equivalentes em toneladas de CO2, levando em consideração parâmetros por tipo de veículo.

São 7 categorias de veículos para a distribuição, cada um com sua autonomia e emissão de CO2, o
cálculo é feito da seguinte forma:

$$
Cálculo\ de\ CO_2\ [kg] = \frac{Distância\ [km]}{Autonomia\ \left[\frac{km}{litro}\right]} \times Emissão\ \left[\frac{kg}{litro}\right]
$$


| Veículo           | Exemplo de veículo     | Autonomia (km/litro) | Emissão de CO2 (kg/litro) |
|-------------------|------------------------|----------------------|--------------------------|
| Passeio Leve      | Carro de passeio        | 13,4                 | 2,1                      |
| Comercial Leve    | Van                    | 10,9                 | 2,1                      |
| Leves             | VUC                    | 5,6                  | 2,62                     |
| Semi Leves        | Caminhão pequeno        | 9,1                  | 2,62                     |
| Médios            | Caminhão médio          | 5,6                  | 2,62                     |
| Semi Pesado       | Caminhão grande         | 3,4                  | 2,62                     |
| Pesados           | Carreta                | 3,4                  | 2,62                     |

