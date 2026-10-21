---
title: "Avaliação do evento da convocação"
tipo: "nota"
status: "requisito-documentado"
atualizado_em: "2026-10-21"
fontes: ["https://app.notion.com/p/3fffe13c3652804db179d730f13783b5?pvs=204"]
---

# Avaliação do evento da convocação

## Fluxo documentado

1. Após a data do evento, os atletas que confirmaram a convocação devem receber uma notificação no dia seguinte.
2. A notificação é intitulada **Avaliação de Competição** e informa que o atleta compareceu à convocação, com o nome da competição/convocação.
3. A avaliação segue o conceito da avaliação de treino.
4. A conclusão da avaliação deve gerar pontuação no ranking.

A planilha de critérios prevê **+20 pontos** para “Avaliação do Evento/Convocação” quando o atleta avalia o evento após receber a notificação no dia do evento, e marca esta funcionalidade como “Desenvolver funcionalidade”. Há uma divergência de momento do disparo entre a página de melhoria e a planilha; ela está registrada em [[03-Rankings/Lacunas-da-avaliacao-da-convocacao]].

## Avaliação de 5 estrelas

| Critério | Descrição documentada |
|---|---|
| Arbitragem | Postura, imparcialidade e condução da partida |
| Pontualidade | Cumprimento dos horários da tabela de jogos |
| Estrutura | Qualidade das quadras, iluminação, redes e espaço |
| Fair Play | Respeito e espírito esportivo dentro e fora de quadra |
| Organização | Divulgação de resultados, tabelas e suporte |
| Saúde | Suporte e atendimento de emergências médicas, primeiros socorros e hidratação |
| Nível do Jogo | Equilíbrio técnico e competitividade da partida |
| Comunicação | Condução das anotações e placar |

## Avaliação de 4 estrelas ou menos

Os subitens documentados são:

| Grupo | Subitens |
|---|---|
| Arbitragem | Postura e comunicação; imparcialidade; condução da partida; condução das anotações e placar |
| Evento / Estrutura | Atrasos nos horários da tabela de jogos; qualidade das quadras, local e equipamentos; segurança, acessibilidade e infraestrutura |
| Suporte / Atendimento | Primeiros socorros; atendimento médico de emergência; hidratação, higiene e sanitização |
| Organização | Divulgação de resultados, tabelas e suporte; divulgação de partidas, horários e equipes; acesso a informações e localizações |

## Regra de apresentação confirmada

- **5 estrelas:** apresentar somente as tags de aspectos positivos; não apresentar tópicos nem subitens.
- **1 a 4 estrelas:** ocultar as tags e apresentar os tópicos expansíveis, com seleção dos respectivos subitens como motivos.

A regra foi confirmada no comentário de revisão e foi aplicada ao protótipo. Ela não decide as lacunas de negócio registradas nesta base.

## Protótipo visual

O protótipo móvel navegável representa: escolha de 1 a 5 estrelas; os oito critérios de 5 estrelas; exibição dos subitens para notas até 4; e confirmação de envio.

- [Abrir protótipo privado](https://ritmo-avaliacao-convocacao-20261020.giovanafrancisconi.chatgpt.site)
- O protótipo não confirma implementação nem define regras de pontuação fora das fontes.

## Evidências ainda necessárias

- Modelo e conteúdo final da notificação.
- Regras de envio, reenvio, expiração e resposta única.
- Critérios de elegibilidade baseados na presença efetiva no evento.
- Persistência, auditoria e tratamento de edição ou exclusão da avaliação.

A página de origem contém referências visuais de imagens no Notion.

## Conexões

[[03-Rankings/Criterios/Atleta]] · [[03-Rankings/Lacunas-da-avaliacao-da-convocacao]] · [[01-Atletas/Participacao-em-convocacao]] · [[90-Fontes/F17-Avaliacao-do-evento-da-convocacao]] · [[90-Fontes/F19-Comentario-1-prototipo-avaliacao]]

## Referência visual implementada

O vídeo da avaliação de treino foi integrado como referência da interface. O protótipo agora reproduz o padrão observado de Feed → modal inferior → estrelas → categorias ou motivos → envio, adaptado ao conteúdo da competição.

- Referência: [[90-Fontes/F18-Video-avaliacao-de-treino]]
- A adaptação visual não resolve as lacunas AC01 a AC08 nem substitui a especificação de negócio.
