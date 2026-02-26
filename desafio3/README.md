# 🚀 Desafio 3 — Controle Financeiro

Bem-vindo ao terceiro desafio da Formação Android.

Agora você irá evoluir do armazenamento em memória para um aplicativo com **persistência real de dados**, utilizando banco de dados local.

Este desafio marca a transição para um nível mais profissional de desenvolvimento Android.

---

# 🎯 Objetivo do Desafio

Criar um aplicativo chamado **Controle Financeiro**, permitindo que o usuário:

- Registre receitas e despesas
- Visualize saldo atualizado
- Edite e exclua transações
- Filtre transações por tipo
- Visualize relatórios por categoria
- Armazene todos os dados localmente

⚠️ Importante:
Todos os dados devem ser persistidos no dispositivo utilizando banco de dados local.

---

# 🧠 Tecnologias que você irá praticar

Este desafio foi projetado para consolidar:

- Room Database
- Entities
- Migrations
- Relacionamentos (1-1, 1-N, N-N)
- TypeConverters
- CRUD completo

---

# 📱 Estrutura do Aplicativo

O aplicativo deve conter as seguintes telas:

1️⃣ Splash Screen  
2️⃣ Dashboard (Resumo Financeiro)  
3️⃣ Lista de Transações  
4️⃣ Cadastro / Edição de Transação  
5️⃣ Relatórios  

<img width="1158" height="595" alt="Captura de Tela 2026-02-25 às 21 01 21" src="https://github.com/user-attachments/assets/78f0abaf-f96f-4d3f-b1ec-f0cc4fb50cf2" />


---

# 🟢 Tela 1 — Splash

- Logo
- Nome do app
- Versão
- Layout minimalista

---

# 🟡 Tela 2 — Dashboard (Resumo)

Deve exibir:

- Saldo atual
- Total de receitas
- Total de despesas
- Lista das últimas transações
- Botão para adicionar nova transação

Requisitos técnicos:

- Consultas agregadas no banco (SUM)
- Atualização automática após inserção

---

# 🔵 Tela 3 — Lista de Transações

- RecyclerView com todas as transações
- Filtro por:
  - Todas
  - Receitas
  - Despesas
- Ordenação por data
- Atualização dinâmica após CRUD

---

# 🟣 Tela 4 — Nova Transação / Editar

Campos obrigatórios:

- Nome
- Valor
- Tipo (Receita / Despesa)
- Categoria
- Conta
- Data
- Observação (opcional)

Requisitos técnicos:

- Inserção no banco
- Atualização
- Exclusão
- Uso de DAO
- TypeConverter para datas

---

# 🟤 Tela 5 — Relatórios

- Total por categoria
- Filtro por período
- Lista ou gráfico representando:
  - Categoria
  - Total gasto

Requisitos técnicos:

- Consultas com agrupamento
- Relacionamento entre entidades

---

# 🗂 Estrutura de Banco Esperada

## Entidades sugeridas

### Conta
- id
- nome

### Categoria
- id
- nome
- tipo (Receita ou Despesa)

### Transacao
- id
- descricao
- valor
- tipo
- data
- categoriaId
- contaId

---

# 🔗 Relacionamentos

- 1 Conta → N Transações
- 1 Categoria → N Transações
- Possível extensão futura para N-N (ex: Tags)

---

# 🔄 Migrações

Você deve:

- Criar pelo menos uma Migration
Exemplo:
- Adicionar campo “observacao” na transação
ou
- Adicionar campo “formaPagamento”

---

# 🧩 Regras Técnicas

- CRUD completo funcionando
- Uso de DAO
- Estrutura organizada
- Banco isolado da camada de UI
- Uso de TypeConverter


---

# ⭐ Parte Opcional (Avançado)
- Implementar histórico mensal
- Criar exportação simples em JSON
- Implementar múltiplas contas

---

# 🏁 Resultado Esperado

Ao concluir este desafio você será capaz de:

- Trabalhar com banco de dados local no Android
- Estruturar Entities corretamente
- Criar DAOs profissionais
- Implementar relacionamentos
- Realizar consultas complexas
- Aplicar Migrations
- Desenvolver um app com persistência real
