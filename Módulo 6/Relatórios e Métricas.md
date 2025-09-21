Perfeito! Vamos fechar esse primeiro ciclo da sua playlist com um vídeo fundamental para times de QA: **relatórios e métricas de qualidade** no Azure DevOps.

---

## 🎬 **Roteiro 6 – Gerando Relatórios e Métricas de Qualidade no Azure DevOps (Indicadores para QA)**

### 🎯 Objetivo:

Mostrar como o QA pode extrair relatórios e indicadores úteis diretamente do Azure DevOps, tanto para testes manuais quanto automatizados — incluindo rastreabilidade, cobertura de testes, e taxas de sucesso.

---

### 📌 Estrutura do Roteiro:

---

#### ✅ 1. Introdução (0:00–0:30)

> “Olá! Neste vídeo, vamos ver como gerar relatórios e acompanhar métricas de qualidade dentro do Azure DevOps. São dados importantes para o time de QA mostrar valor, acompanhar evolução, e apoiar a tomada de decisão.”

---

#### ✅ 2. Visão Geral dos Relatórios no Azure DevOps (0:30–1:00)

> “O Azure DevOps não tem um painel único de QA, mas oferece vários pontos de visualização e análise de dados — dentro do Test Plans, dos Pipelines e dos Work Items. Vamos ver cada um deles.”

---

#### ✅ 3. Relatórios no **Test Plans** (1:00–2:30)

Vá em: `Test Plans > Test Runs`

##### Mostre:

* Testes executados por sprint ou plano
* Resultado por caso (Passed, Failed, Not Run)
* Filtros por executor, data, plano ou suíte
* Link com bugs criados a partir da execução

> “Aqui você tem um histórico completo de execuções manuais e seus resultados. É ótimo para saber o que foi testado e o que ainda falta testar.”

---

#### ✅ 4. Relatórios nos **Pipelines** (2:30–3:30)

* Vá em `Pipelines > <nome do pipeline>`
* Acesse uma execução
* Mostre a aba `Tests`

##### Destaque:

* Número total de testes
* Taxa de sucesso/falha
* Histórico de builds com falhas
* Links com PRs ou commits que causaram falhas

> “Esse painel é muito útil para testes automatizados. Ele mostra se os testes estão quebrando com frequência e onde estão os gargalos.”

---

#### ✅ 5. Dashboard com Widgets de QA (3:30–5:00)

> “Você pode montar **dashboards personalizados** no Azure DevOps com widgets que ajudam o time a acompanhar a qualidade em tempo real.”

##### Criando o dashboard:

1. Vá em `Dashboards > New Dashboard`
2. Nome: `Qualidade - QA`
3. Escolha o time ou projeto

##### Adicione widgets:

* **Test Plans Progress**: progresso dos testes em uma sprint
* **Test Results Trend**: histórico de resultados
* **Work Items**: bugs abertos por prioridade
* **Build History**: últimas execuções

> “Com isso, seu time pode acompanhar em tempo real como está a qualidade por sprint, módulo ou tipo de teste.”

---

#### ✅ 6. Relatórios com Power BI (opcional) (5:00–5:30)

> “Se você quiser ir além, é possível integrar o Azure DevOps com o Power BI e montar relatórios avançados, combinando dados de testes, bugs, builds e produtividade.”

(Se quiser, você pode gravar esse como um **vídeo bônus avançado** mais pra frente.)

---

#### ✅ 7. Boas Práticas de Métricas para QA (5:30–6:30)

> “Algumas métricas importantes para QA acompanhar com ajuda do Azure DevOps:
>
> * Cobertura de testes manuais e automatizados
> * Taxa de sucesso por suíte de testes
> * Bugs encontrados por tipo de teste
> * Bugs abertos x fechados por sprint
> * Tempo médio de resolução de defeitos”

> “Mas lembre-se: não use métricas apenas para cobrança, e sim como ferramentas para melhoria contínua e tomada de decisão.”

---

#### ✅ 8. Conclusão (6:30–7:00)

> “Com esses recursos do Azure DevOps, seu time de QA pode gerar relatórios claros, acompanhar a qualidade do produto e manter a rastreabilidade dos testes. Isso fortalece o papel do QA dentro do time de desenvolvimento.”

> “Se você gostou dessa série até aqui, já deixa seu like e comenta qual tema você quer ver nos próximos vídeos. Até a próxima!”

---

## 🛠️ Dicas Visuais para Gravação:

* Mostre a criação de um dashboard real, mesmo que com dados fictícios.
* Navegue entre os painéis reais do Test Plans e Pipelines.
* Use filtros em tempo real para mostrar como segmentar por sprint ou executor.

---

## ✅ Com isso, sua playlist cobre:

| Módulo | Tema                    | Tipo                  |
| ------ | ----------------------- | --------------------- |
| 1      | O que é Azure DevOps    | Teórico               |
| 2      | Tour pela interface     | Teórico/Demonstrativo |
| 3      | Criando o projeto       | Prático               |
| 4      | Casos de teste manuais  | Prático               |
| 5      | Automação com pipelines | Prático               |
| 6      | Relatórios e métricas   | Estratégico           |


