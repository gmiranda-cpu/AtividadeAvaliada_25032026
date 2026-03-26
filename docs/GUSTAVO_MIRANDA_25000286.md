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
Essa funcionalidade permite localizar o cliente no sistema antes de realizar a venda, possibilitando vincular a compra ao histórico.
- Cadastrar cliente
  Essa funcionalidade permite registrar novos clientes quando eles ainda não estão cadastrados, facilitando futuras compras e controle.
- Consultar produto
  Essa funcionalidade permite buscar produtos pelo nome, código ou fabricante, agilizando o atendimento no balcão.
- Verificar estoque
  Essa funcionalidade garante que o sistema confira se há quantidade disponível do produto antes da venda, evitando erros.  
- Registrar venda
  Essa é a principal funcionalidade do sistema, permitindo registrar os produtos comprados pelo cliente.
- Registrar venda a prazo
  Essa funcionalidade permite realizar vendas onde o pagamento será feito posteriormente, vinculando ao cliente.
- Validar receita
  Essa funcionalidade permite que o farmacêutico autorize a venda de medicamentos controlados, garantindo segurança e cumprimento das regras.
- Atualizar estoque
  Essa funcionalidade garante que o estoque seja atualizado automaticamente após cada venda, mantendo os dados corretos.
- Emitir comprovante
  Essa funcionalidade permite gerar um comprovante com os dados da venda para o cliente.
- Registrar conta a receber
  Essa funcionalidade permite criar um registro financeiro quando a venda é a prazo, controlando valores e vencimentos.

### O que está fora do MVP

- Cadastro de fornecedores

Essa funcionalidade ficou fora do MVP porque não é essencial para o processo de venda inicial. O foco foi no atendimento ao cliente, então o cadastro de fornecedores pode ser implementado depois.

- Registro de compras

O registro de compras não foi incluído no MVP porque está mais relacionado ao setor administrativo. Como o objetivo foi focar na venda, essa parte pode ser adicionada em versões futuras.

- Contas a pagar

Essa funcionalidade envolve o controle financeiro interno da empresa, que não é necessário para o funcionamento básico da venda. Por isso, ficou fora do MVP.

- Relatórios completos

Relatórios mais detalhados e estratégicos não foram incluídos porque o MVP prioriza apenas o funcionamento básico do sistema. Esses relatórios podem ser desenvolvidos posteriormente.

- Gerenciamento de usuários

A parte de administrar usuários e permissões completas foi deixada de fora para simplificar o sistema inicial, já que o foco foi apenas nas funcionalidades principais de atendimento.

### Por que fiz essas escolhas
Escolhi focar no processo de venda por ser a parte mais importante do sistema, envolvendo atendimento, estoque e financeiro, entregando valor rápido e reduzindo erros.

---

## 2. Regras de Negócio


RN01 — Produtos sem estoque não podem ser vendidos  

Essa regra garante que o sistema não permita vender produtos que não estão disponíveis no estoque, evitando erros e problemas com clientes.

RN02 — Medicamentos controlados exigem validação de receita 

Essa regra define que alguns medicamentos só podem ser vendidos com autorização do farmacêutico, garantindo o cumprimento das normas de saúde.

RN03 — Venda a prazo gera conta a receber automaticamente

Essa regra faz com que toda venda a prazo seja registrada no financeiro, criando automaticamente uma conta a receber para controle do pagamento.

RN04 — Estoque é atualizado automaticamente após venda 

Essa regra garante que, após cada venda, o estoque seja atualizado sem precisar de intervenção manual, evitando divergências.

RN05 — Cliente deve estar cadastrado para compra a prazo

Essa regra exige que o cliente esteja registrado no sistema para poder comprar a prazo, permitindo controle e histórico de pagamentos.

---

## 3. Requisitos Funcionais


RF01 — Consultar produtos  

Esse requisito permite que o atendente busque produtos pelo nome, código ou fabricante, facilitando o atendimento ao cliente.

RF02 — Identificar cliente 

Esse requisito permite localizar o cliente no sistema para vincular a compra ao seu histórico.

RF03 — Cadastrar cliente  

Esse requisito permite cadastrar novos clientes quando eles ainda não estão registrados no sistema.

RF04 — Registrar venda  

Esse requisito permite registrar a venda de produtos, sendo a principal função do sistema.

RF05 — Verificar estoque  

Esse requisito garante que o sistema confira se há quantidade suficiente do produto antes de realizar a venda.

RF06 — Registrar venda a prazo  

Esse requisito permite registrar vendas onde o pagamento será feito depois, vinculando ao cliente.

RF07 — Atualizar estoque automaticamente  

Esse requisito garante que o estoque seja atualizado após cada venda, sem necessidade de ação manual.

RF08 — Emitir comprovante  

Esse requisito permite gerar um comprovante com os dados da venda para o cliente.

RF09 — Validar receita  

Esse requisito permite que o farmacêutico valide receitas médicas para liberar a venda de medicamentos controlados.

RF10 — Gerar conta a receber 

Esse requisito permite criar registros financeiros quando a venda é feita a prazo, controlando valores e vencimentos.

---

## 4. Requisitos Não Funcionais


RNF01 — Sistema deve ter login e controle de acesso  

Esse requisito garante que apenas usuários autorizados possam acessar o sistema, com diferentes permissões de acordo com o tipo de usuário (atendente, gerente, etc.), aumentando a segurança.

RNF02 — Resposta em até 3 segundos  

Esse requisito define que o sistema deve ser rápido, respondendo às ações do usuário em até 3 segundos, garantindo um atendimento ágil no dia a dia.

RNF03 — Garantir integridade dos dados 

Esse requisito garante que as informações do sistema, como vendas e estoque, sejam armazenadas corretamente, sem erros ou perdas de dados.

RNF04 — Interface simples e fácil de usar  

Esse requisito define que o sistema deve ser intuitivo, facilitando o uso pelos funcionários, mesmo sem muito conhecimento técnico.

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

- UC11 — Diagrama Geral
  
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
