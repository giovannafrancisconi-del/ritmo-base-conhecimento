---
title: "Manutenção e integração de documentos"
tipo: "nota"
status: "documentacao-organizacional"
atualizado_em: "2026-10-20"
fontes: []
---

# Manutenção e integração de documentos

Este procedimento organiza a base; não constitui regra de negócio do Ritmo. Atualizações são executadas quando novas fontes ou alterações forem informadas e disponibilizadas nesta conversa. Não há monitoramento automático dos links.

## Integração

1. Identificar o arquivo, tipo, origem, data e versão; preservar o original em `06-Midias/Originais/` quando fornecido.
2. Extrair o texto de documentos e PDFs; para imagens, registrar a leitura e eventuais incertezas; para áudio e vídeo, registrar transcrição, trechos e limitações. Não declarar análise de uma mídia apenas por existir um link.
3. Relacionar a evidência às notas existentes e criar uma nota somente quando houver um novo conceito ou processo.
4. Separar procedimentos descritos, requisitos futuros e decisões pendentes. Não resolver conflitos sem validação.
5. Atualizar apenas as notas afetadas, suas referências, o mapa, o grafo e o registro de alterações.
6. Validar wikilinks, integridade das fontes e ausência de decisões presumidas.

## Atualizações incrementais

- Consultar a versão atual da fonte informada e comparar seu conteúdo com o registro anterior.
- Usar o manifesto de fontes e as referências de cada nota para identificar dependências.
- Manter os caminhos existentes sempre que o conceito for o mesmo.
- Registrar conteúdo alterado, origem, notas afetadas e perguntas em aberto.
- Se a fonte estiver inacessível, sinalizar a limitação e pedir o conteúdo; não apagar fatos anteriores nem tratá-los como reconfirmados.

## Convenções

- Markdown UTF-8 e wikilinks com caminho relativo à raiz do cofre.
- Metadados YAML: título, tipo, status, data de atualização e URLs das fontes.
- `procedimento-documentado`: comportamento descrito em guia, sem teste do aplicativo.
- `requisito-documentado`: comportamento solicitado pela especificação.
- `validacao-pendente`: informação não confirmada.
- `mapeamento-documental`: organização de relações encontradas nas fontes.
- Alteração de data da fonte não prova entrega em produção.
- Os registros JSON preservam o retorno consultado; as notas de fontes normalizam marcação para leitura.

## Conexões

[[00-Mapa/Fontes-e-cobertura]] · [[00-Mapa/Pendencias]] · [[05-Governanca/Registro-de-alteracoes]]
