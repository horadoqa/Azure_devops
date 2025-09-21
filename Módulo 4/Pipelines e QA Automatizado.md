# 🎬 **Roteiro 4 – Criando e Executando Casos de Teste Manuais no Azure DevOps (Test Plans)**

## 🎯 Objetivo:

Ensinar como criar, organizar e executar **casos de teste manuais** no módulo **Test Plans** do Azure DevOps — com foco total nas tarefas do dia a dia de um QA manual.

---

## 📌 Estrutura do Roteiro:

---

### ✅ 1. Introdução (0:00–0:30)

> “Oi, pessoal! Neste vídeo, vamos aprender como criar e executar testes manuais no Azure DevOps, usando o módulo Test Plans. Esse é um recurso super útil para quem trabalha com testes funcionais, exploratórios ou regressivos.”

---

### ✅ 2. Acessando o Azure Test Plans (0:30–1:00)

* Vá para o menu lateral: `Test Plans`
* Mostre um plano já criado (ex: `Sprint 1 - Testes de Autenticação`)

> “Aqui dentro do Azure Test Plans, podemos estruturar todos os nossos testes manuais em planos e suítes. Vamos começar criando uma suíte e adicionando alguns casos.”

---

### ✅ 3. Criando uma Static Test Suite (1:00–1:45)

* Dentro do plano de teste:

  * Clique em `+ New Suite > Static suite`
  * Nome: `Validações de Login`

> “As suítes ajudam a agrupar casos de teste por funcionalidade ou tipo de teste. Aqui vamos organizar os testes relacionados ao login.”

---

### ✅ 4. Criando Casos de Teste (1:45–3:30)

* Dentro da suíte recém-criada, clique em `+ New Test Case`

##### Exemplo 1:

* **Título**: `Login com credenciais válidas`
* **Steps**:

  1. Acessar a tela de login.
  2. Inserir usuário e senha válidos.
  3. Clicar em “Entrar”.
  4. Verificar se foi redirecionado à home.

#### Exemplo 2:

* **Título**: `Login com senha incorreta`
* Passos similares, resultado esperado: "Mensagem de erro visível: 'Usuário ou senha inválidos'"

> “Cada caso pode ter vários passos, com campos para entrada, ação e resultado esperado. Isso ajuda na clareza e rastreabilidade dos testes.”

---

### ✅ 5. Executando Casos de Teste (3:30–5:30)

* Selecione o caso > clique em `Run for web application`

Durante a execução:

* Marque os passos como **Pass** ou **Fail**
* Adicione **comentários** se necessário
* Adicione **evidências** (prints ou arquivos)

> “Essa é uma das maiores vantagens do Test Plans: você pode registrar exatamente o que aconteceu em cada execução — incluindo o que falhou, prints, e até criar um bug diretamente daqui.”

---

### ✅ 6. Criando um Bug diretamente da execução (5:30–6:30)

* Mostre como clicar em `Create bug` durante um teste que falhou
* Preencher título: `Mensagem de erro ausente na tela de login`
* Bug é automaticamente vinculado ao caso de teste

> “Isso garante rastreabilidade completa: o bug está linkado ao teste que falhou, à execução e ao plano.”

---

### ✅ 7. Dicas de Organização (6:30–7:00)

> “Você pode organizar as suítes por módulos, funcionalidades, ou sprints. E também pode clonar, importar e mover testes facilmente — isso ajuda muito quando você precisa repetir testes em várias iterações.”

---

### ✅ 8. Conclusão e Gancho para o Próximo Vídeo (7:00–7:30)

> “Agora você já sabe como criar e executar testes manuais dentro do Azure DevOps. No próximo vídeo, vamos avançar para a automação: como integrar testes automatizados e visualizar os resultados diretamente aqui nos Test Plans. Até lá!”

---

## 🛠️ Dicas Visuais para Gravação:

* Mostre sempre os cliques com o mouse destacado.
* Faça zoom nos campos de passo a passo.
* Mostre claramente a mudança de status dos testes e a criação do bug.


