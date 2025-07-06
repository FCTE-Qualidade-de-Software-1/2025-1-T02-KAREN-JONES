# Teste de Usabilidade Agromart com Foco em Usabilidade

## 1. Login

- Tela inicial bem simples, com campos para e-mail e senha.

<div align="center">
  <img src="./assets/prints_usabilidade/image1.png" style="max-width: 800px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

- O sistema de autorização funciona bem, não permitindo login de usuários inexistentes.

<div align="center">
  <img src="./assets/prints_usabilidade/image6.png" style="max-width: 800px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

- **Ponto negativo:** o link de recuperação de senha não funciona e leva a uma página que não existe.

<div align="center">
  <img src="./assets/prints_usabilidade/image10.png" style="max-width: 400px; border: 1px solid #ccc; margin: 20px 0;" />
</div>
<div align="center">
  <img src="./assets/prints_usabilidade/image5.png" style="max-width: 600px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

- Boa responsividade: mesmo alterando o tamanho da tela, a área de login continua visível.

<div align="center">
  <img src="./assets/prints_usabilidade/image14.png" style="max-width: 500px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

---

## 2. Tela Principal

<div align="center">
  <img src="./assets/prints_usabilidade/image16.png" style="max-width: 600px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

- O botão de Logout está funcional, mesmo sem indicação visual clara.

<div align="center">
  <img src="./assets/prints_usabilidade/image11.png" style="max-width: 600px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

### 2.1 Barra Lateral

- A barra lateral funciona e possui animação de abertura.

<div align="center">
  <img src="./assets/prints_usabilidade/image4.png" style="max-width: 150px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

- **Problema:** não é responsiva, prejudicando usuários que não usam tela cheia.

<div align="center">
  <img src="./assets/prints_usabilidade/image12.png" style="max-width: 300px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

- O botão de notificação não executa nenhuma ação ao ser clicado.

<div align="center">
  <img src="./assets/prints_usabilidade/image3.png" style="max-width: 400px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

- O botão de cadastro redireciona corretamente para a tela de cadastro (avaliada no próximo tópico).

<div align="center">
  <img src="./assets/prints_usabilidade/image9.png" style="max-width: 400px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

- A seção de **Novas Notificações** exibe título, descrição e um botão que responde ao clique.

<div align="center">
  <img src="./assets/prints_usabilidade/image15.png" style="max-width: 400px; border: 1px solid #ccc; margin: 20px 0;" />
</div>
<div align="center">
  <img src="./assets/prints_usabilidade/image2.png" style="max-width: 400px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

- **Problema:** ao clicar, gera erro 405 (Method Not Allowed), não conseguindo realizar a ação pretendida.

<div align="center">
  <img src="./assets/prints_usabilidade/image13.png" style="max-width: 600px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

---

## 3. Tela de Cadastro

- A tela possui campos para nome, e-mail e senha, além de um botão para retornar à página principal.

<div align="center">
  <img src="./assets/prints_usabilidade/image17.png" style="max-width: 500px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

- O botão de envio aparenta executar a ação com feedback visual, mas **não registra o usuário** de fato.

<div align="center">
  <img src="./assets/prints_usabilidade/image7.png" style="max-width: 500px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

- A validação de senha está implementada, restringindo senhas com menos de 6 dígitos.

<div align="center">
  <img src="./assets/prints_usabilidade/image8.png" style="max-width: 400px; border: 1px solid #ccc; margin: 20px 0;" />
</div>

---

## Checklist De Avaliação

| Item Avaliado                | Evidência Coletada  | Aceitação    | Prioridade | Observações / Ação de Melhoria                  |
| --------------------------- | ------------------- | --------------- | ---------- | ----------------------------------------------- |
| Link de Recuperação de Senha | Teste funcional     | ❌ Não Aceito  | Alta       | Corrigir redirecionamento                       |
| Responsividade Login         | Inspeção visual     | ✅ Aceito      | Baixa      | -                                               |
| Botão de Logout              | Teste de fluxo      | ⚠️ Parcial     | Média      | Melhorar indicação visual do botão              |
| Barra Lateral                | Inspeção responsiva | ❌ Não Aceito  | Alta       | Ajustar exibição em telas menores               |
| Botão de Notificação         | Teste funcional     | ❌ Não Aceito  | Alta       | Implementar ação de abertura de notificação     |
| Cadastro de Usuário          | Teste de fluxo      | ❌ Não Aceito  | Alta       | Registro não salva no banco                     |
| Validação de Senha           | Teste de regra      | ✅ Aceito      | Baixa      | -                                               |
| Campo Novas Notificações     | Teste funcional     | ❌ Não Aceito  | Alta       | Corrigir erro 405 na ação                       |