# 🚀 Desafio 5 — Tech Events (MVVM do Zero)

Bem-vindo ao quinto desafio da Formação Android.

Neste desafio você vai criar um aplicativo **do zero**, aplicando **arquitetura MVVM** como uma aplicação profissional é construída no dia a dia.

O foco aqui é: organização, separação de responsabilidades e código escalável.

---

# 🎯 Objetivo do Desafio

Criar um aplicativo chamado **Tech Events** que:

- Consome uma API de eventos de tecnologia e programação
- Exibe uma lista paginada de eventos
- Permite buscar e filtrar eventos
- Exibe detalhe do evento
- (Opcional) permite criar/editar evento
- Implementa **MVVM** com **Repository Pattern**
- Modela estados de UI com **Sealed Class**

⚠️ Importante:
- Este desafio **não usa DI** (Hilt entra no Desafio 7).
- O app deve ser criado **do zero** já em MVVM.

---

# 🌐 API Utilizada

Tech Events API (Mock)

Endpoints:

- `GET /events?page=1&limit=10`
- `GET /events/{id}`
- `POST /events`
- `PUT /events/{id}`
- `DELETE /events/{id}`

---

# 🧠 Tecnologias e Conceitos Trabalhados

## Arquitetura e Jetpack

- MVVM
- ViewModel
- LiveData
- DataBinding

## Organização e Boas Práticas

- Repository Pattern
- Separação clara entre UI e dados
- Modelagem de estado de tela
- Extensões Kotlin

## Conceitos Avançados

- Sealed class vs Enum
- Sealed class aplicada à arquitetura (UI State)
- Generics
- Covariant vs Contravariant em tipos genéricos

---

# 📱 Telas do Aplicativo

O aplicativo deve conter:

1️⃣ Splash  
2️⃣ Lista de Eventos (com busca e filtros)  
3️⃣ Detalhe do Evento  

<img width="1208" height="807" alt="Captura de Tela 2026-02-27 às 13 25 36" src="https://github.com/user-attachments/assets/b76caf7c-e68a-4e17-a244-5602a723d266" />


---

# 🏗 Estrutura Recomendada do Projeto

Uma estrutura simples e profissional (sem Clean completo ainda):
data/
api/
dto/
repository/

domain/
model/
repository/

presentation/
ui/
viewmodel/


✅ Observação:
- Você pode manter `domain` simples (somente models + interface do repository).
- A evolução para UseCases/Clean pode vir depois.

---

# 🔄 Estados de UI (Obrigatório)

Você deve modelar o estado da tela usando **Sealed Class**.

Exemplo:

```kotlin
sealed class UiState<out T> {
    object Loading : UiState<Nothing>()
    data class Success<T>(val data: T) : UiState<T>()
    data class Error(val message: String) : UiState<Nothing>()
}
```

## 🔄 Estados Obrigatórios

- Loading  
- Success  
- Error  
- Empty (recomendado para busca sem resultado)  

---

## 🧩 Regras Técnicas

- Não colocar lógica de negócio dentro da Activity  
- A Activity/Fragment deve apenas:
  - Observar estado do ViewModel  
  - Renderizar UI  
  - Disparar ações (cliques, buscas, filtros)  

- A UI não pode acessar a API diretamente  
- Toda comunicação com rede deve passar por:
  - Repository → API Service  

- ViewModel não conhece Retrofit diretamente  
- ViewModel depende do Repository (via interface, se possível)  

Implementar:

- Busca (query)  
- Filtros (categoria / online/presencial)  
- Paginação (scroll infinito ou “carregar mais”)  

---

## ⭐ Parte Opcional (Avançado)

- Implementar tela de criar evento (POST)  
- Implementar edição (PUT)  
- Implementar delete (DELETE)  
- Implementar mappers DTO → Domain Model  
- Criar um wrapper genérico de resultados (`Result`, `ApiResult`)  
- Implementar cache simples em memória no repository  

---

## 🏁 Resultado Esperado

Ao concluir este desafio você será capaz de:

- Criar um app do zero com MVVM  
- Separar UI, ViewModel e Data Layer corretamente  
- Trabalhar com estados de tela (Loading/Success/Error)  
- Aplicar Repository Pattern  
- Manter código organizado e escalável  
- Preparar base para evoluir com DI no Desafio 7  

Você agora está desenvolvendo como alguém que trabalha em empresa.
