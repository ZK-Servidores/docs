# Corrigir Erro Retrying Public

Este problema acontece com usuários de operadoras que fazem a utilização de sistemas de **CG NAT \(Compartilhamento de IPs\)** ou até mesmo players quem jogam em vários PC na mesma rede.

Nós não temos como alterar nada disso, ou seja o problema, até onde sabemos, é quando tem muita gente dentro destes IPs compartilhados pela operadora que necessitam usar portas do jogo que já estão em uso por usuários no mesmo grupo de IPs.

Este problema acontece em MM e outros servidores da comunidade que tiverem muitos usuários jogando CS:GO porém é um problema aleatório, uma das soluções que funciona em vários casos é o `+clientport` e um numero aleatório entre **27001 até 27099**.

**Sigua o tutorial abaixo:** 

* Na **Steam**, vá ao menu **Biblioteca**, clique com o **botão direito no CS:GO**, vá em **Propriedades &gt; Geral &gt; clique no botão Definir Opções de Onicialização**.
* Adicione o seguinte comando: `+clientport 270XX` **\(no XX coloque um numero entre 01 e 99, o número inicial pode ser de 20 a 50, exemplo `+clientport 27040`\)** após inserir o comando clique em ok e abra o jogo.

![](../../.gitbook/assets/image%20%286%29.png)

_**OBS: Esta solução só funciona ao inicializar o jogo através do menu Biblioteca, fazer com jogo já aberto não funciona.**_

Tendo qualquer dúvida, problema não hesite em nos contatar!

