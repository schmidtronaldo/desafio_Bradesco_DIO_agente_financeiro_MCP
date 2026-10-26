# desafio_Bradesco_DIO_agente_financeiro_MCP
Criando um agente financeiro com MCP

<p>
  Entendendo o Desafio
Agora é a sua hora de praticar, aprender fazendo e levar o banco para onde o cliente já está: uma conversa em que um assistente responde em português sobre contas, saldos e transações, com os dados chegando por MCP.

Materiais do Desafio:
Apresentação da aula
Guia prático

Nas Aulas, o Expert Bruno Lima conecta o Codex à Pluggy e à Plaid e termina com um chat publicado no Lovable. Os slides trazem os prompts de cada prática, e o guia detalha cada configuração, os erros comuns e a especificação do chat.

O Que Criar
Um web app em formato de chat que responde sobre um banco de teste. O MCP é a tomada padrão entre a IA e as fontes externas: a Pluggy explica a integração brasileira pela documentação, a Plaid fornece dados fictícios, e a IA organiza tudo em linguagem simples.

O Expert entrega esse chat como um app de banco. Você escolhe onde o seu cliente já está: ali, ou no app de outra indústria, como uma loja ou uma agência de viagem, na hora da decisão financeira.

Como Fazer
Não há repositório base. Você refaz do zero o caminho do Expert, com os slides e o guia abertos ao lado:

Conecte a Pluggy. Nas configurações de MCP da sua IA, o Codex ou outra, adicione um servidor Streamable HTTP com a URL https://mcp.pluggy.ai/mcp, sem chave. Confira com /mcp e peça que a IA explique o que é um Item, com as fontes;
Prepare a Plaid. Copie o Client ID e o secret de Sandbox em Developers, Keys, instale o uv e adicione o servidor mcp-server-plaid, do tipo STDIO, com o caminho do uvx no comando e as duas chaves como variáveis de ambiente;
Consulte o banco fictício. Crie um Item de teste, leia contas, saldos e transações e peça tabelas com três padrões de gasto. Na Plaid, valor positivo é saída;
Construa o chat no Lovable. Cole a especificação das páginas 25 a 28 do guia, com o seu nome e o seu cenário no lugar do que aparece desfocado, ou peça à IA um prompt no formato OpenSpec, como o Expert. Mande primeiro no modo chat, para tirar as dúvidas, e publique.
O guia foi feito num Mac, então caminhos e atalhos mudam no seu computador, e a página 23 resolve os erros mais comuns. A Plaid é só um laboratório: não representa o Open Finance brasileiro, que em produção exige consentimento e segurança.

Ideias para Evoluir
Responder perguntas novas, como gasto por categoria, período ou conta;
Mostrar os valores também em reais, com a conversão declarada;
Transformar a configuração dos servidores numa skill de agente;
Receber avisos por webhook, como na página 18 do guia, e levá-los ao cliente por push, SMS ou WhatsApp;
Fazer a Etapa 2 da especificação, um backend com as chaves só no servidor.
Se você ainda está começando, tudo bem. O Expert monta tudo sem escrever código, pedindo cada passo à IA. Um chat da Etapa 1 do guia, com dados locais e bem explicado, vale mais que uma integração pela metade.

Uma Ajuda durante o Caminho
Se o caminho de uma resposta não ficar claro, o DIO Agent ajuda a entender:

Estou montando um chat financeiro com MCP, usando a documentação da Pluggy e os dados de sandbox da Plaid.
Me ajude a entender o caminho de uma pergunta como "qual é o meu saldo?", da ferramenta chamada até a resposta.
Quero entender também por que o saldo de um cartão aparece como dívida.

Importante: não quero uma resposta pronta para copiar.
Quero entender o processo e construir o meu assistente.
O Que Entregar
Publique o web app e crie um repositório na sua conta do GitHub, para onde o Lovable exporta o código. No README.md, explique:

Onde o seu cliente já está, o que o assistente responde ali, e de onde vem cada dado;
Como configurar os servidores MCP da Pluggy e da Plaid;
A especificação ou o prompt mandado ao Lovable, e o que ajustou depois;
A melhoria escolhida, e o endereço do app publicado.
Print das tabelas na sua IA e da conversa no app contam muito: evidência de que tudo funciona é o que mais pesa no portfólio.

Antes de submeter, confira:

O app está publicado e avisa que os dados são fictícios;
Nenhuma chave, token ou senha ficou versionada ou aparece em print;
Todo arquivo e pasta citada no README existem e têm conteúdo;
O link enviado é o do repositório, não o do app nem o de um arquivo;
O repositório está na sua conta e público;
O nome do repositório ficou legível, em minúsculas e sem acento.
Resultado Esperado
Ao final, você terá no portfólio um assistente financeiro no ar, que leva o banco até onde o cliente já está, e um README que mostra o caminho de cada resposta, da pergunta até o endpoint.

Bons estudos e bom projeto 🚀
</p>
