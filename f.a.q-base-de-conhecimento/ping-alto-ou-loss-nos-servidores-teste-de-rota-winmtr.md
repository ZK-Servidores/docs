# Ping alto ou loss nos servidores (Teste de Rota - WinMTR)

Um problema muito comum é o ping alto nas partidas geralmente relacionado à **rota** das operadoras. Porém antes de iniciar os testes com o **WinMTR** verifique este [**tópico**](https://docs.zkservidores.com/f.a.q-base-de-conhecimento/corrigindo-problemas-de-loos-and-choke-alto-nos-servidores) e veja se resolve seu problema, caso não continue com os testes.

### **Fazendo teste de rota**

Para identificarmos onde está o problema e verificar se há solução, é necessário fazer um **teste de rota.**

*   Faça o download do programa [**WinMTR**](https://winmtr.br.uptodown.com/windows), depois coloque o endereço de IP do servidor que esta tendo problema no campo **`host` ** e clique em start.

    ```
    177.54.144.126
    ```
* Após 5 minutos, clique em "**STOP**", e nos encaminhe a print do programa, como exibido a seguir.

#### **Para entender como interpretar os testes, leia as informações a baixo.**

Na coluna ** **_**`Loss %` (Perda)**_, estes valores representam a porcentagem de perda de pacotes na rota da sua conexão. É importante entender que mesmo uma baixa porcentagem pode impactar negativamente sua jogabilidade, causando travamentos e rollbacks durante a partida. Se o valor estiver diferente de 0 nos últimos IPS pode ser esse a causa dos seus problemas **(travamentos e rollbacks)**.

![](<../.gitbook/assets/image (29).png>)

Nas colunas **`Sent`** e **`Recv`  **_**(Enviados e Recebidos)**_ estes valores demonstram o número de pacotes enviados e recebidos durante o teste. Se você estiver com Loss, com certeza o número de pacotes recebidos será menor do que os de enviados.

![](<../.gitbook/assets/image (30).png>)

As outras 4 colunas informam:

* **Best**, **o melhor ping** identificado durante o teste;
* **Avrg**, **o ping médio** identificado durante o teste;
* **Worst**, **o pior ping** identificado durante o teste;
* **Last**, **o último ping** registrado durante o teste;

![](<../.gitbook/assets/image (27).png>)

A alta variação de valores nessas colunas também podem indicar uma instabilidade em sua rota!

<mark style="color:yellow;">**OBS: Se você enfrentar o erro “unknown hostname” verifique se o endereço de IP no campo host está correto. Geralmente isso acontece quando há espaços ou barras no IP.**</mark>

<mark style="color:yellow;">**Se não funcionar, tente desativar o Anti-Vírus, Windows Defender e o Firewall, depois reiniciar o programa WinMTR.**</mark>
