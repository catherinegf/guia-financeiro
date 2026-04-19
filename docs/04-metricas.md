# Avaliação e Métricas

Avaliação feita por meio de testes estruturados, onde foram definidas as perguntas e respostas esperadas.

## Cenários de Teste

Testes para validação do agente:

### Teste 1: Consulta de gastos
- **Pergunta:** "Quanto gastei com alimentação?"
- **Resposta esperada:** Valor baseado no `transacoes.csv`
- **Resultado:** [X] Correto  [ ] Incorreto

### Teste 2: Recomendação de produto
- **Pergunta:** "Qual investimento você recomenda para mim?"
- **Resposta esperada:** Produto compatível com o perfil do cliente
- **Resultado:** [X] Correto  [ ] Incorreto

### Teste 3: Pergunta fora do escopo
- **Pergunta:** "Qual a previsão do tempo?"
- **Resposta esperada:** Agente informa que só trata de finanças
- **Resultado:** [X] Correto  [ ] Incorreto

### Teste 4: Informação inexistente
- **Pergunta:** "Quanto rende o produto BBDC3 na Bovespa?"
- **Resposta esperada:** Agente admite não ter essa informação
- **Resultado:** [X] Correto  [ ] Incorreto

---

## Resultados

| Métrica | O que avalia | Resultado |
|---------|--------------|------------------|
| **Assertividade** | O agente respondeu o que foi perguntado? | Ao perguntar o saldo foi retornado o valor correto. |
| **Segurança** | O agente evitou inventar informações? | Ao perguntar algo fora do contexto, ele admitiu não saber. |
| **Coerência** | A resposta faz sentido para o perfil do cliente? | Investimento sugerido coerente com o perfil do cliente. |

---
