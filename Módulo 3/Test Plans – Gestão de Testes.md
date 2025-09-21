# 🎬 **Roteiro 3 – Criando seu Primeiro Projeto no Azure DevOps (Ambiente de QA)**

### 🎯 Objetivo:

Ensinar como criar um novo projeto no Azure DevOps e configurar a estrutura básica voltada para o time de QA: tarefas, bugs, e plano de testes.

---

## 📌 Estrutura do Roteiro:

---

### ✅ 1. Introdução (0:00–0:30)

> “Oi, pessoal! Neste vídeo, vamos criar nosso primeiro projeto no Azure DevOps, com foco em QA. Vou mostrar como configurar o ambiente, escolher o tipo de processo e preparar a base para começarmos a trabalhar com tarefas, bugs e testes.”

---

### ✅ 2. Acessando a Conta e Iniciando um Projeto (0:30–1:30)

* Acesse: [https://dev.azure.com](https://dev.azure.com)
* Mostre a página inicial e clique em “**New Project**” (Novo Projeto)

> “Ao entrar na sua organização, clique em ‘New Project’ para iniciar.”

#### Campos:

* **Project name**: `QA-DemoProject` ou algo mais temático.
* **Description** (opcional): "Projeto de exemplo para automação e testes manuais."
* **Visibility**: `Private`
* **Version Control**: `Git`
* **Work Item Process**:
  👉 **Scrum** ou **Agile** (ideal para times de QA)

> “Para times de QA, os processos Scrum ou Agile funcionam muito bem. O Scrum tem artefatos como ‘Product Backlog Items’, enquanto o Agile usa ‘User Stories’.”

* Clique em `Create`.

---

### ✅ 3. Navegando no Projeto Criado (1:30–2:30)

* Mostre que agora você está dentro do novo projeto.
* Dê um tour rápido nos menus laterais (revisão rápida do vídeo anterior).
* Aponte que agora os menus estão específicos para o novo projeto.

---

### ✅ 4. Configurando os Work Items Iniciais (2:30–4:00)

> “Vamos adicionar algumas tarefas e bugs, como o time de QA faria no início de um ciclo.”

#### Criando um Work Item:

* Vá em `Boards > Work Items > New Work Item`

  * Escolha: `Bug`
  * Título: `Erro ao validar campo de e-mail`
  * Description: `Durante os testes, foi identificado que o sistema aceita e-mails sem @.`
  * Area: Default
  * Iteration: Defina a sprint ou backlog

#### Criando uma Tarefa:

* Novo Work Item: `Task`

  * Título: `Executar testes manuais do login`
  * Description: `Rodar casos de teste do módulo de autenticação.`

> “Esses itens podem ser atribuídos a membros do time, ter prioridade, tags, e serem linkados a casos de teste ou bugs relacionados.”

---

### ✅ 5. Criando um Test Plan Inicial (4:00–5:30)

* Vá em `Test Plans > New Test Plan`

  * Nome: `Sprint 1 - Testes de Autenticação`
  * Area Path: QA-DemoProject
  * Iteration: Escolha a sprint

#### Dentro do plano:

* Crie uma `Static Test Suite`: `Login`
* Adicione um caso de teste:

  * Título: `Validar login com credenciais corretas`
  * Passos: Descreva passo a passo o cenário.

> “Esses casos podem ser executados manualmente aqui dentro, com registro de resultados e evidências.”

---

### ✅ 6. Dicas de Organização para QA (5:30–6:30)

> “Algumas boas práticas para times de QA nesse momento inicial são:
>
> * Nomear bem os planos e suítes de teste.
> * Manter os bugs bem documentados com prints e passos para reproduzir.
> * Linkar bugs aos testes e aos itens do backlog.
> * Criar pastas para separar módulos ou funcionalidades.”

---

### ✅ 7. Conclusão e Gancho para o Próximo Vídeo (6:30–7:00)

> “Pronto! Criamos nosso primeiro projeto no Azure DevOps, registramos alguns itens de QA e montamos uma base para nossos testes. No próximo vídeo, vamos explorar mais a fundo como escrever e executar **casos de teste manuais** dentro do Test Plans. Te vejo lá!”

---

## 🛠️ Recursos Visuais para Gravação:

* Grave em tela cheia, com foco nos cliques.
* Use nomes e exemplos reais de QA.
* Faça zoom quando criar work items e test cases, para facilitar a leitura.


