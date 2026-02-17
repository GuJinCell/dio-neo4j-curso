# Grafo simples de filmes, atores e diretores

Este repositório contém um modelo de grafos simples mostrando relações entre usuários de uma rede social e os posts feitos nela,
desenvolvido como atividade do curso Neo4J - Análise de Dados com Grafos da plataforma DIO cursos

## Ferramenta utilizada
- https://arrows.app

## Arquivos
- `grafo_rede_social.json`: modelo do grafo exportado do arrows.app
- `grafo.png`: visualização estática do grafo em um exemplo menor

## Como visualizar
1. Acesse https://arrows.app
2. Clique em "Import"
3. Selecione o arquivo `grafo_rede_social.json`

## Descrição do modelo
- Nós representam usuários(user) e posts(post)
- Arestas representam relações como:
  - POSTED
  - LIKED
  - FOLLOWS
  - ABOUT
  - BY
  - IN_GENRE