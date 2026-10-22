---
title: "Protótipo — Configuração do ranking de equipes"
tipo: "nota"
status: "prototipo-validado"
atualizado_em: "2026-10-22"
fontes: ["Tarefa (2).xlsx", "recording-2026-10-21-20-33-26.webm", "Decisões do usuário — 2026-10-22"]
---

# Protótipo — Configuração do ranking de equipes

Primeira etapa do protótipo do módulo **Ranking** na plataforma Ritmo Equipes. O menu Ranking expõe os submenus **Configuração**, **Usuários**, **Atletas** e **Visualização**; nesta entrega, somente a configuração de **Equipes** foi detalhada. A visualização do ranking é uma etapa posterior.

## Escopo implementado no protótipo

- Navegação lateral com o módulo Ranking e seus submenus.
- Lista de temporadas por ano, com criação, seleção e edição da temporada em configuração.
- Seleção de ano para configurar períodos futuros, além de nome e meses que compõem a vigência de cada temporada.
- Exclusividade de meses por ano: um mês usado por uma temporada fica indisponível para outra temporada do mesmo ano.
- Configuração opcional de premiação: escolha inicial entre conceder ou não; quando habilitada, há abrangência para Brasil inteiro ou por estado e descrição correspondente.
- Fluxo progressivo da premiação: depois de selecionar “Sim”, a escola escolhe Brasil inteiro ou por estado; somente os campos da abrangência selecionada são exibidos.
- Navegação lateral simplificada com os submenus Conf. Equipes, Conf. Usuário Equipe e Conf. Atletas; o cabeçalho orienta a configurar as temporadas do ano.
- Grupos expansíveis de critérios, pontuação editável e ativação individual.
- Ações locais de descartar e salvar, com confirmação visual.
- Critérios e valores da aba Escola da fonte vigente [[90-Fontes/F21-Planilha-de-pontuacao-atualizada]].

| Grupo | Critérios exibidos | Fonte |
|---|---:|---|
| Pagamentos | 8 | Escola!B2:D10 |
| Chamada | 3 | Escola!B11:D13 |
| Grupos | 2 | Escola!B14:D15 |
| Convocação | 2 | Escola!B16:D17 |
| Notas públicas com descrição | 1 | Escola!B18:E18 |
| Mensagens | 2 | Escola!B19:D20 |
| Galeria | 1 | Escola!B21:D21 |

## Limites conhecidos

- O rótulo de temporada, os meses e as descrições de premiação são dados demonstrativos de interface; não determinam uma temporada ativa de produção.
- O protótipo não implementa persistência, autorização, apuração, auditoria ou aplicação efetiva de alterações de pontos.
- A interface é demonstrativa: os controles de vigência e premiação não representam persistência ou validação de produção.
- A regra de adimplência em “Pagamento em dia com a Ritmo” permanece sem gatilho definido na planilha.
- Posições premiadas, elegibilidade, desempate, periodicidade e entrega das premiações não foram definidos nesta decisão.
- Os submenus de Usuários, Atletas e Visualização estão previstos como próximas etapas e não devem ser interpretados como telas entregues.

## Referências

- Critérios: [[03-Rankings/Criterios/Escola]].
- Requisitos de configuração por temporada e preservação de histórico: [[03-Rankings/Configuracao-e-alteracao-da-pontuacao]] e [[03-Rankings/Configuracao-das-temporadas-pela-escola]].
- Referência visual: [[90-Fontes/F22-Video-referencia-plataforma-ranking]].
- Vigência e premiação: [[90-Fontes/F23-Configuracao-de-vigencia-e-premiacao]].
- Múltiplas temporadas no ano: [[90-Fontes/F24-Multiplas-temporadas-no-ano]].
- Exclusividade anual e premiação opcional: [[90-Fontes/F25-Exclusividade-de-meses-e-premiacao-opcional]].
- Ajustes de interface e fluxo: [[90-Fontes/F26-Ajustes-de-interface-e-fluxo-da-premiacao]].

## Conexões

[[03-Rankings/Visao-geral-ranking]] · [[03-Rankings/Ranking-de-Escolas]] · [[03-Rankings/Criterios/Escola]] · [[03-Rankings/Configuracao-das-temporadas-pela-escola]] · [[03-Rankings/Periodicidade-e-temporadas]] · [[03-Rankings/Premiacoes]] · [[03-Rankings/Lacunas-da-planilha]]
