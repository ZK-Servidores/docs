# Corrigindo o erro "Retrying Public"

Isso acontece por conta das operadoras que utilizam o sistema de **CGNAT** _**\(compartilhamento de IPs\)**_. Seria como se estivesse em uma lan house e todos estivessem tentando conectar na mesma partida, o server barraria os outros 9 players por utilizarem o mesmo IP de alguém que já está lá, já esta conectado.

Caso o tutorial não resolva tente contatar sua provedora e verifique a possibilidade de remoção do CGNAT ou abertura de pedido para um IP fixo na residência.

Lembrando que não temos controle quanto a esses casos, quando o problema é no servidor, nenhum jogador consegue se conectar à partida.

Para tentar resolver o problema você tem duas opções:

* Reiniciar seu modem e/ou roteador;
* Atribuir o comando**`+clientport`** nas opções de inicialização do CSGO;

Para adicionar o comando nas opções de inicialização do CSGO, siga este exemplo:

![Op&#xE7;&#xF5;es de inicializa&#xE7;&#xE3;o CSGO](../.gitbook/assets/corrigindo-o-erro-retrying-public.gif)

* Abra a biblioteca de jogos na Steam e clique com o botão direito no **Counter-Strike: Global Offensive** e escolha a opção **Propriedades,** depois vá em **Opções de inicialização**.
* Adicione o comando **`+clientport XX0YY`** no lugar do **XX** coloque um numero entre 20 e 50 e no lugar do **YY** coloque um numero entre 0 e 99.
* Depois abra o CSGO e tente novamente se conectar no servidor.

