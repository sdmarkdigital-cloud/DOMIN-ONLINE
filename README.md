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
