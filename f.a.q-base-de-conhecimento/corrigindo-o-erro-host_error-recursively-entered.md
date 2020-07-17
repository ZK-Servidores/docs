# Corrigindo o erro Host\_error recursively entered

Vamos por parte, tente um por vez e veja se resolve o problema.  
  
Primeiro, desligue o roteador / modem da tomada por alguns minutos e ligue-o novamente. Feito isso tente entrar novamente no servidor.

**OPCIONAL -** Caso o problema continue **REMOVA** _**\(ou seja, REMOVER e não desativar\)**_ Antivírus!

Se até aqui seu problema não foi resolvido vamos redefinir sua rede, para isso siga este tutorial abaixo.

Inicie seu **Prompt de Comando** como **Administrador**.

![](../.gitbook/assets/image%20%286%29.png)

E execute os comandos abaixo um por um:

* **ipconfig /flushdns**
* **netsh int ipv4 reset**
* **netsh int ipv6 reset**
* **netsh winhttp reset proxy**
* **netsh winsock reset**
* **ipconfig /registerdns**

Feito isso redefina sua steam, para isso basta digitar ****`steam://flushconfig` no **Executar.**

![Tecla Windows + R](../.gitbook/assets/image%20%288%29.png)

Depois basta reinicia seu windows e veja se seu problema foi resolvido.

Caso o problema persista entre em contato conosco.

