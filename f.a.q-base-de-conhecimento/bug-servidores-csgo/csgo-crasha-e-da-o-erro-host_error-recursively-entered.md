# Corrigir Erro HOST\_ERROR RECURSIVELY ENTERED

Verificando na Deep Web isso se trata de um erro de IPV4 e/ou IPV6, solução que encontramos, resetar eles.

Então siga esses passos e veja se resolve:

**Primeiro de tudo, dele o mapa de seu CSGO que esta causando este problema. Caso não saiba como, recomendamos da uma** [**lida aqui**](https://docs.zkservidores.com/f.a.q-base-de-conhecimento/bug-servidores-csgo/jogo-fecha-sozinho-ao-tentar-me-conectar-nos-servidores)**.**

* Abra seu **Prompt de Comando como Administrador**, segue uma print de exemplo: 

![Prompt de Comand](../../.gitbook/assets/image%20%286%29.png)

* Aberto seu **CMD** digite esses comandos um por um e aperte enter: 
  * **`ipconfig /flushdns`**
  * **`netsh int ipv4 reset`**
  * **`netsh int ipv6 reset`**
  * **`netsh winhttp reset`**
  * **`proxy netsh winsock reset`**
  * **`ipconfig /registerdns`**
* Abra agora o **Executar**, segue um print de exemplo: 

![OBS: Caso queira um atalho, basta clicar em seu teclado Win+R.](../../.gitbook/assets/image%20%285%29.png)

Feito isso digite o comando dentro do **Executar:** `steam://flushconfig`

![](../../.gitbook/assets/image%20%282%29.png)

Geralmente depois de tudo feito ainda é preciso reiniciar o computador.

Finalizado, teste novamente se conectando no servidor. 

Tendo qualquer dúvida, problema não hesite em nos contatar!

_**Obrigado ao @\[💎\] Alimento=Cachaça\| MOD \| pelo feedback.**_ 😘 

