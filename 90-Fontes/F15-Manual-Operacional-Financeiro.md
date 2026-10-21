---
title: "💸 Manual Operacional – Financeiro"
tipo: "nota"
status: "fonte-consultada"
atualizado_em: "2026-10-20"
fontes: ["https://app.notion.com/p/352fe13c365280acbddbfbd6165da4b8?pvs=204"]
---

# 💸 Manual Operacional – Financeiro

> Registro documental consultado em 2026-10-20. Última edição informada pela fonte: 2026-04-30T20:55:03.790Z. Verificação nativa: unverified.

O conteúdo abaixo preserva as afirmações da fonte; linguagem de requisito não comprova implementação. Vídeos são referências, sem transcrição ou análise audiovisual.

# 1️⃣ Visão Geral da Estrutura Financeira

O módulo financeiro é um **espelho direto da conta Asaas da escola**.

Ele é dividido em:

- **Saldo das Contas**
- **Receitas**
  - Atrasados
  - A Receber
  - Recebidos
- **Despesas**
  - Atrasadas
  - A Pagar
  - Pagas
- Exportação de extrato

---

# 2️⃣ Estrutura de Contas

## 🔹 Conta Digital

- Tudo que entra **via aplicativo**
- PIX gerado pelo app
- Boleto gerado pelo app
- Cartão pelo app
- Links de pagamento gerados no app

👉 É o saldo da **Carteira Ritmo (Asaas)**

---

## 🔹 Conta Banco

- Valores recebidos **fora do app**
- PIX feito diretamente para chave da escola
- Dinheiro recebido na secretaria
- Transferências diretas para o gestor
- Baixas manuais

⚠️ Importante:

Tudo que for registrado manualmente cai na **Conta Banco**.

---

## 🔹 Resultado do Período

Fórmula:

```txt
Receitas – Despesas = Resultado
```

---

# 3️⃣ Sincronização Financeira (Ponto Crítico para Suporte)

## Como identificar falta de sincronização:

Comparar:

- Saldo da Conta Digital (Financeiro)
- Saldo da Carteira Ritmo (Tela Inicial)

Se os valores estiverem diferentes → **Financeiro dessincronizado**

---

## Situações que indicam dessincronização:

- Atleta aparece como pago no perfil, mas consta como atrasado
- Pagamentos “somem” da visualização
- Datas pulando movimentações
- Divergência entre carteira e financeiro

📌 Procedimento N1:

1. Conferir sincronização
2. Se necessário, exportar extrato
3. Validar no admin do atleta
4. Escalar se inconsistência persistir

---

# 4️⃣ Exportação de Extrato

Disponível em:

- Tela principal (3 pontinhos)
- Dentro de Receitas
- Dentro de Despesas

Permite exportar:

- Conta Digital
- Conta Banco
- Ambas
- Período personalizado

📤 O extrato sempre vai para o e-mail logado no app.

---

# 5️⃣ Receitas

## 🔹 Atrasados (Inadimplência)

Mostra:

- Todas as faturas vencidas e não pagas

Permite:

- Editar fatura
- Quitar
- Remover (se aplicável)

Pode filtrar por:

- Categoria (mensalidade, uniforme etc.)
- Nome do atleta

---

## 🔹 A Receber

Mostra:

- Faturas futuras ainda não pagas

Serve como:

- Previsibilidade de entrada

---

## 🔹 Recebidos

Mostra:

- Todos os pagamentos efetivados
- Baixas manuais
- PIX
- Boleto
- Cartão
- Transferências
- Outras fontes de receita

Pode filtrar por:

- Método de pagamento, entre outros 

---

# 6️⃣ Baixa Manual – Procedimento Correto

## 📌 Regra principal:

**NUNCA registrar mensalidade manualmente pelo botão “Adicionar Receita”.**

O procedimento correto para pagamento fora do app é:

1. Ir no perfil do atleta
2. Acessar mensalidade
3. Editar
4. Quitar

Isso:

- Atualiza o status do atleta
- Evita cobrança automática
- Evita duplicidade
- Registra corretamente no financeiro

---

## ❌ O que NÃO fazer:

Adicionar receita manual de mensalidade sem quitar no perfil.

Consequência:

- Atleta continua recebendo cobrança
- Duplica pagamento no financeiro

---

# 7️⃣ Identificação de Pagamentos Fora do App

Quando o responsável paga via:

- Chaves PIX cadastradas na conta Asaas

O sistema registra como:

```txt
Outras fontes de receita
Cobrança gerada automaticamente a partir de PIX recebido
```

IMPORTANTE: Nosso único banco parceiro é o Asaas, comprovantes de qualquer outro Banco são pagamentos por fora do app que deve ser realizado a baixa manual. 

---

## Como identificar que NÃO foi pago pelo app:

- Não aparece descrição da fatura
- Não aparece identificador da escolinha
- ID de transação diferente
- Fatura continua como “Aguardando pagamento” no admin
- Pagamentos para outro banco que não é o Asaas

---

# 8️⃣ Caso Crítico – Pagamento Duplicado via PIX Direto

### Cenário:

Responsável pagou 2 vezes via PIX.

### Procedimento correto:

1. Verificar se os dois valores já constam no financeiro
2. Cancelar as duas faturas correspondentes ( a depender do caso pois existem clientes que desejam o reembolso da fatura duplicada)
3. NÃO registrar manualmente
4. Ajustar conforme combinado com responsável:
   - Estorno
   - Compensar no mês seguinte

📌 Regra:

Se o valor já aparece no financeiro → NÃO registrar manual.

---

# 9️⃣ Despesas

## 🔹 Despesas Automáticas (Conta Digital)

São geradas automaticamente:

- Taxas de PIX
- Assinatura da Ritmo
- Transferências internas
- Saques

---

## 🔹 Despesas Manuais

O gestor pode registrar:

- Luz
- Aluguel
- Salário
- Equipamentos
- Qualquer custo fixo ou variável

---

## 🔹 Parcelamento de Despesas

Permite registrar:

- Despesas fixas mensais
- Contratos anuais
- Parcelamentos

Exemplo:

Aluguel quadra → 12 parcelas → periodicidade mensal

Isso gera previsibilidade.

---

# 🔟 Transferências

Quando o gestor realiza saque:

- Aparece como despesa na Conta Digital
- Aparece como receita na Conta Banco

⚠️ Pode gerar confusão visual.

---

# 1️⃣1️⃣ Movimentações Fora do Contexto da Escola

Se o gestor usar a conta Asaas para fins pessoais:

- Compra no mercado
- Receber PIX de familiar
- Pagar parcela do carro

Tudo aparecerá no financeiro.

Porque:

> O financeiro é espelho da conta Asaas.

---

# 1️⃣2️⃣ Saques da Carteira Ritmo

Disponível na tela inicial:

- PIX → cai na hora
- TED → solicitar até 16h para cair no mesmo dia (normalmente entre 17h e 18h)

---

## Dados de Transferência

Menu → Configurações → Dados de Transferência

- O gestor pode alterar quando quiser
- Sempre validar essa conta em caso de problema de saque

---

# 1️⃣3️⃣ Permissões

- **Financeiro Full** → pode lançar e quitar
- **Financeiro Read** → apenas visualizar

---

# 1️⃣4️⃣ Checklist Operacional N1

Quando gestor abre chamado financeiro:

1. Verificar sincronização
2. Conferir status da fatura no admin
3. Conferir descrição da transação
4. Verificar se pagamento foi pelo app ou direto na chave
5. Conferir duplicidade
6. Validar dados de transferência (se for saque)
7. Exportar extrato se necessário

## Fontes

- [💸 Manual Operacional – Financeiro](https://app.notion.com/p/352fe13c365280acbddbfbd6165da4b8?pvs=204)

## Conexões

[[00-Mapa/Indice]] · [[00-Mapa/Pendencias]]
