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
  
<img width="369" height="282" alt="image" src="https://github.com/user-attachments/assets/e83a437c-532b-4323-a979-2bcfd55715af" />

- UC02 — Consultar Produto 

<img width="392" height="297" alt="image" src="https://github.com/user-attachments/assets/7011f6d0-06b3-424c-bae0-d0d9209a575b" />

- UC03 — Identificar Cliente

<img width="380" height="282" alt="image" src="https://github.com/user-attachments/assets/882dc1d3-d594-4ea2-9998-b82632ce1ea5" />

- UC04 — Cadastrar Cliente

<img width="398" height="337" alt="image" src="https://github.com/user-attachments/assets/9980e057-45eb-4959-a01f-301f8dd40fdd" />

- UC05 — Registrar Venda

<img width="490" height="929" alt="image" src="https://github.com/user-attachments/assets/cf5960a6-ba41-4644-8154-1062c5216243" />

- UC06 — Validar Receita

<img width="251" height="282" alt="image" src="https://github.com/user-attachments/assets/afe5e95c-c2ae-419c-8c45-2192c15b8edc" />

- UC07 — Venda a Prazo

<img width="352" height="392" alt="image" src="https://github.com/user-attachments/assets/37458342-2b73-4ea2-b2ff-aaf1eebbc24f" />

- UC08 — Atualizar Estoque

  <img width="245" height="451" alt="image" src="https://github.com/user-attachments/assets/45b09eee-d249-4579-8454-9591960326c6" />

- UC09 — Emitir Comprovante

  <img width="212" height="248" alt="image" src="https://github.com/user-attachments/assets/1c56f756-9d97-40b8-8007-7a1aaf7e4126" />

- UC10 — Gerar Conta a Receber
  <img width="223" height="358" alt="image" src="https://github.com/user-attachments/assets/19c85ac3-f959-4a86-8988-c723427d9d4b" />


  <img width="680" height="485" alt="image" src="https://github.com/user-attachments/assets/5459c643-1b3b-4735-a8c4-dbebce69ffa5" />


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
