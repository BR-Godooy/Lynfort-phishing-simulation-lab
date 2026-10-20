# Cenário 01 — Aviso de atualização cadastral

## Ambiente
Empresa fictícia: Aurora Comércio
Participantes simulados: 10, identificados de COL-01 a COL-10.

## Objetivo
Ensinar a identificar urgência artificial, remetente suspeito
e solicitações inesperadas de atualização cadastral.

## Mensagem fictícia
Remetente: Suporte <suporte@aurora.example>
Assunto: Ação urgente: atualize seu cadastro hoje

Olá,

Seu cadastro precisa ser atualizado até o fim do dia.
Acesse o link abaixo para evitar a suspensão do acesso.

[Revisar cadastro — link para a página local de treinamento]

Equipe de Suporte

## Execução
A mensagem será apresentada como exemplo dentro do laboratório.
Não haverá envio de e-mails nesta etapa.
O link abrirá a página educativa em http://127.0.0.1:8000.

## Sinais para discussão
- Pressão para agir rapidamente.
- Ameaça de suspensão de acesso.
- Pedido inesperado que deve ser confirmado por outro canal.
- Necessidade de verificar o destino do link.

O endereço usa o domínio reservado .example para representar
uma organização fictícia. Em uma situação real, o remetente
deve ser comparado com os canais oficiais da organização.

## Critérios de conclusão
- Página educativa abre no navegador do Kali.
- Página explica os sinais suspeitos.
- Nenhum dado pessoal ou senha é solicitado.
- Evidência visual é salva na pasta screenshots.

## Resultados
Ainda não executado como cenário completo.
Não há métricas de envio, clique ou participação nesta versão.

## Validação da página educativa

Testes manuais realizados no navegador do Kali Linux.

- Mensagem simulada abriu corretamente.
- Botão "Revisar cadastro" abriu a página educativa.
- Conteúdo e orientações apareceram corretamente.
- Link de retorno abriu a mensagem simulada.
- Janela reduzida manteve o conteúdo legível, sem cortes
  ou rolagem horizontal.
- Link de retorno recebeu destaque com Tab e funcionou com Enter.

Todos os testes acima passaram.

## Evidências

Capturas da página educativa, em ordem de leitura:

- screenshots/pagina-educativa-01.png
- screenshots/pagina-educativa-02.png
- screenshots/pagina-educativa-03.png
