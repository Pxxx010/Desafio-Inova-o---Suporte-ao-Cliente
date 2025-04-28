# Sistema de Suporte ao Cliente para Provedores Pequenos

Este repositório contém o design e o plano de implementação de um sistema simples de registro de chamados, desenvolvido especificamente para pequenos provedores de internet.

## Índice
- [Mapa de Empatia](#mapa-de-empatia)
- [Sprint Planning](#sprint-planning)
- [Protótipo de Solução](#protótipo-de-solução)
- [Teste e Feedback](#teste-e-feedback)

## Mapa de Empatia

![Mapa de Empatia](Mapa%20de%20Empatia.png)

O seguinte mapa de empatia foi criado para entender melhor as experiências diárias e os desafios da equipe de suporte em provedores pequenos:

| Área | Respostas |
|------|-----------|
| O que vê? | Poucos funcionários, muitos clientes chamando no WhatsApp e telefone. |
| O que ouve? | Reclamações de clientes impacientes, colegas sobrecarregados. |
| O que pensa e sente? | Cansaço, pressão, vontade de atender bem mas falta estrutura. |
| O que fala e faz? | Pede desculpas, tenta atender todos, corre para resolver o que consegue. |
| Quais são suas dores? | Multitarefa extrema, falta de organização, estresse. |
| Quais são seus ganhos? | Satisfação ao resolver rápido, reconhecimento de clientes e da empresa. |

## Sprint Planning

### Objetivo da Sprint
**Criar um sistema simples para registrar e organizar chamados de clientes no provedor pequeno.**


## Product Backlog (Tarefas Técnicas)

![Product Backlog](Product%20Backlog.png)

### 1. Estrutura de Dados
- Criar modelo de dados para chamados (schemas)
- Implementar banco de dados SQLite local

### 2. API Backend
- Desenvolver API REST básica para CRUD de chamados
- Implementar endpoints para filtros e ordenação

### 3. Frontend - Listagem
- Implementar componente de listagem de chamados
- Integrar com API para exibição em tempo real

### 4. Frontend - Formulários
- Desenvolver formulário de cadastro com validações
- Criar tela de edição de chamados existentes

### 5. Gestão de Status
- Implementar função "Marcar como Resolvido" 
- Adicionar transições de status com histórico

### 6. Filtros e Ordenação
- Desenvolver filtros avançados (por status, data, prioridade)
- Implementar sistema de ordenação customizável

### 7. Responsividade e UX
- Adaptar interface para dispositivos móveis
- Implementar feedback visual (notificações, animações)

## Sprint: **05/05/2025 a 09/05/2025**

### Planejamento dos 5 dias

| Dia | Atividades |
|-----|------------|
| 1 | Desenvolver estrutura de dados e configurar banco SQLite |
| 2 | Implementar API backend e iniciar componente de listagem |
| 3 | Finalizar frontend de listagem e desenvolver formulários |
| 4 | Implementar gestão de status, filtros e ordenação |
| 5 | Finalizar responsividade, realizar testes e preparar demonstração 
## Protótipo de Solução

### Telas a serem implementadas no Figma

#### 1. Tela Login
* Título: "W3cSys - Login"
* Campos:
   * Email/Usuário
   * Senha

Botão **[Entrar]**

#### 2. Tela Inicial: Lista de Chamados
* Título: "Chamados em Aberto"
* Lista de cartões com:
   * Nome do Cliente
   * Telefone
   * Descrição do Problema
   * Prioridade (Baixa, Média, Alta) com cor ou ícone indicativo
   * Data/Hora de abertura
   * Botão **[Marcar como Resolvido]**
* Cards indicadores:
  * Chamados Abertos: 0 (ícone azul)
  * Chamados Fechados: 2 (ícone verde)
  * Chamados > 3 dias: 0 (ícone vermelho)
* Filtros:
  * Dropdown de status "Todos"
  * Seletor de datas
* Abas de navegação:
  * Todos (2)
  * Abertos (0)
  * Fechados (2)

#### 3. Tela de Cadastro de Chamado
* Título: "Novo Chamado"
* Campos para preencher:
   * Nome do Cliente
   * Login do Cliente
   * Telefone
   * Descrição do Problema
   * Prioridade (Seleção: Baixa, Média, Alta)
* Botão **[Criar Chamado]**

### Fluxo de Uso (roteiro)
1. Atendente abre a tela de "Chamados em Aberto".
2. Clica em "Novo Chamado" para adicionar um novo atendimento.
3. Preenche nome, telefone, descrição do problema e prioridade.
4. Salva o chamado.
5. O chamado aparece na lista, organizado por prioridade (alta primeiro) e depois por ordem de abertura.
6. Quando resolver o problema, clica em "Marcar como Resolvido".

## Teste e Feedback

### Feedback Simulado
* **O que funcionou bem:** "....."
* **O que pode melhorar:** "....."