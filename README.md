# Mapa de Densidade de Raios (Ng) por Município — Brasil

Cópia dos dados de densidade de descargas atmosféricas (**Ng**, raios/km²/ano) por município
brasileiro, usados no módulo SPDA (Sistema de Proteção contra Descargas Atmosféricas) do sistema
GESTOR (EDUCANR Treinamentos e Consultoria), conforme **ABNT NBR 5419-2:2026, Anexo F**.

## Origem dos dados

Estes dados foram copiados do projeto público **ng-brasil-mapas**, de Rafael Fernandes:

- Repositório original: https://github.com/rafaelf09/ng-brasil-mapas
- Arquivo de origem: `docs/ng_dados.json`
- Licença: MIT (ver `LICENSE` neste repositório)

Segundo o autor original, o campo `ng_nbr5419_2026` reproduz a Tabela F.1 (Anexo F) da norma
vigente. Antes de usar aqui, validamos manualmente 9 municípios lidos diretamente da norma
(arquivo escaneado da ABNT) contra este dataset — **9 de 9 bateram exatamente**.

## Arquivos

- `ng_dados.json` — cópia integral do arquivo original (inclui também os valores da geração
  antiga de dados, 2015, pra referência histórica/comparação).
- `ng_nbr5419_2026_por_municipio.csv` — versão simplificada em CSV, só com o valor vigente
  (`codigo_ibge, municipio, uf, ng_nbr5419_2026`), a mesma usada pela tabela `spda_ng_municipios`
  do GESTOR.
- `ng_dados_2015_geracao_antiga.csv` — dados da geração antiga (grid histórico INPE 1988-2011),
  só para referência/comparação, não usados no cálculo do GESTOR.

## Aviso técnico

Estes valores são uma cópia de conveniência para consulta rápida. Para uso formal em laudo
técnico ou projeto de SPDA, **confirme sempre o valor diretamente no Anexo F da ABNT NBR
5419-2:2026 vigente**.
