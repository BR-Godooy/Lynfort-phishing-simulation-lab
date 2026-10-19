# Cenário 01 — Aviso de atualização cadastral

## Ambiente

- Projeto: Lynfort — Phishing Simulation Lab.
- Empresa fictícia: Aurora Comércio.
- Participantes fictícios: 10, identificados de COL-01 a COL-10.
- Ambiente de teste: Kali Linux em máquina virtual.
- Acesso: navegador na própria máquina virtual.

Os participantes representam o cenário planejado.
Nesta etapa, não houve participação de pessoas nem envio de mensagens.

## Objetivo

Ensinar a reconhecer urgência artificial, ameaça de suspensão
e solicitações inesperadas de atualização cadastral.

## Mensagem fictícia

Remetente: Suporte <suporte@aurora.example>

Assunto: Ação urgente: atualize seu cadastro hoje

Olá,

Seu cadastro precisa ser atualizado até o fim do dia.
Acesse o link abaixo para evitar a suspensão do acesso.

[Revisar cadastro]

Equipe de Suporte

## Fluxo do exercício

1. Abrir a mensagem fictícia no navegador:
   http://127.0.0.1:8000/mensagem.html
2. Observar o remetente, o assunto e o conteúdo.
3. Clicar no botão "Revisar cadastro".
4. Ler as orientações na página educativa index.html.

O domínio .example é reservado para exemplos.
O endereço de e-mail apresentado é fictício.

## Sinais para discussão

- Urgência: prazo curto para realizar uma ação.
- Ameaça: possibilidade de suspensão do acesso.
- Solicitação inesperada: atualização sem contexto anterior.
- Remetente: conferir o endereço completo e confirmar por canal conhecido.
- Link: verificar o destino antes de abrir.

Esses sinais justificam uma verificação.
Isoladamente, não comprovam que uma mensagem seja maliciosa.

## Limites desta versão

- Nenhum e-mail é enviado.
- Nenhuma senha ou dado pessoal é solicitado.
- Não há formulário de autenticação.
- Não há rastreamento individual de participantes.
- Não há métricas de envio, entrega ou clique.
- O servidor atende somente na própria máquina, em 127.0.0.1.

## Como iniciar

Na pasta principal do projeto, executar:

python3 -m http.server 8000 --bind 127.0.0.1 --directory lab/paginas

Manter o terminal aberto durante o teste.
Para encerrar o servidor, pressionar Ctrl + C.

## Critérios de conclusão

- A mensagem fictícia abre no navegador.
- O botão abre a página educativa.
- A página apresenta orientações sobre phishing.
- Nenhuma informação pessoal é solicitada.

## Resultados

Teste manual realizado no Kali Linux.

- A mensagem simulada abriu em /mensagem.html.
- O botão "Revisar cadastro" abriu a página educativa.
- Nenhuma senha ou dado pessoal foi solicitado.
- Nenhum e-mail foi enviado.

O fluxo de navegação funcionou.
Este teste verifica a navegação, sem medir aprendizagem
ou comportamento de participantes.

## Evidências

Capturas previstas na pasta screenshots:

- primeira-pagina-lynfort.png
- mensagem-simulada-lynfort.png

Confirmar a presença dos arquivos antes de publicar o projeto.
