# Recomendação de música (Neo4j)

Projeto/modelo de grafo para **recomendação de músicas** usando Neo4j.

## Modelo (visão geral)
- **Nós**:
  - `User` (usuário)
  - `Song` (música)
  - `Artist` (artista)
  - `Genre` (gênero)
- **Relacionamentos**:
  - `(:User)-[:LISTENED]->(:Song)` (propriedades: `times`, `last_date`)
  - `(:User)-[:LIKED]->(:Song)` (propriedade: `date`)
  - `(:User)-[:FOLLOWS]->(:Artist)` (propriedade: `since`)
  - `(:Song)-[:BY]->(:Artist)`
  - `(:Song)-[:IN_GENRE]->(:Genre)`

## Arquivos
- `recomendacao_musica_arrows.json`: **importável no** [arrows.app](https://arrows.app) (contém `position.x/y`).
- `recomendacao_musica.json`: JSON com **dados** (`nodes` e `relationships`) para uso em scripts/imports no Neo4j.
- `modelo recomendação de música.json` e `modelo recomendação de música.png`: versão do modelo/export (Arrows) e imagem.

## Como visualizar no Arrows
1. Acesse [arrows.app](https://arrows.app)
2. Clique em **Import**
3. Selecione `recomendacao_musica_arrows.json` (ou `modelo recomendação de música.json`)