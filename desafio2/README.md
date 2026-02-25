# 🚀 Desafio 2 — Aplicativo de Eventos

Bem-vindo ao segundo desafio da Formação Android.

Agora você irá evoluir do mundo das telas simples para trabalhar com **listas dinâmicas**, manipulação de dados em memória e organização de informações em tempo real.

Este desafio consolida sua base em UI e introduz estruturas fundamentais para qualquer app moderno.

---

# 🎯 Objetivo do Desafio

Criar um aplicativo chamado **Eventos**, contendo:

- Splash Screen
- Tela principal com lista de eventos
- Funcionalidade de busca
- Funcionalidade de ordenação
- Atualização dinâmica da lista
- Navegação para tela de detalhe do evento

⚠️ Importante:
- Não utilizar API
- Não utilizar banco de dados
- Todos os dados devem estar em memória

---

# 🧠 Tecnologias que você irá praticar

Este desafio foi projetado para consolidar os seguintes conceitos:

- RecyclerView
- Adapter
- ListView
- CardView
- LayoutManager
- Atualização dinâmica de listas
- Kotlin Collections (List, Set, Map)
- Funções lambda
- Funções de escopo
- Data Classes
- Manipulação de dados dinâmicos

---

# 📱 Estrutura do Aplicativo

O aplicativo deve conter 3 partes principais.

<img width="796" height="763" alt="Captura de Tela 2026-02-25 às 18 50 38" src="https://github.com/user-attachments/assets/c2c97769-1f73-4fd6-bae7-4112bc59620a" />


---

# 🟢 Tela 1 — Splash Screen

Objetivo:
Apresentar o aplicativo ao usuário.

Elementos esperados:

- Ícone central
- Nome do app: “Eventos”
- Subtítulo
- Versão do aplicativo
- Layout minimalista

Tecnologias aplicadas:
- Activity
- Organização de layout
- ConstraintLayout
- Temas e estilos

---

# 🟡 Tela 2 — Lista de Eventos

Objetivo:
Exibir eventos dinamicamente utilizando RecyclerView.

## 🔹 Estrutura visual

Cada item deve conter:

- Categoria (Chip ou badge)
- Nome do evento
- Data e hora
- Local
- Indicador visual (ex: Hoje / Esta semana)
- Ícone de navegação

Utilizar:
- CardView
- LayoutManager vertical

---

# 🔎 Funcionalidade de Busca

Criar campo de busca que:

- Filtre eventos pelo nome
- Filtre por categoria
- Atualize a lista dinamicamente

Aplicar:
- `filter`
- Funções lambda
- Atualização do adapter

---

# ↕ Funcionalidade de Ordenação

Permitir ordenar por:

- Nome (A-Z)
- Data (mais próxima)
- Categoria

Aplicar:
- `sortedBy`
- `sortedByDescending`
- Manipulação da lista original

---

## 🧩 Regras Técnicas

- Lista inicial com no mínimo 6 eventos mockados  
- A lista deve ser mutável  
- Utilizar boas práticas no Adapter  
- Código organizado  
- Separação clara de responsabilidades  

---

## ⭐ Parte Opcional (Avançado)

- Implementar agrupamento por categoria  
- Implementar contagem dinâmica de eventos  
- Implementar estado vazio (Nenhum evento encontrado)  
- Criar versão alternativa usando ListView  

---

## 🏁 Resultado Esperado

Ao concluir este desafio você será capaz de:

- Criar listas dinâmicas com RecyclerView  
- Criar e organizar um Adapter  
- Manipular coleções Kotlin  
- Filtrar e ordenar dados    

Você agora domina a base de qualquer aplicativo moderno baseado em listas.
