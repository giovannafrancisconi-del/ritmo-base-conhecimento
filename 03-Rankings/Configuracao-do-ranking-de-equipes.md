---
title: "Protótipo — Configuração do ranking de equipes"
tipo: "nota"
status: "prototipo-validado"
atualizado_em: "2026-10-21"
fontes: ["Tarefa (2).xlsx", "recording-2026-10-21-20-33-26.webm"]
---

# Protótipo — Configuração do ranking de equipes

Primeira etapa do protótipo do módulo **Ranking** na plataforma Ritmo Equipes. O menu Ranking expõe os submenus **Configuração**, **Usuários**, **Atletas** e **Visualização**; nesta entrega, somente a configuração de **Equipes** foi detalhada. A visualização do ranking é uma etapa posterior.

## Escopo implementado no protótipo

- Navegação lateral com o módulo Ranking e seus submenus.
- Tela de Configuração > Equipes com seletor de temporada, vigência e aviso de não retroatividade.
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

- O rótulo de temporada e a vigência exibidos são dados demonstrativos de interface; não determinam uma temporada ativa de produção.
- O protótipo não implementa persistência, autorização, apuração, auditoria ou aplicação efetiva de alterações de pontos.
- A regra de adimplência em “Pagamento em dia com a Ritmo” permanece sem gatilho definido na planilha.
- Os submenus de Usuários, Atletas e Visualização estão previstos como próximas etapas e não devem ser interpretados como telas entregues.

## Referências

- Critérios: [[03-Rankings/Criterios/Escola]].
- Requisitos de configuração por temporada e preservação de histórico: [[03-Rankings/Configuracao-e-alteracao-da-pontuacao]] e [[03-Rankings/Configuracao-das-temporadas-pela-escola]].
- Referência visual: [[90-Fontes/F22-Video-referencia-plataforma-ranking]].

## Conexões

[[03-Rankings/Visao-geral-ranking]] · [[03-Rankings/Ranking-de-Escolas]] · [[03-Rankings/Criterios/Escola]] · [[03-Rankings/Lacunas-da-planilha]]
