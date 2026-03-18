# 📄 Product Requirements Document (PRD) - MR SNKRS

## 1. Visão Geral e Objetivo

O **MR SNKRS** é uma aplicação web didática que simula as funcionalidades de um e-commerce moderno focado na venda de sneakers.

O sistema permite que usuários naveguem por um catálogo de produtos, adicionem itens ao carrinho e realizem a finalização de compras por meio de um formulário com validações.

**Diferencial do projeto:** A aplicação tem como foco a construção de uma interface moderna, responsiva e interativa, integrando APIs para manipulação dinâmica de dados e proporcionando uma experiência próxima a lojas virtuais reais.

---

## 2. Atores do Sistema

- **Visitante:** Usuário que acessa o site e navega pelos produtos disponíveis.
- **Cliente:** Usuário que adiciona produtos ao carrinho e realiza a finalização da compra.
- **Sistema (MR SNKRS):** Responsável por gerenciar os produtos, processar pedidos e integrar APIs para fornecer dados dinâmicos.

---

## 3. Histórias de Usuário e Escopo

Abaixo estão as funcionalidades principais do MVP (Minimum Viable Product), escritas sob a perspectiva do usuário final.

---

### 🛍️ Épico 1: Catálogo de Produtos

- **US01 - Visualizar Produtos:** Como um Visitante, quero visualizar uma lista de produtos disponíveis para que eu possa conhecer os itens da loja.
  - _Critérios de Aceitação:_ Os produtos devem ser exibidos em formato de cards com imagem, nome e preço.

- **US02 - Visualizar Detalhes do Produto:** Como um Visitante, quero visualizar mais informações sobre um produto para decidir se desejo comprá-lo.
  - _Critérios de Aceitação:_ Deve exibir imagem ampliada, descrição e preço.

---

### 🛒 Épico 2: Carrinho de Compras

- **US03 - Adicionar Produto ao Carrinho:** Como um Cliente, quero adicionar produtos ao carrinho para comprá-los posteriormente.
  - _Critérios de Aceitação:_ O produto deve ser armazenado no localStorage e refletido no carrinho.

- **US04 - Visualizar Carrinho:** Como um Cliente, quero visualizar os itens adicionados ao carrinho para revisar minha compra.
  - _Critérios de Aceitação:_ Deve listar produtos, quantidade e valor total.

- **US05 - Atualizar Carrinho:** Como um Cliente, quero alterar a quantidade ou remover produtos do carrinho.
  - _Critérios de Aceitação:_ O total deve ser recalculado automaticamente.

---

### 💳 Épico 3: Checkout

- **US06 - Finalizar Compra:** Como um Cliente, quero preencher um formulário com meus dados para concluir a compra.
  - _Critérios de Aceitação:_ Todos os campos devem ser obrigatórios e validados (nome, email, telefone, CEP).

- **US07 - Preenchimento Automático de Endereço:** Como um Cliente, quero inserir meu CEP e ter o endereço preenchido automaticamente.
  - _Critérios de Aceitação:_ O sistema deve consumir uma API externa para buscar os dados do endereço.

---

### 🌐 Épico 4: Integração com APIs

- **US08 - Listar Produtos Dinamicamente:** Como sistema, quero buscar produtos de uma API fake para exibir no catálogo.
  - _Critérios de Aceitação:_ Os dados devem ser carregados dinamicamente na interface.

- **US09 - Registrar Pedido:** Como sistema, quero enviar os dados do pedido para uma API fake para simular persistência.
  - _Critérios de Aceitação:_ O pedido deve ser salvo com sucesso e o carrinho limpo após a compra.

---

### 💾 Épico 5: Persistência Local

- **US10 - Manter Carrinho:** Como um Cliente, quero que os itens do carrinho sejam mantidos mesmo ao atualizar a página.
  - _Critérios de Aceitação:_ Os dados devem ser armazenados no localStorage.

---
