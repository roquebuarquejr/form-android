
# 🚀 Desafio 1 — Simulador de Investimentos

Bem-vindo ao primeiro desafio da Formação Android.

Neste desafio você irá construir um aplicativo completo chamado **Simulador de Investimentos**, colocando em prática os fundamentos essenciais do desenvolvimento Android.

O objetivo aqui não é apenas fazer funcionar — é entender como as telas se comunicam, como o ciclo de vida funciona e como estruturar layouts profissionais.

---

# 🎯 Objetivo do Desafio

Criar um aplicativo com múltiplas telas que:

- Recebe dados do usuário
- Realiza cálculos com base em juros compostos
- Navega entre telas
- Exibe o resultado de forma organizada
- Utiliza Fragments para modularizar a interface

---

# 🧠 Tecnologias que você irá praticar

Este desafio foi projetado para consolidar os seguintes conceitos:

- Activity
- Navegação entre activities
- Ciclo de vida de Activity
- Passagem de dados entre telas
- Passagem de objetos entre telas
- Fragments
- Fragment KTX (Jetpack)
- XML
- ConstraintLayout
- ScrollView
- TextInputLayout
- Temas e estilos
- Organização de layouts

---

# 📱 Estrutura do Aplicativo

O aplicativo deve conter **3 telas principais**.

<img width="1203" height="790" alt="Captura de Tela 2026-02-25 às 18 29 18" src="https://github.com/user-attachments/assets/41143ddc-03f6-4767-9825-3de4f8728de4" />


---

## 🟢 Tela 1 — Boas-vindas

Objetivo:
Apresentar o app ao usuário.

Elementos esperados:

- Ícone ilustrativo
- Título: “Simulador de Investimentos”
- Texto explicativo
- Botão: “Começar Simulação”

Ao clicar no botão:
➡ Navegar para a tela de configuração.

Tecnologias aplicadas:
- Activity
- Navegação entre Activities
- Temas e estilos
- Organização de layout com ConstraintLayout

---

## 🟡 Tela 2 — Configuração da Simulação

Objetivo:
Coletar os dados do usuário.

Campos obrigatórios:

- Valor inicial
- Aporte mensal
- Taxa de juros (% ao ano)
- Tempo (anos)

Requisitos técnicos:

- Utilizar `TextInputLayout`
- Layout dentro de `ScrollView`
- Validar entradas
- Organizar com `ConstraintLayout`

Botão:
➡ “Calcular Investimento”

Ao clicar:
- Realizar o cálculo
- Criar um objeto com os dados
- Passar os dados para a próxima Activity

Tecnologias aplicadas:
- Passagem de dados entre Activities
- Passagem de objeto
- Ciclo de vida de Activity
- XML estruturado

---

## 🔵 Tela 3 — Resultado da Simulação

Objetivo:
Exibir os resultados do cálculo.

Elementos esperados:

- Valor final acumulado (destaque principal)
- Total investido
- Lucro obtido
- Container para Fragment

---

### 🧩 Fragment — Resumo

Este fragment deve:

- Receber parâmetros via Bundle
- Utilizar Fragment KTX para leitura dos argumentos
- Exibir informações detalhadas

Tecnologias aplicadas:
- Criação de Fragment
- Passagem de parâmetros para Fragment
- Uso de Fragment KTX
- Organização modular da interface

---

# 🧮 Regras de Cálculo

Utilize a fórmula de juros compostos:
M = P (1 + i)^t

Onde:

- M = montante final
- P = valor inicial
- i = taxa de juros
- t = tempo

Caso haja aporte mensal, você pode implementar uma fórmula aproximada ou um cálculo iterativo por mês.

---

# ⭐ Parte Opcional (Avançado)

A terceira tela pode conter uma **lista de projeção anual** (exemplo: Ano 1, Ano 2, Ano 3...).

⚠ Essa parte é opcional neste nível.

Ela poderá ser aprimorada após o aluno avançar para o próximo nível, quando trabalhará com listas e RecyclerView.

---

# 📐 Boas Práticas Esperadas

- Código organizado
- Separação clara entre responsabilidades
- Layout limpo
- Uso adequado do ciclo de vida
- Tratamento básico de rotação de tela
- Nomeação clara de variáveis e classes

---

# 🏁 Resultado Esperado

Ao concluir este desafio, você será capaz de:

- Criar aplicações com múltiplas telas
- Navegar entre Activities
- Trabalhar com Fragments
- Passar dados entre telas
- Estruturar layouts profissionais
- Entender o ciclo de vida no Android

Este é o primeiro passo para se tornar um desenvolvedor Android profissional.

---

## 🚀 Próximo Nível

No próximo desafio você irá trabalhar com:

- Listas dinâmicas
- RecyclerView
- Manipulação de coleções
- Atualização de dados em tempo real

Continue evoluindo.
