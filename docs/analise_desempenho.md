## Relatório de Análise de Dados e Melhoria - Projeto AgroMart

## 1. Planilha Estruturada de Dados

Abaixo está a consolidação dos dados extraídos dos relatórios em um formato de planilha. Os critérios de classificação foram definidos com base nas informações e implicações observadas nos relatórios, priorizando segurança > usabilidade > desempenho.

| Métrica | Valor Coletado | Classificação | Fonte | Critério de Aceitação |
| :----------------------------------------- | :--------------------- | :------------ | :------------------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tempo de Resposta da API (POST /api/lojas) | 42 ms | Excelente | Pessoa 1 | Excelente: <100ms \| Aceitável: 100-300ms \| Ruim: >300ms |
| Tempo de Resposta da API (PUT /api/lojas) | 38 ms | Excelente | Pessoa 1 | Excelente: <100ms \| Aceitável: 100-300ms \| Ruim: >300ms |
| Tempo de Resposta da API (DELETE /api/lojas) | 40 ms | Excelente | Pessoa 1 | Excelente: <100ms \| Aceitável: 100-300ms \| Ruim: >300ms |
| Bugs (Back-end - SonarQube) | 2 | Ruim | Pessoa 1 | Excelente: 0 \| Aceitável: 1-2 (menor gravidade) \| Ruim: >2 ou qualquer "Blocker" |
| Vulnerabilidades (Back-end - SonarQube) | 0 | Excelente | Pessoa 1 | Excelente: 0 \| Aceitável: 1-2 (menor gravidade) \| Ruim: >2 ou qualquer "Crítico" |
| Security Hotspots (Back-end - SonarQube) | 14 para revisão | Ruim | Pessoa 1 | Excelente: 0 \| Aceitável: 1-5 (revisados e sem risco) \| Ruim: >5 ou com riscos não mitigados (ex: hardcoded credentials) |
| Credenciais Hardcoded (Back-end) | Presente em testes (ex: `password: "1234userauth"`) | Ruim | Pessoa 1 | Excelente: Ausente \| Aceitável: Presente apenas em mocks de teste não expostos \| Ruim: Presente em código-fonte, mesmo em testes, se houver risco de exposição |
| Bugs (Front-end - SonarQube) | 0 | Excelente | Pessoa 1 | Excelente: 0 \| Aceitável: 1-2 (menor gravidade) \| Ruim: >2 ou qualquer "Blocker" |
| Vulnerabilidades (Front-end - SonarQube) | 0 | Excelente | Pessoa 1 | Excelente: 0 \| Aceitável: 1-2 (menor gravidade) \| Ruim: >2 ou qualquer "Crítico" |
| Security Hotspots (Front-end - SonarQube) | 0 | Excelente | Pessoa 1 | Excelente: 0 \| Aceitável: 1-5 (revisados e sem risco) \| Ruim: >5 ou com riscos não mitigados |
| Débito Técnico (Front-end - SonarQube) | 1h 17min | Excelente | Pessoa 1 | Excelente: <2h \| Aceitável: 2h-8h \| Ruim: >8h |
| Code Smells (Front-end - SonarQube) | 17 | Excelente | Pessoa 1 | Excelente: <20 \| Aceitável: 20-50 \| Ruim: >50 |
| Cobertura de Testes (Front-end - SonarQube) | 0% (0 testes) | Ruim | Pessoa 1 | Excelente: >80% \| Aceitável: 50-80% \| Ruim: <50% ou 0% |
| Duplicação de Código (Front-end - SonarQube) | 2.9% (2 blocos) | Aceitável | Pessoa 1 | Excelente: <1% \| Aceitável: 1-5% \| Ruim: >5% |
| Controle de Acesso (Login sem autenticação) | Redirecionado para login | Excelente | Pessoa 1 | Excelente: Impede acesso/redireciona para login \| Ruim: Permite acesso |
| Controle de Acesso (Login Válido) | Página carregada com dados | Excelente | Pessoa 1 | Excelente: Acesso concedido e dados exibidos corretamente \| Ruim: Falha no acesso ou dados incorretos |
| Controle de Acesso (Pós-Logout) | Redirecionado para login | Excelente | Pessoa 1 | Excelente: Redireciona para login e remove sessão \| Ruim: Mantém sessão ou acesso |
| Rota /lojas na Interface Web | Rota não encontrada/inacessível (Erro de navegação/renderização) | Ruim | Pessoa 1 | Excelente: Funcionalidade acessível e operante \| Aceitável: Pequenos bugs visuais \| Ruim: Funcionalidade inacessível/bloqueada |
| Testes Automatizados Backend | 44 testes falharam (DB não configurado, JWT indefinido, Timeouts) | Ruim | Pessoa 1 | Excelente: >90% passando \| Aceitável: 70-90% passando \| Ruim: <70% passando ou falha crítica de infraestrutura de testes |
| Testes Automatizados Frontend | Nenhum teste encontrado | Ruim | Pessoa 1 | Excelente: Testes automatizados implementados \| Ruim: Ausência de testes automatizados |
| Link de Recuperação de Senha | Não funciona (leva para página inexistente) | Ruim | Pessoa 2 | Excelente: Funciona corretamente \| Aceitável: Redireciona para página genérica \| Ruim: Não funciona ou leva a erro |
| Envio de Notificações (Web) | Erro 405 Method Not Allowed | Ruim | Pessoa 2 | Excelente: Funcionalidade operante \| Aceitável: Mensagens de erro claras \| Ruim: Funcionalidade não executa/erro inesperado |
| Cadastro de Usuário (Web) | Não registra usuário (mensagem de erro "Erro no cadastro") | Ruim | Pessoa 2 | Excelente: Cadastra usuário corretamente \| Aceitável: Pequenos bugs ou lentidão \| Ruim: Não permite cadastro |
| Responsividade da Barra Lateral (Web) | Não é responsiva em tela não cheia | Ruim | Pessoa 2 | Excelente: Totalmente responsiva \| Aceitável: Pequenos ajustes necessários \| Ruim: Prejudica a usabilidade em diferentes tamanhos de tela |
| Botão de Notificação (Web) | Não resulta em nada ao clicar | Ruim | Pessoa 2 | Excelente: Funcionalidade operante \| Ruim: Não funciona |

## 2. Análise dos Resultados e Priorização da Melhoria

Com base na tabela e nos critérios de priorização (segurança > usabilidade > desempenho), identifiquei que a melhoria mais urgente é a **falha crítica nos testes automatizados do backend** e a **ausência de testes automatizados no frontend**. 

Embora existam problemas de usabilidade impactantes, a base de testes inoperante ou inexistente representa um risco significativo para a sustentabilidade e a introdução de novas funcionalidades no futuro.

 A falta de testes automatizados de backend, com 44 falhas devido a problemas de infraestrutura (banco de dados de teste e autenticação), e a completa ausência de testes no frontend, indicam uma lacuna fundamental no processo de desenvolvimento que pode levar a regressões e falhas não detectadas, impactando indiretamente tanto a segurança quanto a usabilidade.

**Métrica Prioritária:** Testes Automatizados (Backend e Frontend) - Classificação: Ruim.

**Justificativa:** A ausência ou falha generalizada dos testes automatizados impacta diretamente a **confiabilidade** e a **segurança** do sistema a longo prazo. Sem testes robustos, qualquer alteração no código pode introduzir novos bugs ou vulnerabilidades sem que sejam detectados rapidamente, comprometendo a estabilidade da aplicação e a experiência do usuário.

 As falhas nos testes de backend são de infraestrutura (banco de dados e JWT), o que impede a validação de qualquer funcionalidade, e a ausência de testes no frontend significa que a interface do usuário não tem garantia de funcionamento, o que pode levar a problemas de usabilidade não identificados antes do deploy.

## 3. Plano de Ação para Implementação da Melhoria

**Métrica Escolhida:** Correção e Implementação de Testes Automatizados (Backend e Frontend).

**Solução Proposta:**
1.  **Backend:** Corrigir a infraestrutura dos testes automatizados (configuração do banco de dados de teste e inicialização do JWT) e garantir que todos os 44 testes falhos sejam corrigidos e passem.

2.  **Frontend:** Implementar testes unitários e de integração para garantir a cobertura de código e a regressão segura da interface web.

**Ferramentas:**
* **Backend:** `sudo u postgres createdb tobemodified-test` (para o banco de dados), Jest/Supertest (framework de testes), Postman (para validação manual de endpoints da API após a correção).

* **Frontend:** Jest/React Testing Library (framework de testes e utilitários), Cypress/Playwright (para testes de integração/E2E, se aplicável).

* **Controle de Versão:** GitHub (para revisão de código e gerenciamento de tarefas).

<br>

**Passos Detalhados:**

**Fase 1: Correção dos Testes Automatizados de Backend**

1.  **Configuração do Banco de Dados de Teste:**
    * Criar o banco de dados de teste `tobemodified-test` conforme recomendado: `sudo u postgres createdb tobemodified-test`.
    * Aplicar migrações ao ambiente de teste: `yarn strapi migrations:apply-env test`.
    * **Verificar:** Executar novamente os testes e observar se o erro "database 'tobemodified-test' does not exist" foi resolvido.
2.  **Inicialização da Autenticação (JWT):**
    * Adicionar um helper para gerar o token JWT antes da execução dos testes que dependem de autenticação, conforme sugerido no documento.
    * **Verificar:** Executar os testes de autenticação novamente e garantir que `ReferenceError: jwt is not defined` não ocorra mais.
3.  **Ajustar Timeouts:**
    * Aumentar o `testTimeout` para 30000 ms (ou um valor adequado) no arquivo `jest.config.js` para evitar falhas por operações assíncronas lentas.
    * **Verificar:** Executar os testes com operações assíncronas e confirmar que não há mais `Exceeded timeout of 150000 ms for a hook`.
4.  **Correção dos Bugs Remanescentes:**
    * Analisar os logs de erro e arquivos afetados (ex: `tests/auth/login.js`, `tests/extracoes/index.js`, `config/env/test/database.js`) para identificar as causas raiz dos 44 testes falhos após as correções de infraestrutura.
    * Implementar as correções necessárias no código dos testes e/ou da aplicação para que todos os testes passem.

**Fase 2: Implementação de Testes Automatizados no Frontend**

1.  **Configuração do Ambiente de Testes:**
    * Garantir que o Jest e as bibliotecas de teste (como React Testing Library) estejam corretamente instaladas e configuradas no projeto `agromart-web`.
2.  **Definição de Cenários de Teste:**
    * Identificar as funcionalidades críticas do frontend que precisam de testes unitários e de integração, como:
        * Login (sucesso, falha, recuperação de senha - *importante priorizar a correção do link de recuperação de senha paralelamente*).
        * Cadastro de usuário (sucesso, validação de campos, mensagens de erro - *importante priorizar a correção do erro no cadastro paralelamente*).
        * Navegação (acesso à rota `/lojas` - *priorizar a correção desta rota paralelamente*).
        * Funcionalidades da barra lateral (notificações, cadastro).
        * Envio de notificações (verificar a integração com o backend após a correção do erro 405).
3.  **Desenvolvimento dos Testes:**
    * Escrever testes unitários para componentes individuais (ex: formulário de login, componentes da barra lateral).
    * Escrever testes de integração para fluxos de usuário mais complexos (ex: login completo, navegação para diferentes páginas, submissão de formulários).
    * Assegurar que os testes cubram as 226 linhas de código a serem testadas.
4.  **Execução e Validação:**
    * Executar os testes regularmente e garantir que novos commits não introduzam falhas.
    * Acompanhar a métrica de cobertura de testes no SonarQube para aumentar a porcentagem de cobertura (atualmente 0%).

### Histórico de Versões

| Versão | Data de Produção | Descrição da Alteração | Autor(es) | Revisor(es) | Data de Revisão |
|:------:|:----------------:|:----------------------:|:---------:|:-----------:|:--------------:|
| 1.0    | 06/07/2025       |Desenvolvimento de Relatorio de análise de desempenho |  [Rafael Matuda](https://github.com/rmatuda) |[Mateus Bastos](https://github.com/MateuSansete)| 08/07/2025|
