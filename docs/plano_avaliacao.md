# __Fase 3 - Plano de Avaliação__

## 1. Fonte dos Dados

- Logs de erro do sistema
- Resultado de testes automatizados e manuais
- Ferramentas de análise estática de código
- Ferramentas de análise de performance

## 2. Técnicas de Coleta

- Execução de testes automatizados e inspeção de resultados
- Testes manuais simulando fluxos de uso do consumidor e agricultor
- Análise com ferramentas como Lighthouse e WebPageTest
- Avaliação da interface a partir de critários heurísticos

## 3. Responsáveis

<center> 

| Tarefas | Responsável | 
| ------- | ----------- |
| Testes funcionais e automatizados | [Mateus Bastos] |
| Avaliação de usabilidade | [Rafael Kenji] | 
| Análise de desempenho            | [Rafael Matuda]  |
| Coleta de dados de segurança     | [Catlen Cleane] |
| Organização dos dados            | [Luiza Maluf]  |

</center>

## 4. Cronograma

<center>

| Atividade                            | Data Limite | Responsável       |
|--------------------------------------|-------------|-------------------|
| Execução dos testes                  | 03/07       | [Mateus Bastos]   |
| Avaliação de usabilidade             | 04/07       | [Rafael Kenji]    |
| Coleta de métricas de segurança      | 05/07       | [Catlen Cleane]   |
| Testes de performance e eficiência   | 06/07       | [Rafael Matuda]   |
| Consolidação dos dados da avaliação  | 07/07       | [Luiza Maluf]     |

</center>

# 5. Ferramentas Utilizadas

- **Jest / Vitest** – para testes unitários e de integração
- **Postman** – para testes de API
- **Lighthouse / WebPageTest** – para avaliação de performance
- **ESLint / SonarQube** – para inspeção de código
- **GitHub Projects / Issues / Commits** – para registro das atividades e progresso

## 6. Forma de Documentação

- Planilha de métricas (.ods/.xlsx)
- Documentação em `docs/` no repositório GitHub
- Slides com resumo da avaliação e gráficos de desempenho
- Tabela de critérios + valores reais + julgamentos
- Proposta de ação de melhoria ancorada nos dados coletados

## 7. Mapeamento Objetivo-Métrica

<center>

| Objetivo Estratégico                               | Métrica Avaliada                              |
|----------------------------------------------------|-----------------------------------------------|
| __Garantir robustez e qualidade do sistema__           | Nº de falhas críticas por semana              |
|                                                    | % de funcionalidades implementadas com sucesso|
| __Aumentar a segurança da plataforma__                 | Presença de criptografia e autenticação forte |
| __Promover inovação e adaptabilidade__                 | Nº de funcionalidades novas via feedback     |

</center>

## 9. Critérios de Aceitação

<center>

| Métrica                           | Excelente | Aceitável | Ruim     |
|----------------------------------|-----------|-----------|----------|
| Tempo de resposta (ms)           | < 500     | 500–1000  | > 1000   |
| Taxa de falhas críticas (%)      | < 1%      | 1%–3%     | > 3%     |
| Cobertura de testes (%)          | > 90%     | 70%–90%   | < 70%    |

</center>