# Lynfort — Phishing Simulation Lab

Laboratório educacional de conscientização sobre phishing, desenvolvido como projeto de aprendizagem e portfólio técnico da Lynfort.

## Objetivo

Demonstrar sinais de mensagens suspeitas por meio de um cenário corporativo fictício e uma página educativa.

## Funcionalidades atuais

- Mensagem fictícia de atualização cadastral.
- Navegação da mensagem para uma página educativa.
- Explicação dos sinais suspeitos e orientações de verificação e denúncia.
- Link de retorno à mensagem.
- Layout adaptável à largura da janela.
- Navegação do link por teclado.

## Cenário

A empresa fictícia Aurora Comércio é o contexto de uma mensagem que solicita atualização cadastral urgente, sob ameaça de suspensão do acesso.

O planejamento prevê 10 colaboradores fictícios, identificados de COL-01 a COL-10. Nesta versão, eles representam apenas o cenário: não há contas, envio de mensagens ou acompanhamento individual.

## Tecnologias

- HTML e CSS.
- Python 3 para servir os arquivos localmente.
- Git para versionamento.
- Kali Linux em máquina virtual no VirtualBox.

## Como executar

É necessário ter Python 3 instalado.

Abra um terminal na pasta principal do projeto e execute:

```bash
python3 -m http.server 8000 --bind 127.0.0.1 --directory lab/paginas
```

No navegador da mesma máquina, acesse:

http://127.0.0.1:8000/mensagem.html

Mantenha o terminal aberto durante o uso. Para encerrar o servidor, pressione **Ctrl + C**.

Após reiniciar a máquina virtual, execute novamente o comando a partir da pasta principal do projeto.

## Estrutura principal

```text
lynfort-phishing-simulation-lab/
├── README.md
├── lab/
│   ├── paginas/
│   │   ├── index.html
│   │   └── mensagem.html
│   └── cenarios/
│       └── cenario-01.md
└── screenshots/
```

## Testes realizados

Validação manual no navegador do Kali Linux:

- Abertura da mensagem simulada.
- Navegação para a página educativa.
- Exibição das orientações.
- Retorno à mensagem.
- Leitura com janela reduzida, sem cortes ou rolagem horizontal.
- Destaque do link com Tab e ativação com Enter.

Os testes verificam o funcionamento da interface. Não medem aprendizagem nem comportamento de participantes.

## Evidências e documentação

As capturas de tela estão na pasta [screenshots](screenshots/).

O roteiro e os resultados estão na [descrição do cenário](lab/cenarios/cenario-01.md).

## Escopo e limites

- Empresa e mensagem fictícias.
- Nenhum envio de e-mail.
- Nenhuma solicitação ou coleta de senhas.
- Nenhum rastreamento individual.
- Nenhuma métrica de envio, entrega ou clique.
- Servidor configurado para acesso somente na própria máquina, em 127.0.0.1.

## Próximas etapas

- Organizar a documentação da arquitetura e metodologia.
- Acrescentar exercícios de identificação de sinais suspeitos.
- Avaliar métricas com dados sintéticos.
- Estudar ferramentas de simulação em ambiente autorizado.

## Referência de estudo

O desafio abaixo foi utilizado como referência educacional. A implementação deste laboratório foi desenvolvida separadamente.

[Desafio de phishing — brenoluizdev](https://github.com/brenoluizdev/cibersecurity-desafio-phishing)



