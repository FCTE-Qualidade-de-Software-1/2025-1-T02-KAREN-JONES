# __Fase 3 - Plano de Avaliação__

## 1. Fonte dos Dados

- Logs de erro do sistema para as métricas de Performance
- Resultado de testes automatizados e manuais para ambas métricas
- Ferramentas de análise estática de código para as métricas de Performance
- Ferramentas de análise de performance

## 2. Técnicas de Coleta

- Execução de testes automatizados e inspeção de resultados para as métricas de Performance
- Testes manuais simulando fluxos de uso do consumidor e agricultor para as métricas de Usabilidade
- Análise com ferramentas como Lighthouse e WebPageTest para as métricas de Performance
- Avaliação da interface de acordo com a legibilidade em geral para as métricas de Usabilidade

## 3. Responsáveis

| Tarefas | Responsável | 
| ------- | ----------- |
| Testes funcionais e automatizados | [Mateus Bastos](https://github.com/MateuSansete) |
| Avaliação de usabilidade | [Rafael Kenji](https://github.com/rafa-kenji) | 
| Análise de desempenho            | [Rafael Matuda](https://github.com/rmatuda)  |
| Coleta de dados de segurança     | [Catlen Cleane](https://github.com/catlenc) |
| Organização dos dados            | [Luiza Maluf](https://github.com/LuizaMaluf)  |

## 4. Cronograma

| Atividade                            | Data Limite | Responsável       |
|--------------------------------------|-------------|-------------------|
| Execução dos testes                  | 03/07       | [Mateus Bastos](https://github.com/MateuSansete)   |
| Avaliação de usabilidade             | 04/07       | [Rafael Kenji](https://github.com/rafa-kenji)    |
| Coleta de métricas de segurança      | 05/07       | [Catlen Cleane](https://github.com/catlenc)   |
| Testes de performance e eficiência   | 06/07       | [Rafael Matuda](https://github.com/rmatuda)   |
| Consolidação dos dados da avaliação  | 07/07       | [Luiza Maluf](https://github.com/LuizaMaluf)     |

# 5. Ferramentas Utilizadas

- **Postman** – para testes de API
- **Lighthouse / WebPageTest** – para avaliação de performance para as métricas de Performance
- **ESLint / SonarQube** – para inspeção de código para as métricas de Performance
- **GitHub Projects / Issues / Commits** – para registro das atividades e progresso

## 6. Forma de Documentação

- Planilha de métricas (.ods/.xlsx) para as métricas de Usabilidade
- Documentação em `docs/` no repositório GitHub
- Slides com resumo da avaliação e gráficos de desempenho
- Tabela de critérios + valores reais + julgamentos em todas as métricas
- Proposta de ação de melhoria ancorada nos dados coletados

## 7. Mapeamento Objetivo-Métrica

| Objetivo Estratégico                                      | Métrica Avaliada                                                                 |
|----------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **Assegurar desempenho eficiente e escalável da aplicação**          | - Tempo de resposta (ms)                                                         |
|                                                                      | - Número médio de requisições por segundo (RPS)                                  |
|                                                                      | - Latência média das requisições                                                 |
|                                                                      | - Taxa de respostas 2xx vs não-2xx                                               |
|                                                                      | - FCP, LCP, TBT (indicadores de performance front-end)                           |
|                                                                      | - Gargalos de cache/JS e consumo de recursos                                     |
| **Garantir experiência de uso acessível, responsiva e confiável**   | - M1 a M6 (visibilidade, feedback, responsividade, acessibilidade)               |
|                                                                      | - Avaliação heurística e testes manuais                                          |
| **Aumentar a confiabilidade e estabilidade do sistema sob demanda** | - Logs de erro                                                                    |
|                                                                      | - Taxa de falhas críticas (%)                                                    |
|                                                                      | - Taxa de respostas de erro (HTTP 4xx, 5xx)                                      |
| **Fortalecer a qualidade estrutural do código**                      | - Relatórios do ESLint / SonarQube                                               |
|                                                                      | - Identificação de erros lógicos e uso ineficiente de recursos                   |
| **Aumentar a cobertura e efetividade dos testes**                    | - Cobertura de testes (%)                                                        |
|                                                                      | - % de funcionalidades testadas com sucesso (via Jest / Vitest ou testes manuais)|



## 8. Critérios de Aceitação

| Métrica                           | Excelente | Aceitável | Ruim     |
|----------------------------------|-----------|-----------|----------|
| Tempo de resposta (ms)           | < 500     | 500–1000  | > 1000   |
| Taxa de falhas críticas (%)      | < 1%      | 1%–3%     | > 3%     |
| Cobertura de testes (%)          | > 90%     | 70%–90%   | < 70%    |

---
## Histórico de versão

| Versão | Descrição | Responsável | Revisor | Data de Revisão |
|--------|-----------|-------------|---------|-----------------|
| `1.0`  | Documentação do planejamento | [Luiza Maluf](https://github.com/LuizaMaluf) | [Mateus Bastos](https://github.com/MateuSansete)| 08/07/2025|
| `1.1`  | Atualização do planejamento | [Rafael Kenji](https://github.com/rafa-kenji) | [Mateus Bastos](https://github.com/MateuSansete), [Luiza Maluf](https://github.com/LuizaMaluf)| 08/07/2025|
