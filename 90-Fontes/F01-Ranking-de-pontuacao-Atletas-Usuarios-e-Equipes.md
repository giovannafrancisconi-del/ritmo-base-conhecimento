---
title: "Ranking de pontuação: Atletas, Usuários e Equipes"
tipo: "nota"
status: "fonte-consultada"
atualizado_em: "2026-10-20"
fontes: ["https://app.notion.com/p/3fbfe13c365280ef892cde6bc50c9e54?pvs=204"]
---

# Ranking de pontuação: Atletas, Usuários e Equipes

> Registro documental consultado em 2026-10-20. Última edição informada pela fonte: 2026-10-20T15:15:27.485Z. Verificação nativa: unverified.

O conteúdo abaixo preserva as afirmações da fonte; linguagem de requisito não comprova implementação. Vídeos são referências, sem transcrição ou análise audiovisual.

#### **Objetivo: **

Desenvolver um sistema de ranking integrado ao aplicativo Ritmo, com pontuação individual para **Atletas, Usuários e Escolas**, considerando ações realizadas na plataforma, utilização das funcionalidades, participação e cumprimento de atividades.

O sistema deverá contabilizar automaticamente pontos positivos e negativos conforme os critérios definidos na planilha de referência, permitindo calcular a pontuação acumulada e a posição de cada participante no ranking.

#### Escopo do desenvolvimento:

Criar três rankings independentes:

- **Ranking de Atletas:** considera pagamentos, pontualidade, participação nas chamadas, avaliações de treino, justificativas de faltas, convocações, documentação, notas de desempenho, interação com mensagens, galeria e tempo de matrícula.
- **Ranking de Usuários:** considera ações realizadas pelos usuários responsáveis pela gestão da escola, como chamadas, inclusão de atletas em grupos, convocações, registros de notas, envio e resposta de mensagens, compartilhamento de fotos e baixas manuais de faturas.
- **Ranking de Escolas:** considera pagamentos recebidos pelo aplicativo, baixas manuais, realização de chamadas, avaliações de satisfação, organização dos grupos de atletas, convocações, registros de notas, comunicação e compartilhamento de fotos.

#### Regras de pontuação:

A pontuação deverá seguir os critérios, valores e condições definidos nas abas **Atleta, Usuário e Escola** da planilha.

[https://docs.google.com/spreadsheets/d/1jUSL969W-z0BVpVlo0Th9lSk9qxTURNEb-5\_qqIA6DU/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1jUSL969W-z0BVpVlo0Th9lSk9qxTURNEb-5_qqIA6DU/edit?usp=sharing)

### Ranking de Atletas

Implementar a contabilização dos seguintes eventos:

- **Pagamentos:** pontuar pagamentos via Pix, pagamentos realizados no vencimento, pagamentos antecipados e pagamentos em atraso.
- **Chamadas:** pontuar a presença registrada na chamada inicial, identificando separadamente atletas adicionados posteriormente.
- **Avaliação de treino:** pontuar o preenchimento da avaliação e aplicar a pontuação negativa quando não houver resposta, conforme a regra definida.
- **Justificativa de falta:** pontuar a justificativa enviada e aplicar a penalidade prevista para faltas não justificadas.
- **Convocações:** pontuar o recebimento, a resposta, a confirmação de participação e a presença no evento.
- **Documentação:** pontuar a inclusão ou renovação de documentos solicitados e aplicar penalidades por pendências conforme a periodicidade definida.
- **Notas de desempenho e pessoais:** pontuar notas públicas com descrição preenchida, de acordo com a classificação em estrelas.
- **Mensagens:** pontuar a visualização, o acesso à mensagem e o clique em links.
- **Galeria:** pontuar o compartilhamento de fotos, condicionado à validação da escola.
- **Bonificações por tempo de matrícula:** considerar os marcos de mais de 3, 6 e 12 meses, conforme a tabela de pontuação.

### Ranking de Usuários

Implementar a contabilização das seguintes ações:

- Baixa manual de faturas de atletas, com aplicação de pontuação negativa.
- Realização de chamadas.
- Avaliações de satisfação abaixo da nota de referência.
- Inclusão de atletas em grupos ou turmas.
- Criação de convocações.
- Realização da chamada de eventos e convocações.
- Inclusão de notas públicas de desempenho ou pessoais, com descrição preenchida.
- Envio de avisos e mensagens aos atletas.
- Resposta às mensagens recebidas dos atletas.
- Compartilhamento de fotos com atletas e responsáveis.

Os pontos devem ser atribuídos ao usuário responsável pela ação, respeitando os critérios e as condições definidos na planilha.

### Ranking de Escolas

Implementar a contabilização das seguintes ações:

- Pagamentos recebidos por meio do aplicativo.
- Baixas manuais de faturas, com aplicação de pontuação negativa.
- Realização de chamadas.
- Avaliações de satisfação abaixo da nota de referência.
- Ausência de chamadas durante o período semanal definido.
- Atletas que permanecem fora de grupos ou turmas.
- Inclusão de atletas em grupos.
- Criação de convocações.
- Realização de chamadas de eventos e convocações.
- Inclusão de notas públicas de desempenho ou pessoais, com descrição preenchida.
- Envio e resposta de mensagens.
- Compartilhamento de fotos com atletas e responsáveis.

A pontuação deverá refletir as atividades da escola e ser calculada conforme as regras estabelecidas para cada evento

#### Regras gerais do ranking

#### Periodicidade e temporadas

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

### Configuração das temporadas pela escola

Disponibilizar uma área de configuração para que a escola possa:

- Criar e nomear uma temporada.
- Selecionar os meses de início e término ou os meses que farão parte do período.
- Consultar a temporada vigente.
- Visualizar as datas de início e encerramento.
- Definir a pontuação utilizada naquela temporada.
- Configurar as premiações vinculadas ao ranking.
- Consultar temporadas anteriores e seus resultados.
- Criar uma nova temporada com regras atualizadas.

As alterações de configuração deverão respeitar as regras de vigência, preservando os resultados já consolidados.

### Premiações

Criar uma configuração para que a escola defina se haverá premiação ou não vinculada ao ranking e quais benefícios serão oferecidos aos atletas.

O sistema deverá permitir informar a descrição da premiação e exibi-la na área do ranking para que os atletas e responsáveis conheçam os benefícios disponíveis.

Sugestões de premiação:

- Desconto na mensalidade, Uniforme esportivo, Camisa personalizada, Garrafa, Bola, Chaveiro, Brindes diversos e Outras premiações definidas pela escola.

A escola deverá poder configurar a premiação por temporada, permitindo que os benefícios sejam diferentes entre períodos (mensal ou temporada)

Quando houver premiação configurada, ela deverá ficar visível no ranking, com a descrição do benefício e a indicação dos critérios de classificação, conforme as regras definidas pela escola.

A configuração da premiação deverá permitir identificar quais posições serão contempladas, como os três primeiros colocados, ou estabelecer outro critério de elegibilidade.

### Atletas bolsistas

Definir e implementar uma regra específica para atletas bolsistas, considerando sua participação no ranking e sua elegibilidade às premiações.

A regra deverá ser validada com Produto antes da implementação, contemplando as seguintes definições:

- Se atletas bolsistas participarão normalmente do ranking.
- Se haverá uma categoria específica para esses atletas.
- Se poderão concorrer às mesmas premiações dos demais atletas.
- Como tratar atletas com bolsa integral ou parcial, caso exista diferença de regra.

A condição de bolsista deverá ser considerada na apuração somente conforme a regra de negócio aprovada, sem alterar indevidamente a pontuação gerada pelas ações do atleta.

### Configuração e alteração da pontuação

- A pontuação padrão deverá ser definida internamente pelo Ritmo, utilizando os critérios e valores da planilha como referência.
- A escola poderá ter a possibilidade de alterar os valores de pontuação conforme as permissões e regras definidas pelo produto.
- Deverá ser possível configurar pontuações específicas por temporada.
- As alterações de pontuação deverão ter uma vigência definida, evitando modificar retroativamente os resultados de períodos já encerrados.
- O sistema deverá manter o registro das regras utilizadas em cada temporada, permitindo auditar e reproduzir os resultados históricos.
- Caso uma escola não personalize a pontuação, deverão ser aplicadas as regras padrão do Ritmo.

## Disponibilização do ranking nos aplicativos

### Ritmo Equipes — visão da escola

Criar um novo menu denominado **Ranking** no aplicativo Ritmo Equipes.

Nesse menu, deverão ser apresentados:

- Os três primeiros colocados em destaque (Top 3).
- A listagem dos demais atletas ativos da escola, ordenada pela pontuação.
- A pontuação total de cada atleta no período selecionado.
- A identificação da temporada ou do mês de referência.
- A premiação configurada pela escola, quando houver.
- O acesso ao detalhamento da pontuação individual de cada atleta.
- O histórico das temporadas encerradas.

Ao selecionar um atleta na listagem, o usuário deverá acessar uma tela com o detalhamento dos pontos positivos e negativos, seguindo a mesma lógica já aplicada no Ritmo Atletas.

A listagem deverá considerar os atletas ativos da escola, respeitando as regras de elegibilidade definidas para o ranking.

### Ritmo Atletas — visão do responsável

O aplicativo Ritmo Atletas deverá disponibilizar ao responsável o detalhamento da pontuação do atleta, conforme o modelo já aplicado.

Deverá ser possível consultar:

- A posição do atleta no ranking.
- A pontuação acumulada.
- O detalhamento dos pontos recebidos e perdidos.
- A descrição dos eventos que geraram cada pontuação.
- O período de referência, seja mensal ou por temporada.
- A premiação disponível, quando configurada pela escola.
- O histórico dos resultados, conforme a disponibilidade definida para o produto.

A experiência deverá ser consistente com o ranking disponibilizado no Ritmo Equipes, garantindo que a pontuação e a classificação apresentadas correspondam aos mesmos critérios de cálculo.

#### Informações adicionais

#### Requisitos técnicos e funcionais

1. **Cálculo automático:** registrar os eventos elegíveis e calcular a pontuação correspondente.
2. **Pontuação positiva e negativa:** permitir somar ou subtrair pontos conforme as regras configuradas.
3. **Apuração mensal:** consolidar os resultados do mês anterior e disponibilizá-los no dia 1º.
4. **Apuração por temporada:** calcular a pontuação considerando o período configurado pela escola.
5. **Ordenação:** organizar os atletas conforme a pontuação válida para o período selecionado.
6. **Prevenção de duplicidade:** impedir que um mesmo evento gere pontos repetidos indevidamente.
7. **Histórico e auditoria:** registrar evento, participante, data, pontuação aplicada e regra utilizada.
8. **Preservação dos resultados:** manter os resultados das temporadas encerradas, mesmo após alterações nas configurações.
9. **Configuração de premiações:** permitir definir e apresentar os benefícios oferecidos pela escola.
10. **Consistência entre aplicativos:** garantir que a pontuação exibida no Ritmo Equipes corresponda à apresentada no Ritmo Atletas.
11. **Elegibilidade:** respeitar o status dos atletas e as regras específicas para bolsistas, cancelamentos e outros casos excepcionais.
12. **Desempate:** definir critérios de desempate entre participantes com a mesma pontuação.
13. **Permissões:** garantir que somente usuários autorizados possam configurar temporadas, pontuações e premiações.
14. **Desempenho:** garantir que o cálculo e a exibição do ranking funcionem adequadamente para escolas com diferentes quantidades de atletas.

#### Critérios de aceite

A tarefa será considerada concluída quando:

- Os rankings de Atletas, Usuários e Escolas estiverem implementados conforme suas regras.
- O ranking mensal for calculado e publicado automaticamente no dia 1º de cada mês.
- A escola puder configurar temporadas e selecionar seus meses.
- Alterações no período de uma temporada em andamento não modificarem retroativamente os resultados.
- A pontuação padrão estiver configurada e a personalização por temporada funcionar conforme as permissões definidas.
- A escola puder cadastrar premiações e visualizar sua descrição no ranking.
- O menu Ranking estiver disponível no Ritmo Equipes.
- O Top 3 e a listagem dos demais atletas ativos forem exibidos corretamente.
- O detalhamento individual da pontuação estiver disponível no Ritmo Equipes e no Ritmo Atletas.
- O histórico de temporadas encerradas permanecer armazenado e consultável.
- A pontuação não apresentar duplicidades ou divergências entre os aplicativos.
- Os cálculos forem validados por testes de eventos positivos, negativos, limites, alterações de configuração e encerramento de temporada.

#### Dependências e definições pendentes

Antes do desenvolvimento, validar:

- A regra de participação e premiação dos atletas bolsistas.
- Os critérios de desempate.
- A possibilidade e os limites para personalização da pontuação pela escola.
- O tratamento de atletas que se tornam inativos durante uma temporada.
- O comportamento de eventos registrados após o fechamento mensal.
- A possibilidade de corrigir ou reverter pontuações já lançadas.
- As regras de publicação do resultado mensal e do resultado final da temporada.
- Os critérios de elegibilidade às premiações e a forma de identificar os ganhadores.

## Fontes

- [Ranking de pontuação: Atletas, Usuários e Equipes](https://app.notion.com/p/3fbfe13c365280ef892cde6bc50c9e54?pvs=204)

## Conexões

[[00-Mapa/Indice]] · [[00-Mapa/Pendencias]]
