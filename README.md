# Concurso educativo

Jogo de perguntas para a sala de aula, em progresso. O programa roda na máquina, sem depender de internet depois de instalado. Este repositório explica o que ele faz. O código completo e o instalador não estão aqui.

Para usar, copiar ou instalar o concurso é preciso uma licença de uso da STC FRANCO. O pedido pode ser feito em [stcfranco.com.br](https://stcfranco.com.br) ou pelo [WhatsApp](https://wa.me/5511959282551).

## O que o programa faz

É um aplicativo de mesa para a sala de aula. O professor monta listas de perguntas e o aluno joga um concurso em tela cheia, com tempo, prêmios e ajudas.

- Entrada com usuário e senha. A senha fica guardada com PBKDF2-HMAC-SHA256, não em texto aberto. Dá para lembrar a sessão e recuperar o acesso com uma pergunta.
- Painel com menu lateral, atalhos e a tabela das listas.
- Criar, editar, buscar e apagar listas de perguntas. Cada pergunta tem quatro opções, uma resposta certa e um nível de dificuldade.
- Usuários com papéis, tempo por pergunta e relatório das partidas.
- Jogo em tela cheia, com a escada de prêmios, cronômetro, 50:50, plateia e ligação para um amigo.
- Base SQLite só naquele computador. As listas e o histórico não vão sozinhos para outra máquina.

As matérias de exemplo do protótipo são biologia, história, matemática, geografia e cultura geral.

## Como está feito

- Python e Flet na interface.
- SQLite no disco do usuário do Windows.
- Pensado para Windows 10 e 11. A mesma ideia pode ir para macOS ou Linux, ainda sem esse pacote.
- A base fica numa pasta local do usuário, no Windows.
- O uso previsto é um computador por vez. Não há sincronização entre máquinas.
- Para a sala sem internet, a entrega é o programa empacotado, não este repositório.

## O que ainda falta

1. Modo apresentador e modo participante, com turnos ou equipes.
2. Importar e exportar Excel ou CSV, e exportar o resultado da partida.
3. Cópia de segurança e restauração pela própria tela.

Enquanto isso não fecha, o código-fonte completo fica fora do GitHub.
