---
title: "Periodicidade e temporadas"
tipo: "nota"
status: "requisito-documentado"
atualizado_em: "2026-10-22"
fontes: ["https://app.notion.com/p/3fbfe13c365280ef892cde6bc50c9e54?pvs=204", "Decisão do usuário — 2026-10-22"]
---

# Periodicidade e temporadas

O sistema deverá permitir duas formas de acompanhamento dos resultados:

**A) Ranking mensal automático**

- A apuração será realizada mensalmente, considerando as ações registradas do primeiro ao último dia de cada mês.
- No dia 1º de cada mês, deverá ser disponibilizado o resultado referente ao mês anterior.
- A pontuação mensal deverá respeitar os critérios e limites definidos para cada evento dentro do período.
- Os resultados dos meses anteriores deverão permanecer disponíveis no histórico.

**B) Ranking por temporada**

- A escola poderá configurar temporadas próprias, definindo o período de validade do ranking.
- A configuração deverá permitir selecionar os meses que compõem cada temporada.
- O sistema deverá permitir temporadas baseadas no calendário convencional, como bimestres, semestres e ano completo, ou períodos personalizados.
- Exemplos de configuração:
  - Primeiro semestre: janeiro a junho.
  - Segundo semestre: julho a dezembro.
  - Temporada trimestral: três meses selecionados pela escola.
  - Temporada personalizada: qualquer combinação de meses consecutivos definida pela escola.
- A escola deverá conseguir consultar a pontuação acumulada dos atletas durante a temporada vigente.
- Ao encerrar uma temporada, o resultado final deverá ser consolidado e armazenado no histórico.
- A criação de uma nova temporada deverá permitir configurar um novo período sem alterar os resultados históricos das temporadas anteriores.

**Regra para alteração de temporada:** caso a escola reduza a quantidade de meses de uma temporada já configurada, a alteração deverá valer somente para a próxima temporada, sem modificar retroativamente o período ou o resultado da temporada em andamento.

O sistema deverá distinguir claramente a pontuação mensal da pontuação por temporada, evitando confusão entre os dois resultados.

## Múltiplas temporadas no mesmo ano

O protótipo deve permitir criar e selecionar diversas temporadas para um mesmo ano. Cada uma é identificada pelo nome, ano e pelos meses de vigência. O ano deve ser selecionável para permitir configuração de períodos futuros.

Cada mês pode estar associado a somente uma temporada dentro do mesmo ano. Assim, um mês já incluído em uma temporada de 2027 fica indisponível para as demais temporadas de 2027; essa restrição não se estende a outros anos.

## Fontes

- [Ranking de pontuação: Atletas, Usuários e Equipes](https://app.notion.com/p/3fbfe13c365280ef892cde6bc50c9e54?pvs=204)

## Conexões

[[03-Rankings/Visao-geral-ranking]] · [[03-Rankings/Configuracao-do-ranking-de-equipes]] · [[90-Fontes/F24-Multiplas-temporadas-no-ano]] · [[90-Fontes/F25-Exclusividade-de-meses-e-premiacao-opcional]] · [[00-Mapa/Pendencias]] · [[90-Fontes/F01-Ranking-de-pontuacao-Atletas-Usuarios-e-Equipes]]
