# FASE 1 – PROPÓSITO DA AVALIAÇÃO DE QUALIDADE DO AGROMART WEB

## 1.1 Contexto e Motivação

O **AgroMart Web** é uma aplicação web desenvolvida para conectar pequenos produtores rurais a consumidores por meio de um sistema digital acessível, funcional e responsivo. 

Voltada para agricultores familiares que buscam autonomia na venda de seus produtos, a plataforma oferece funcionalidades como cadastro de loja, publicação de produtos e envio de notificações para clientes.

Dada a natureza do público-alvo, muitas vezes com baixa escolaridade digital, conectividade limitada e uso predominante de dispositivos móveis, a **qualidade da experiência de uso** se torna um fator decisivo para o sucesso da solução. Garantir que os usuários consigam interagir com o sistema de forma eficaz, eficiente e satisfatória é essencial para promover a adoção e retenção da plataforma.

## 1.2 Declaração do Propósito

> Avaliar a qualidade do sistema **AgroMart Web**, com foco especial em **usabilidade**, **performance** e **robustez**, a fim de diagnosticar falhas de interação, lentidão ou inconsistência no uso da plataforma, propondo ações concretas para melhoria contínua da experiência do usuário, principalmente agricultores familiares.

## 1.3 Objetivos Específicos

- **Avaliar a Usabilidade**
  - Verificar se os elementos da interface são compreensíveis e visíveis;
  - Testar a experiência em diferentes resoluções de tela (responsividade);
  - Avaliar a clareza dos feedbacks interativos da aplicação.

- **Avaliar a Performance**
  - Medir tempos de carregamento e resposta das páginas principais;
  - Avaliar o desempenho do back-end sob carga;
  - Identificar gargalos de desempenho no código front-end e backend.

- **Apoiar Melhorias Contínuas**
  - Fornecer evidências para aprimorar a qualidade da interface;
  - Priorizar pontos críticos de usabilidade e desempenho;
  - Promover ajustes baseados em dados reais e nos perfis reais dos usuários.

## 1.4 Alinhamento com os Objetivos de Negócio

| Objetivo Estratégico                | Contribuição da Avaliação                                           |
|------------------------------------|----------------------------------------------------------------------|
| **Robustez e Qualidade**           | Detectar falhas críticas e inconsistências na interface ou nos fluxos de uso |
| **Segurança da Plataforma**        | Avaliar a clareza de telas de login, cadastro e recuperação de acesso |
| **Inovação e Adaptabilidade**      | Coletar dados que embasem novas funcionalidades e melhorias incrementais |
| **Inclusão Digital**               | Avaliar a acessibilidade e clareza da interface para agricultores de baixa letramento digital |

## 1.5 Produtos Avaliados

- **Nome do Sistema:** AgroMart Web  
- **Tipo:** Aplicação Web Responsiva  
- **Frontend:** React  
- **Backend:** Strapi (Headless CMS via API REST)  
- **Banco de Dados:** PostgreSQL  
- **Repositório:** [github.com/AgroMart/agromart-web](https://github.com/AgroMart/agromart-web)  
- **Público-alvo:** Agricultores familiares (usuários que gerenciam lojas e produtos)  

## 1.6 Escopo da Avaliação

**Incluído na Avaliação:**
- Interface web do agricultor (login, cadastro, dashboard);
- Módulo de notificações e gerenciamento de produtos;
- Funcionalidades identificadas por inspeção da API e interface;
- Responsividade e feedback visual da interface;
- Análise de performance de carregamento de páginas e respostas da API.

**Excluído da Avaliação:**
- Aplicativo mobile voltado ao consumidor;
- Camada administrativa do CMS (Strapi);
- Infraestrutura de rede e banco de dados;
- Processamento de pagamentos externos.

## 1.7 Modelo de Qualidade Utilizado

A avaliação se baseia no modelo da norma **ISO/IEC 25010**, com ênfase nas características:

- **Usabilidade**: Apreensibilidade, Operabilidade, Proteção contra Erros, Estética da Interface, Acessibilidade;
- **Desempenho e Eficiência**: Comportamento de tempo de resposta, utilização de recursos;
- **Confiabilidade**: Tolerância a falhas e estabilidade sob carga.

Além disso, será aplicado o método **GQM (Goal-Question-Metric)** para seleção e justificativa de métricas, conforme detalhado na Fase 2.

---

## 1.8 Perfil dos Usuários

Com base em dados do **Censo Agropecuário 2017 (IBGE)** e no propósito social do AgroMart, o perfil típico do usuário da plataforma é:

- **Idade**: Predominância de usuários com mais de 45 anos;
- **Escolaridade**: Parte significativa sem ensino fundamental completo;
- **Experiência Digital**: Limitada; muitos utilizam smartphones como principal dispositivo;
- **Infraestrutura**: Acesso intermitente à internet e dispositivos de entrada simples (touchscreen);
- **Familiaridade com sistemas**: Baixa exposição a plataformas digitais sofisticadas.

Este perfil reforça a necessidade de **interfaces simples**, **mensagens claras**, **feedbacks visuais fortes** e **responsividade** adaptada a conexões lentas.

## 1.9 Ambiente de Uso

- **Local físico**: Propriedades rurais, cooperativas ou casas de agricultores;
- **Dispositivos predominantes**: Smartphones básicos ou intermediários com Android;
- **Conectividade**: Redes móveis 3G/4G com sinal instável em muitas regiões;
- **Condições ambientais**: Exposição à luz solar, uso ao ar livre, tempo reduzido para navegação;
- **Suporte técnico**: Escasso ou inexistente para resolução de problemas técnicos.

Essas características impactam diretamente na necessidade de interfaces que:

- Sejam **leves e rápidas** (baixo consumo de dados);
- Operem mesmo com falhas intermitentes de conexão;
- Evitem dependência de recursos gráficos pesados ou animações.

## 1.10 Tarefas Críticas Identificadas

As funcionalidades abaixo são consideradas **tarefa crítica**, pois representam ações essenciais para o uso contínuo da plataforma:

| Tarefa                         | Justificativa de Relevância                                    |
|-------------------------------|-----------------------------------------------------------------|
| **Autenticação (Login/Cadastro)** | Primeira barreira de entrada; falhas bloqueiam o uso da plataforma |
| **Cadastro de Loja e Produtos** | Permite a oferta dos itens produzidos pelos agricultores        |
| **Gerenciamento de Notificações** | Facilita a comunicação com os consumidores                      |
| **Acesso ao Dashboard e Navegação** | Controla todas as funções internas da conta do agricultor       |
| **Respostas a dúvidas e mensagens** | Imprescindível para manter relacionamento e confiança do cliente |

---

**Conclusão da Fase 1:**  
Este plano estabelece os fundamentos conceituais e contextuais para a avaliação de qualidade do sistema AgroMart Web, considerando suas especificidades sociais, técnicas e funcionais. As decisões tomadas aqui embasam os critérios, métricas e execuções práticas das Fases 2 e 3.





---


## Tabela de contribuição:

| Matrícula   | Nome Completo                                                   | Contribuição (%) |
|-------------|------------------------------------------------------------------|-----------------|
| 211062240   | [Mateus Bastos](https://github.com/MateuSansete)                 | 50               |
| 190044128   | [Rafael Kenji Taira](https://github.com/rafa-kenji)             | 20              |
| 222006383   | [Rafael Matuda](https://github.com/rmatuda)                     | 10               |
| 211031664   | [Catlen Cleane](https://github.com/catlenc)                     | 10               |
| 221008294   | [Luiza Maluf](https://github.com/LuizaMaluf)                    | 10               |  



### Histórico de Versões

| Versão | Data de Produção | Descrição da Alteração | Autor(es) | Revisor(es) | Data de Revisão |
|:------:|:----------------:|:----------------------:|:---------:|:-----------:|:--------------:|
| 1.0    | 06/07/2025       |Desenvolvimento de Relatorio de análise de desempenho |  [Mateus Bastos](https://github.com/MateuSansete) |[Rafael Kenji](https://github.com/rafa-kenji), [Luiza Maluf](https://github.com/LuizaMaluf) | 08/07/2025|







