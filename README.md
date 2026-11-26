# Dominó Clube

## Teste local
Instale Node.js 18 ou superior. Abra o terminal nesta pasta, execute `npm install` e `npm start`. Abra http://localhost:3000. Use outro navegador ou janela anônima para simular outro participante.

## Publicação no Render
1. Crie um repositório GitHub e envie os arquivos desta pasta (package.json, server.js, public/index.html e README.md), mantendo a pasta public.
2. No Render, crie um Web Service e conecte o repositório.
3. Runtime Node, Build Command `npm install`, Start Command `npm start`. Se disponível, escolha a instância gratuita.
4. Após o deploy, abra o endereço fornecido pelo Render. Crie uma sala e compartilhe o convite.

Não é necessário configurar banco de dados, Firebase ou Google Sheets. O servidor deve permanecer em uma única instância. Reinícios apagam salas e partidas. Salas sem participantes conectados são removidas após aproximadamente uma hora. Não há contas permanentes.

## Regras adotadas
28 pedras, sete por jogador. Duplas com assentos alternados. Maior carroça abre; se não houver, maior soma. Vencedor por batida ou menor soma de pedras restantes no fechamento; empate no fechamento não pontua. Pontos são a soma das pedras restantes dos adversários. Meta 50, 100 ou 200. Compra opcional para 2/3 jogadores; sem compra por padrão. As variantes regionais podem diferir. Robôs usam estratégia simples. O anfitrião inicia rodadas e revanche; vagas são completadas por robôs. Se alguém sair durante a rodada, deve reconectar para prosseguir. O convite não inclui senha.

## Versão 1.3
Atualize server.js e public/index.html (ou todos os arquivos). No Render, Manual Deploy > Deploy latest commit. Confira a identificação v1.3 no cabeçalho e use Ctrl+F5. A mesa utiliza a altura e largura disponíveis da janela, com trilha contínua, buchas transversais e pintas rotacionadas.

## v1.4
Corrigida a falha de renderização quando existe apenas uma pedra na mesa; o estado da partida continua sendo atualizado mesmo se o desenho falhar.

## V1.5
Cada rodada vencida vale um ponto. Primeiro a quatro vence; GATO quando todos os adversários estão zerados. Empate no fechamento não pontua. Atualize server.js e public/index.html.

## v1.6
O criador escolhe seu parceiro no lobby de duplas; os assentos são reorganizados antes da primeira rodada.

V1.7: destaque da última pedra do parceiro (amarelo) e da última jogada geral (azul), com legenda e reinício a cada rodada.

## v1.8
Remove os contornos amarelos das pontas. Somente a última pedra do parceiro recebe contorno amarelo e fundo destacado. Última jogada geral em azul, com prioridade ao amarelo quando coincidem. Apenas index.html foi alterado.
