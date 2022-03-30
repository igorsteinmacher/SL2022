## Chatbots nos Pull Requests

**TRABALHO EM GRUPO**

**Prazo:**: 04/04/2022 (Segunda)

**Como submeter**: Adicionar o código no GitHub e enviar um email para igorfs@utfpr.edu.br, com assunto 
"SL2022: Tarefa Chatbot" contendo o link para o repositório

Usando o código-fonte apresentado na sessão prática da Mairieli como ponto de partida, implemente o seguinte
recursos para o bot:

### 1. Agradeça quando uma solicitação pull for aceita (merged).

Faça o bot postar um comentário para agradecer, sempre que uma solicitação pull for aceita.

Para este caso, você desejará se inscrever no evento **pull_request**, especificamente quando o
ação para o evento **closed**.

Para referência, a documentação relevante da API do GitHub para o evento de pull request está aqui:
https://developer.github.com/v3/activity/events/types/#pullrequestevent

Observação: um pull request pode ser fechada sem que ele seja aceito (merged). Você terá que descobrir como
determinar se a solicitação pull foi merged ou simplesmente fechada (closed).

### 2. Exclua automaticamente uma ramificação mesclada.

Automatize tarefas ainda mais tediosas sempre que um pull request for aceito. Faça o
bot excluir automaticamente um branch que foi merged. O nome do branch pode ser encontrado no webhook do
evento pull request.

Assim como no exercício anterior, você precisará se inscrever no evento **pull_request**,
especificamente quando a ação para o evento é **closed**.



Para referência, a documentação relevante do GitHub para referências está aqui:
https://docs.github.com/en/rest/reference/git#references

Documentação relevante do PyGitHub:
https://pygithub.readthedocs.io/en/latest/github_objects/GitRef.html#github.GitRef.GitRef

