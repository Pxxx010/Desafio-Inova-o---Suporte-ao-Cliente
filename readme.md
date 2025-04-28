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

### Product Backlog (Tarefas Técnicas)
1. **Estrutura de Dados (Dia 1)**
   - Criar modelo de dados para chamados (schemas)
   - Implementar banco de dados SQLite local
   - Desenvolver API REST básica para CRUD de chamados

2. **Frontend - Parte 1 (Dia 2)**
   - Implementar componente de listagem de chamados
   - Desenvolver formulário de cadastro com validações
   - Integrar com API para exibição de dados em tempo real

3. **Frontend - Parte 2 (Dia 3)**
   - Implementar função "Marcar como Resolvido" com atualização de status
   - Adicionar sistema de ordenação por data de criação
   - Desenvolver filtros básicos (chamados abertos/resolvidos)
   - Implementar responsividade para uso em dispositivos móveis

### Planejamento dos 5 dias

| Dia | Atividades |
|-----|------------|
| 1 | Definir informações principais e implementar estrutura de dados e API básica. |
| 2 | Desenvolver componentes frontend principais e integração com API. |
| 3 | Finalizar implementação de funcionalidades e adicionar responsividade. |
| 4 | Realizar testes de integração e correção de bugs. |
| 5 | Apresentar o protótipo funcional e coletar feedback. |

## Protótipo de Solução

### Telas a serem implementadas no Figma

#### 1. Tela Inicial: Lista de Chamados
* Título: "Chamados em Aberto"
* Lista de cartões com:
   * Nome do Cliente
   * Telefone
   * Descrição do Problema
   * Prioridade (Baixa, Média, Alta) com cor ou ícone indicativo
   * Data/Hora de abertura
   * Botão **[Marcar como Resolvido]**

#### 2. Tela de Cadastro de Chamado
* Título: "Novo Chamado"
* Campos para preencher:
   * Nome do Cliente
   * Telefone
   * Problema
   * Prioridade (Seleção: Baixa, Média, Alta)
* Botão **[Salvar Chamado]**

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