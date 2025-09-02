# big-data-espacial

Big Data Espacial – Busca de Dados no Google Maps com RStudio e Google APIs

📌 Proposta da Oficina

Este projeto foi parte do curso de tecnólogo Ciência de Dados para Negócios – Fatec Sebrae e foi inspirado no curso de extensão “Big Data Espacial – Distribuição do Varejo de Serviços em São Paulo”.

O objetivo era capacitar o aluno a levantar informações disponíveis no Google Maps usando RStudio e gerar uma base de dados de estabelecimentos comerciais a partir de um conjunto de coordenadas geográficas.

Durante as aulas, foram apresentados:

Conceitos de Big Data (os 5Vs: Volume, Velocidade, Variedade, Veracidade e Valor).

Instalação e configuração do ambiente RStudio/RTools.

Uso de pacotes do R para conectar-se às APIs do Google (como googleway, httr, jsonlite, entre outros).

Exercícios de programação em R para importar, tratar e visualizar dados espaciais.

Avaliação final: criar uma base de dados real de estabelecimentos e disponibilizar resultados em formato geoespacial (KML/KMZ).


📊 Meus Resultados

Para cumprir a tarefa, desenvolvi (com apoio de IA) um script integrado em R que consulta a Google Places API para localizar livrarias e bibliotecas na cidade de São Paulo.


🔎 Metodologia

Como a API retorna no máximo 60 resultados por busca, foi adotada a estratégia de múltiplos pontos centrais em diferentes regiões da cidade (norte, sul, leste, oeste e extremos).

A sobreposição dessas zonas garantiu uma cobertura mais ampla do território.

Para evitar duplicatas, a filtragem final considerou endereços exatos em vez de apenas nomes.


📌 Observações

Apesar do esforço, uma livraria de grande porte (Martins Fontes Paulista) não apareceu nos resultados, mesmo após ajustes na lógica de deduplicação.

Isso evidencia tanto limitações da API quanto desafios de coleta de dados em projetos de Big Data Espacial.


🗺️ Entregas

Script em R totalmente funcional.

Arquivos KMZ com os pontos mapeados (livrarias e bibliotecas).

Mapa interativo publicado no Google My Maps:
👉 Visualizar o mapa:

https://www.google.com/maps/d/u/0/edit?hl=pt-BR&mid=1KfyhoFiAo3d737hUXeRCFvj3NWceE6E&ll=-23.57563440392239%2C-46.646876000000006&z=10


🚀 Tecnologias Utilizadas

RStudio

Google Places API

Pacotes: httr, dplyr, jsonlite

Saídas geoespaciais: KML/KMZ para visualização no Google My Maps
