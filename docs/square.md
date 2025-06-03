# __AE01 - SQuaRE__

## __Introdução__

O objetivo da avaliação é avaliar a corretude e confiabilidade do sistema AgroMart. Isso significa:

- Verificar se as funcionalidades estão sendo executadas corretamente, sem erros (corretude).
- Avaliar se o sistema é confiável e se comporta de forma estável durante o uso comum, mesmo em situações de carga normal ou leve (confiança).

Essa avaliação ajuda a garantir que os usuários, principalmente agricultores e consumidores, possam usar a plataforma sem enfrentar falhas, erros ou perdas de dados.

A norma ISO/IEC 25010 faz parte da família SQuaRE e define um modelo de qualidade para avaliação de produtos de software. Estabelece características e subcaracterísticas que auxiliam no desenvolvimento e análise da qualidade do software.

## __Aspectos da qualidade e ênfase__

|Aspecto da Qualidade | Ênfase <br> (1 a 5) | Justificativa |
| ----- | ------- | --------|
| Funcionalidade | 5 | Principal foco da avaliação: garantir que o sistema cumpra com seus objetivos e funcionalidades básicas sem erros. | 
| Confiabilidade | 4 | O sistema deve manter estabilidade e resistência a falhas durante o uso comum. |  
| Usabilidade  | 4 | O sistema será usado por produtores e vendedores, então a experiência do usuário é importante para adoção e uso eficaz. |
| Eficiência | 3 | Deseja-se que o sistema responda de forma razoavelmente rápida, mesmo com vários acessos simultâneos. |
| Portabilidade | 2 | Embora relevante, não é prioridade testar em muitos ambientes ou dispositivos, pois a versão web é o foco. | 
| Completitude | 2 | A cobertura total dos requisitos não é o principal objetivo neste momento da avaliação. | 





## __Confiabilidade__

A confiabilidade é o grau em que um sistema executa suas funções sob condições específicas por um período determinado.

Relacionada à capacidade do sistema de operar sem interrupções, garantindo confiança dos usuários e reduzindo custos com manutenção.

### __Subcaracterísticas da Confiabilidade__

- Maturidade: está associada à estabilidade do sistema em operação contínua, refletindo sua capacidade de minimizar falhas causadas por defeitos internos.
- Disponibilidade: está diretamente relacionada ao tempo em que o sistema permanece acessível e funcional, combinando a baixa frequência de falhas (maturidade) com a capacidade de recuperação
rápida.
- Tolerância a falhas: é a habilidade do sistema de manter operações
adequadas mesmo diante de problemas inesperados, como falhas de
hardware ou erros não detectados
- Recuperabilidade: significa que após uma falha, o sistema restaure rapidamente seu estado funcional e recupere dados afetados, minimizando impactos.

## __Métricas Associadas__

- Remoção de Falhas: Mede a proporção de falhas detectadas e corrigidas.
- Cobertura de Testes: Mede a quantidade de testes necessários para
validar o sistema.
- MTBF (Tempo Médio Entre Falhas): Mede a frequência de falhas do
software em operaçãMétricas Associadas

## __Outros aspectos relevantes__

### __Contextos de Aplicação__

A confiabilidade é essencial para softwares críticos, como sistemas bancários, aeroespaciais,
de saúde e automotivos, onde falhas podem ter impactos severos.

### __Importância para o Desenvolvimento e Avaliação de Software__

Uma alta confiabilidade reduz os custos de manutenção, melhora a experiência do usuário e aumenta a
segurança do software.

### __Desafios na Mensuração__

Os principais desafios incluem:
- Dificuldade em prever falhas antes da execução real do sistema.
- Necessidade de testes extensivos para garantir a maturidade.
- Medidas externas podem depender de condições ambientais variáveis.

### __Impacto na Experiência do Usuário__

A confiabilidade é um fator crítico para a satisfação do usuário, pois falhas
frequentes podem resultar em perda de clientes e danos à reputação da empresa.

### __Custo da falta de confiabilidade__ 

A ausência de confiabilidade pode resultar em altos custos operacionais,
multas regulatórias e perda de produtividade. Empresas que dependem de software crítico precisam investir fortemente em testes e monitoramento para garantir um funcionamento estável.


### __Confiabilidade em Software como Serviço__

Para os sistemas onde a disponibilidade contínua é fundamental, a confiabilidade se torna um aspecto ainda mais crítico. Problemas de confiabilidade podem resultar em indisponibilidade do serviço e afetar diretamente os clientes e os negócios.

## __Exemplo de aplicação prática__

A confiabilidade é uma característica essencial para garantir o funcionamento adequado de sistemas de software, especialmente em aplicações críticas. Para ilustrar sua importância e aplicação prática,
pode-se considerar o estudo “Development of a web-based learning application to enhance understanding in Philippine history”.

Nesse artigo, os pesquisadores desenvolveram um sistema de aprendizagem baseado na web para melhorar a compreensão da história das Filipinas, analisando sua qualidade com base nos critérios da norma ISO 25010. A confiabilidade foi avaliada a partir de métricas como disponibilidade, precisão dos dados e capacidade de resposta, fatores essenciais para assegurar a experiência do usuário.

A validação desses atributos foi feita com o algoritmo Locally Weighted Learning (LWL), que obteve uma taxa de precisão de 90% nos  testes realizados, demonstrando um alto nível de maturidade do software. Além disso, constatou-se que o sistema apresentava um tempo de resposta adequado e garantia de segurança na manipulação dos dados, reforçando sua confiabilidade.

Esse estudo destaca a importância da confiabilidade no desenvolvimento de softwares voltados para a educação, pois a disponibilidade contínua e a precisão dos dados são fundamentais para garantir uma boa experiência de aprendizado. O caso reforça a relevância das métricas descritas na ISO 25010 para medir e assegurar a qualidade de um sistema, especialmente no contexto de plataformas educacionais, onde interrupções ou falhas podem comprometer o ensino e a retenção do conhecimento.

---
> <a name="ref2">  </a> **SLIDES SQUARE**. Versão 1.0. - Autor: [Mateus Bastos](https://github.com/MateuSansete).  
[Visualizar PDF](./assets/pdf/square-slides.pdf)



---


## Tabela de contribuição:

| Matrícula   | Nome Completo                                                   | Contribuição (%) |
|-------------|------------------------------------------------------------------|-----------------|
| 211062240   | [Mateus Bastos](https://github.com/MateuSansete)                 | 20               |
| 190044128   | [Rafael Kenji Taira](https://github.com/rafa-kenji)             | 28              |
| 222006383   | [Rafael Matuda](https://github.com/rmatuda)                     | 18               |
| 211031664   | [Catlen Cleane](https://github.com/catlenc)                     | 14               |
| 221008294   | [Luiza Maluf](https://github.com/LuizaMaluf)                    | 20               |  

---

### Histórico de Versões

| Versão | Data de Produção | Descrição da Alteração         | Autor(es)                              | Revisor(es)                          | Data de Revisão |
|:------:|:----------------:|:------------------------------|:-------------------------------------|:-----------------------------------|:--------------:|
| 1.2    | 02/06/2025       | Adição da aba Square           | [Luiza Maluf](https://github.com/LuizaMaluf)                  | [Mateus Bastos](https://github.com/MateuSansete) | 02/06/2025     |
| 1.3    | 02/06/2025       | Adição de link do PDF do Square | [Mateus Bastos](https://github.com/MateuSansete) | [Luiza Maluf](https://github.com/LuizaMaluf)                  | 03/06/2025     |
