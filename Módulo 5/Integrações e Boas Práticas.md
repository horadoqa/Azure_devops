# 🎬 **Roteiro 5 – Integrando Testes Automatizados aos Pipelines e Test Plans (QA Automation no Azure DevOps)**

## 🎯 Objetivo:

Ensinar como integrar testes automatizados (ex: Selenium, Playwright, API tests) com Azure Pipelines e como visualizar os resultados dentro do Azure DevOps — especialmente no Test Plans, para rastreabilidade e análise.

---

## 📌 Estrutura do Roteiro:

---

### ✅ 1. Introdução (0:00–0:30)

> “Olá! Neste vídeo, vamos ver como integrar testes automatizados com Azure Pipelines e visualizar os resultados diretamente no Azure DevOps. Essa prática ajuda o time de QA a garantir qualidade contínua e visibilidade total das execuções.”

---

### ✅ 2. Pré-requisitos (0:30–1:00)

Liste rapidamente:

* Repositório com testes automatizados (ex: Selenium, Playwright, RestAssured etc.)
* Projeto no Azure DevOps com acesso ao **Pipelines**
* Script de execução de testes (ex: `dotnet test`, `npm test`, `pytest`, etc.)

> “Aqui já temos um projeto com testes automatizados versionados no Git e prontos para rodar.”

---

### ✅ 3. Criando um Pipeline Básico (1:00–3:00)

* Vá em `Pipelines > Create Pipeline`
* Escolha a origem (Ex: Azure Repos Git ou GitHub)
* Selecione o repositório com os testes
* Escolha `Starter pipeline` ou `YAML`

#### Exemplo de pipeline simples para .NET:

```yaml
trigger:
- main

pool:
  vmImage: 'windows-latest'

steps:
- task: UseDotNet@2
  inputs:
    packageType: 'sdk'
    version: '6.x'

- script: dotnet restore
  displayName: 'Restore dependencies'

- script: dotnet test --logger:trx
  displayName: 'Run tests'
```

> “Esse pipeline está configurado para rodar os testes sempre que houver uma alteração na branch `main`. E o importante: usamos o parâmetro `--logger:trx` para gerar relatórios que o Azure entende.”

---

### ✅ 4. Publicando os Resultados de Teste no Pipeline (3:00–4:00)

Logo após o `dotnet test`, adicione:

```yaml
- task: PublishTestResults@2
  inputs:
    testResultsFormat: 'VSTest'
    testResultsFiles: '**/*.trx'
    mergeTestResults: true
    testRunTitle: 'Resultados de Testes Automatizados'
```

> “Esse passo envia os resultados de testes para o Azure DevOps, e eles ficam visíveis diretamente no pipeline e também dentro do Test Plans.”

---

### ✅ 5. Executando o Pipeline e Visualizando Resultados (4:00–5:30)

* Salve o pipeline e execute.
* Mostre a execução em andamento.
* Vá na aba `Tests` do pipeline, assim que terminar.
* Mostre quantidade de testes passados, falhados e com erro.

> “Aqui você vê exatamente quais testes passaram ou falharam, com rastreabilidade direta.”

---

### ✅ 6. Integrando com Test Plans (5:30–6:30)

> “Agora vamos vincular esses testes automatizados ao Test Plans, para manter tudo rastreado no contexto de um plano de testes.”

#### Passos:

1. Vá para `Test Plans > Test Suites`
2. Crie uma nova suíte do tipo `Requirement-based suite` ou `Query-based`
3. Associe a um Work Item relacionado à funcionalidade testada
4. Associe o resultado do build ao plano de teste

> “Com isso, mesmo testes automatizados fazem parte da estratégia formal de testes e entram em relatórios.”

---

### ✅ 7. Dicas para Boas Práticas (6:30–7:00)

> “Algumas boas práticas:
>
> * Use nomes padronizados para facilitar leitura dos testes.
> * Crie uma pipeline separada para testes automatizados, se necessário.
> * Sempre publique os resultados com `PublishTestResults`.
> * Integre seus testes com work items para rastreabilidade completa.”

---

### ✅ 8. Conclusão e Gancho para o Próximo Vídeo (7:00–7:30)

> “Pronto! Agora você já sabe como rodar seus testes automatizados direto pelo Azure DevOps e visualizar os resultados de forma integrada. No próximo vídeo, vamos falar sobre como gerar **relatórios de qualidade** e **indicadores úteis para QA**, direto da ferramenta. Até lá!”

---

## 🛠️ Recursos Visuais para Gravação:

* Mostre a criação do pipeline em tempo real.
* Use um projeto de automação de exemplo (mesmo que com poucos testes).
* Dê zoom nos resultados de teste no Azure DevOps (aba `Tests` do pipeline).
* Mostre o Test Plan recebendo os resultados.

