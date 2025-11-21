Recentemente, desenvolvi um projeto completo de análise de dados, cujo foco foi transformar uma planilha simples do Excel em um dashboard de vendas totalmente funcional no Power BI. O objetivo central deste trabalho envolveu a implementação de um fluxo íntegro — desde a ingestão dos dados até a visualização final — pautado em boas práticas técnicas.

Passo 1 — Ingestão dos Dados
Os dados foram devidamente importados do Excel por meio do recurso "Obter Dados > Pasta de Trabalho". Nesse estágio, o Power BI carregou as tabelas "Vendas" e "Lojas" para o ambiente de análise, permitindo iniciar o processo de preparação e higienização das informações.

Passo 2 — Tratamento e Transformações com Power Query
Ao acessar o editor Power Query, identifiquei desafios típicos de fontes operacionais, tais como:

Erros de digitação

Colunas inconsistentes

Tipos de dados incompatíveis

Informações consolidadas em um único campo

Para resolver essas questões, apliquei as principais transformações:

Substituição de valores para corrigir entradas inadequadas

Padronização de textos com a capitalização de cada palavra

Divisão de colunas por delimitador, separando quantidade e preço unitário

Alteração de tipos de dados para garantir a correta leitura dos campos

Adição de coluna personalizada destinada ao cálculo do valor da venda (Quantidade × Preço Unitário)

Ao fim desses procedimentos, os dados foram organizados e preparados para a etapa de modelagem.

Passo 3 — Modelagem de Dados
No modo de exibição de modelo, estabeleci o relacionamento entre as tabelas "Vendas" e "Lojas" por meio do campo "Código da Loja". Essa ligação viabilizou análises integradas, proporcionando o contexto adequado entre transações e suas respectivas lojas.

Passo 4 — Elaboração de Medidas em DAX
Com a base devidamente modelada, utilizei inicialmente medidas implícitas oferecidas pelo Power BI (como soma e contagem). Posteriormente, desenvolvi uma medida explícita para o cálculo de comissão:

Comissão = SUM(Vendas[Valor Venda]) × 0,05

Esta medida permanece dinâmica, adaptando-se automaticamente aos filtros aplicados no relatório.

Passo 5 — Desenvolvimento dos Visuais
Para a etapa de visualização, priorizei clareza, hierarquia e facilidade na leitura dos dados. Foram utilizados:

Cartões para indicadores chave (KPIs)

Gráfico de colunas clusterizado para análise mensal e por loja

Gráfico de rosca para proporção por meio de pagamento

Tabelas com formatação condicional para demonstração de variações e valores comparativos

Ajuste das interações entre visuais, garantindo respostas adequadas a filtros e segmentações

Passo 6 — Finalização e Design
Para reforçar a identidade visual, apliquei um template desenvolvido previamente no PowerPoint, seguido da padronização das cores e refinamento com o Pincel de Formatação. Ícones, formas e a organização do layout foram cuidadosamente trabalhados para garantir uma experiência visual limpa e eficiente.

Conclusão
Este projeto evidencia o fluxo completo de construção de um dashboard no Power BI, englobando ingestão, transformação, modelagem, geração de medidas e montagem visual. O resultado final é um dashboard interativo, funcional e estruturado para futuras análises.
