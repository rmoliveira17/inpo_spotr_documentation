Este manual se refere à versão 6.4.1 do SPOT.R. As principais funcionalidades das versões 6.X do SPOT.RTM, em relação às versões anteriores são:

* Priorização de demanda;
* Parametrização de diferentes modalidades de custeios;
* Janela de atendimento de cliente;
* Restrições de circulação de veículo por cliente;
* Visualização interativa de dados georreferenciados.

O resumo do changelog das últimas versões desenvolvidas é exposto a seguir:

| Tipo      | Título                                | Descrição                                                                                         | Versão |
|-----------|---------------------------------------|---------------------------------------------------------------------------------------------------|--------|
| Melhoria  | Salvar todos os resultados            | Botão que permite salvar todas as soluções de uma só vez.                                          | 6.4.1  |
| Melhoria  | Nome da aba modelo                    | Atualização no nome da aba de "Modelo" para "Parâmetros".                                          | 6.4.1  |
| Melhoria  | Sugestão de melhoria                  | Página que permite cadastrar feedbacks da ferramenta.                                              | 6.4.1  |
| Melhoria  | Funcionalidade de Rentabilidade       | Nova funcionalidade de rentabilidade, necessário adicionar nova coluna de "FretePago?" no arquivo "01-Cliente". | 6.4.1  |
| Melhoria  | Interromper execução                  | Funcionalidade que permite interromper a execução e ter o último resultado encontrado do modelo, mas não o melhor. | 6.3.4  |
| Melhoria  | Arquivo de parâmetros otimizado       | Complemento no arquivo de parâmetros, agora é possível importar apenas a instância a ser rodada junto com outros parâmetros. | 6.3.4  |
| Melhoria  | Log de operação                       | Registra eventos da ferramenta, como as etapas de execução do modelo.                             | 6.3.4  |
| Melhoria  | Salvar arquivos em .csv               | Output de resultados em .csv.                                                                     | 6.3.4  |
| Melhoria  | Possibilidade de excluir e inserir linhas pela interface | Todas as tabelas do modelo podem ter linhas adicionadas ou excluídas com facilidade pela interface da ferramenta. | 6.3.4  |
| Melhoria  | Painel de análise de demanda          | Painel com análises básicas de demanda do modelo com um dashboard.                                | 6.3.4  |
| Melhoria  | Importar arquivos de cenários         | Facilitar a seleção de múltiplas instâncias e diferentes arquivos para rodadas, viabilizando a execução de múltiplos cenários de uma só vez. | 6.3.4  |
| Melhoria  | Possibilidade de ordenar os arquivos de input e output | Todas as tabelas da interface (inputs e outputs) passam a possuir funções de filtro e ordenação.     | 6.3.4  |
| Melhoria  | Cálculo da emissão de CO²             | Inclusão nos relatórios de Transferência, distribuição e consolidação da emissão de CO².           | 6.3.4  |
| Melhoria  | Novo relatório de parâmetros utilizados | Criação de novo arquivo de parâmetros utilizados na rodada como parte dos resultados.              | 6.3.4  |
| Melhoria  | Zoom nas tabelas                     | Habilitada a possibilidade de aplicação de zoom nas tabelas da interface da ferramenta.            | 6.3.3  |
| Melhoria  | Mapa para MatrizOD                          | Novo botão no painel para visualizar os fluxos existentes no arquivo 04-MatrizOD.                                                                          | 6.3.3  |
| Melhoria  | Edição de campos dos arquivos de input diretamente pela interface | Todas as telas de input de arquivos possuem 3 novos botões localizados no canto superior direito, nesta ordem, permitem as seguintes ações: editar campos, duplicar instâncias, exportar instância. | 6.3.2  |
| Melhoria  | Consideração de Pedágios                     | Agora é possível considerar o custo de pedágios na roteirização.                                                                                           | 6.3.2  |
| Melhoria  | Legenda nos botões                           | Agora os botões e painéis têm uma breve descrição, assim, basta deixar o cursor do mouse parado alguns segundos em cima do botão.                          | 6.3.1  |
| Melhoria  | Exportar templates de preenchimento          | Possibilidade de exportar arquivos específicos da execução do modelo.                                                                                      | 6.3    |
| Melhoria  | Layout Importação de base de distâncias rodoviárias | Reformulação na tela de opções, adição de um controle de status de importação, checkbox para ativar/desativar a função e pré-visualização das distâncias.     | 6.3    |
| Melhoria  | Substituição do arquivo Mapa                 | Agora a visualização do mapa é compatível com qualquer navegador.                                                                                          | 6.3    |
| Melhoria  | Funcionalidade de importação de parâmetros   | Funcionalidade de importação e exportação de parâmetros do sistema.                                                                                        | 6.3    |
| Melhoria  | Exportar templates de preenchimento          | Possibilidade de exportar arquivos específicos da execução do modelo.                                                                                      | 6.3    |
| Melhoria  | Padronização do Mapa                         | Novo ajuste para padronização dos mapas. Todos os ajustes visuais são armazenados e aplicados fazendo com que os mapas fiquem sempre iguais.               | 6.2.2  |
| Melhoria  | Importação de base de distâncias rodoviárias | Agora é possível importar a distância via arquivo no sistema, bem como a sua execução direta.                                                              | 6.2.2  |
| Melhoria  | Novos navegadores aceitos para a visualização | Agora o sistema aceita a função "Visualizar" com essa nova melhoria, fazendo com que o navegador Google Chrome deixe de ser o único aceito.                | 6.2.2  |
| Melhoria  | Botão de cancelamento de execução            | Incluído um novo botão de "Cancelar" no painel de modelo do SPOT-R para cancelar o modelo em execução.                                                     | 6.2.2  |
| Melhoria  | Relatório de distâncias não aceitas          | Agora é gerado um relatório com distâncias que foram ignoradas na importação.                                                                              | 6.2.2  |
| Melhoria  | Exportação de arquivos em Excel              | Permite a exportação dos resultados resumidos em um arquivo .xls, facilitando a análise fora do sistema.                                                   | 6.2.2  |
| Bug       | Novas mensagens de erro                     | Agora, ao importar parâmetros, notificar quais campos obrigatórios estão faltando ou inválidos.                                                            | 6.1    |
| Bug       | Alteração do tipo de caixa de arquivo        | Campo de arquivo ajustado para ficar no mesmo padrão dos outros campos de input.                                                                           | 6.1    |
| Melhoria  | Funcionalidade de base de distância          | Permitir a importação de uma base de "Ref. de distância" para refinamento das distâncias entre pares Origem-Destino.                                        | 6.0    |



