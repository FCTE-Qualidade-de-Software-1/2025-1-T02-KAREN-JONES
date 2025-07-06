# Relatório de Performance e Eficiência

Este relatório apresenta uma análise da performance do front-end, avaliada com o Lighthouse, e da eficiência do back-end, medida por testes de carga. O objetivo é identificar gargalos e fornecer recomendações para otimização.

---

## 1. Análise de Performance do Front-End (Client-Side)

Foram analisadas três páginas principais da aplicação: **Página Inicial**, **Login** e **Cadastro**. Os resultados do Lighthouse mostram uma variação significativa de performance entre elas.

| Métrica                     | Página Inicial | Página de Login | Página de Cadastro |
|----------------------------|----------------|------------------|---------------------|
| **Pontuação de Performance** | 🟧 61/100       | 🟩 84/100         | 🟩 89/100            |
| **First Contentful Paint (FCP)** | 3.7 s          | 1.4 s            | 1.3 s               |
| **Largest Contentful Paint (LCP)** | 3.8 s          | 1.9 s            | 1.5 s               |
| **Total Blocking Time (TBT)**     | 0 ms           | 120 ms           | 120 ms              |

### Diagnóstico

- **Página Inicial**: A performance é baixa (**61/100**), com tempos de carregamento (FCP e LCP) muito lentos, ultrapassando **3.7 segundos**, o que prejudica a primeira impressão do usuário.  
  - Principais oportunidades de melhoria:
    - Uso de cache eficiente (pode economizar até **670 KiB**).
    - Redução e minificação de JavaScript não utilizado (economia de quase **700 KiB**).

- **Páginas de Login e Cadastro**: Ambas apresentam boa performance (**84** e **89**), com carregamento visual rápido.
  - Porém, compartilham um problema de **Total Blocking Time (120 ms)**, indicando que tarefas longas de JavaScript podem atrasar a interatividade.
  - Recomendações semelhantes:
    - Otimizar o uso de JavaScript.
    - Melhorar o cache de recursos.

---

## 2. Análise de Eficiência do Back-End (Server-Side)

Foram realizados testes de carga em dois endpoints críticos da API: **autenticação (/auth/local)** e **notificações (/api/notificacoes)**.

### Resultados do Teste de Carga

| Endpoint           | Requisições/Segundo (Média) | Latência (Média) | Respostas 2xx | Respostas não-2xx |
|--------------------|-----------------------------|------------------|----------------|--------------------|
| `/api/notificacoes` | 44.8                        | 220.87 ms        | 0              | 448                |
| `/auth/local`       | 44.0                        | 224.49 ms        | 0              | 440                |

### Diagnóstico

🚨 **Falha Crítica sob Carga**: Ambos os endpoints falharam em **100% das requisições** sob uma carga moderada (10 conexões simultâneas).  
A latência e o número de requisições por segundo tornam-se irrelevantes, pois **nenhuma operação foi concluída com sucesso**.

Possíveis causas:
- Erros de lógica na aplicação sob concorrência.
- Esgotamento de recursos do servidor ou banco de dados.
- Configuração inadequada do ambiente de produção.

---

## Conclusão e Recomendações Prioritárias

### 🔴 Prioridade Máxima (Back-End)

- **Correção imediata** das falhas nos endpoints da API.
- A aplicação **não suporta múltiplos usuários simultâneos** em funções essenciais como login e notificações.
- Necessário realizar **debug no servidor** para encontrar a causa dos erros **não-2xx**.

### 🟠 Prioridade Média (Front-End)

- **Otimizar a Página Inicial** para melhorar retenção de usuários.
  - Configurar uma **política de cache eficiente** para recursos estáticos.
  - **Reduzir e minificar JavaScript** para diminuir tempo de carregamento.
  - **Adiar scripts não essenciais** no carregamento da página.

### 🟢 Melhoria Contínua (Front-End)

- Para páginas de **Login** e **Cadastro**:
  - Foco em **reduzir o Total Blocking Time**.
  - **Quebrar ou otimizar tarefas longas** de JavaScript para melhorar a responsividade da interface.

### Histórico de Versões

| Versão | Data de Produção | Descrição da Alteração | Autor(es) | Revisor(es) | Data de Revisão |
|:------:|:----------------:|:----------------------:|:---------:|:-----------:|:--------------:|
| 1.0    | 06/07/2025       |Desenvolvimento de Relatorio de Performance e Eficiência |  [Rafael Matuda](https://github.com/rmatuda) |||
---