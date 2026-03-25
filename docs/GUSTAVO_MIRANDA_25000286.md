# Avaliação — Engenharia de Software
## Sistema Integrado de Gestão de Farmácia — MVP Definido pelo Estudante

**Aluno:** Gustavo Miranda Rodrigues  
**RA:** 25000286  
**Data:** 25/03/2026 

---

## 1. Definição do MVP

Meu MVP cobre o processo de venda de produtos da farmácia desde a identificação ou cadastro do cliente até a emissão do comprovante, incluindo consulta de produto, verificação de estoque, validação de receita quando necessário, atualização automática do estoque e geração de conta a receber em vendas a prazo.

### O que está dentro do MVP
- Identificar cliente  
- Cadastrar cliente  
- Consultar produto  
- Verificar estoque  
- Registrar venda  
- Registrar venda a prazo  
- Validar receita  
- Atualizar estoque  
- Emitir comprovante  
- Registrar conta a receber  

### O que está fora do MVP
- Cadastro de fornecedores  
- Registro de compras  
- Contas a pagar  
- Relatórios completos  
- Gerenciamento de usuários  

### Por que fiz essas escolhas
Escolhi focar no processo de venda por ser a parte mais importante do sistema, envolvendo atendimento, estoque e financeiro, entregando valor rápido e reduzindo erros.

---

## 2. Regras de Negócio

RN01 — Produtos sem estoque não podem ser vendidos  
RN02 — Medicamentos controlados exigem validação de receita  
RN03 — Venda a prazo gera conta a receber automaticamente  
RN04 — Estoque é atualizado automaticamente após venda  
RN05 — Cliente deve estar cadastrado para compra a prazo  

---

## 3. Requisitos Funcionais

RF01 — Consultar produtos  
RF02 — Identificar cliente  
RF03 — Cadastrar cliente  
RF04 — Registrar venda  
RF05 — Verificar estoque  
RF06 — Registrar venda a prazo  
RF07 — Atualizar estoque automaticamente  
RF08 — Emitir comprovante  
RF09 — Validar receita  
RF10 — Gerar conta a receber  

---

## 4. Requisitos Não Funcionais

RNF01 — Sistema deve ter login e controle de acesso  
RNF02 — Resposta em até 3 segundos  
RNF03 — Garantir integridade dos dados  
RNF04 — Interface simples e fácil de usar  

---

## 5. Casos de Uso

- UC01 — Login  
- UC02 — Consultar Produto  
- UC03 — Identificar Cliente  
- UC04 — Cadastrar Cliente  
- UC05 — Registrar Venda  
- UC06 — Validar Receita  
- UC07 — Venda a Prazo  
- UC08 — Atualizar Estoque  
- UC09 — Emitir Comprovante  
- UC10 — Gerar Conta a Receber  

---

## 6. Documentação dos Casos de Uso

### UC05 — Registrar Venda

**Ator:** Atendente  

**Descrição:** Registrar venda de produtos  

**Pré-condições:** Produto cadastrado  

**Pós-condições:** Venda registrada e estoque atualizado  

### Fluxo Principal
1. Identificar cliente  
2. Consultar produto  
3. Informar quantidade  
4. Verificar estoque  
5. Registrar venda  
6. Atualizar estoque  
7. Emitir comprovante  

### Fluxos Alternativos

FA01 — Estoque insuficiente  
Sistema informa erro  

FA02 — Produto controlado  
Solicita validação da receita  

### Relacionamentos
Include: Identificar Cliente, Consultar Produto  
Extend: Validar Receita, Venda a Prazo  
