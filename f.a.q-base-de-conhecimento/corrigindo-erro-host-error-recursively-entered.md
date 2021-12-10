# Corrigindo erro Host\_Error: recursively entered

Depois de investigar esse problema específico completamente, descobrimos que existem vários cenários diferentes em potencial que podem acionar esse código de erro específico:

* **Arquivos de instalação corrompidos** - Esse erro pode ser causado por um arquivo de instalação do jogo ausente ou corrompido. Isso faz com que o jogo trave e _(em alguns casos)_ até mesmo bugs que travem o jogo durante o tempo de jogo. Felizmente, a Steam tem uma opção que verifica a integridade dos arquivos do jogo e, se detectar arquivos inválidos, irá readquirir os arquivos. Além disso, você pode reinstalar o jogo se não estiver iniciando o jogo pela Steam.
* **Arquivo de mapa corrompido** - Maioria das vezes, esse problema específico também pode ser causado por um arquivo de **mapa personalizado** que está corrompido e não pode ser renderizado dentro do CS:GO. Vários usuários afetados que lidaram com esse problema específico relataram que o problema foi finalmente resolvido depois que excluíram o mapa dos arquivos do jogo.
* **Dados TCP / IP inconsistentes** - Um cache DNS mal armazenado ou um problema com os dados TCP ou IP também pode produzir esse erro específico quando você tenta ingressar em jogos online fora de sua rede local. Nesse caso, você deve ser capaz de resolver o problema realizando uma redefinição do Winsock e liberando os flushing DNS.
* **Dados de cache do Steam mal armazenados** - De acordo com alguns usuários afetados, esse problema também pode aparecer se você estiver lidando com um caso de dados mal armazenados em cache atualmente armazenados pela Steam. Nesse caso, limpar a configuração da Steam permitirá que você resolva o problema na maioria dos casos.

Agora que você está ciente dos cenários possíveis, aqui está uma lista de métodos que podem ajudá-lo a corrigir o **Host\_Error: recursively entered** ao iniciar o Counter-Strike: Global Offensive.

### **Método 1 - Verificar integridade dos arquivos CSGO via Steam**

* Depois de abrir o aplicativo **Steam**, vá para a página da **Biblioteca** do jogo.
* Clique com o botão direito em **CS:GO** e abra o menu **Propriedades**.

![](<../.gitbook/assets/image (13).png>)

* Depois que o menu **Propriedades** aparecer na tela, clique em **Arquivos locais,** que fica do lado esquerdo.
* Em seguida, inicie a verificação clicando em **Verificar integridade dos arquivos do jogo** e aguarde até que seja concluída.

![](<../.gitbook/assets/image (14).png>)

* Depois que a verificação for concluída, uma mensagem aparecerá e dirá se houver arquivos inválidos. Se os arquivos não forem validados, eles serão readquiridos.

Se este método não corrigiu o erro, verifique abaixo o próximo.

### **Método 2 - Excluir o mapa dos arquivos do jogo**

Alguns players relataram que certos arquivos de mapa podem estar corrompidos e, por causa disso, o erro **`host_error recursively entered`** aparece e bloqueia o jogo. A correção que eles usaram é simples - **exclua o mapa dos arquivos do jogo e depois que você entrar novamente no servidor, ele fará o download do mapa automaticamente**.

Aqui estão as etapas para excluir o mapa dos arquivos do jogo:

* Vá para a **Biblioteca** do jogo no Steam, clique com o botão direito em **CS:GO** e mova o cursor para **Gerenciar.**
* Depois de fazer isso, clique em **Procurar arquivos locais.**

![](<../.gitbook/assets/image (15).png>)

* Depois que a pasta do jogo aparecer na tela, acesse a pasta chamada **`csgo`**. Dentro dessa pasta está a localização da pasta onde todos os mapas são armazenados, sendo denominados **`maps`.**

![](<../.gitbook/assets/image (16).png>)

* Acesse a pasta de mapas e, nessa lista de mapas, pesquise o mapa específico que está no servidor ao qual você está tentando ingressar.
* Depois de localizar o mapa delete o mesmo da pasta. _**(Recomendamos deletar todos arquivos que tenham o nome do mapa na pasta)**_
* Em seguida, abra o CS:GO e tente entrar no servidor novamente para ver se ainda encontra o erro.

Se esta solução também não resolveu o seu problema, verifique abaixo o próximo.

### **Método 3 - Resetando Winsock, Flushing DNS & Steam**

Muitos players afetados de CS:GO relataram que não conseguiram se conectar aos servidores da comunidade devido a dados temporários de TCP ou IP inválidos, que afetam a estabilidade da conexão com a Internet. Como resultado, o **`Host_Error Recursively Entered`** aparece quando você tenta se conectar em certos servidores.

Alguns players que encontraram esse erro relataram que a correção consiste na execução de um procedimento de reset do Winsock completo a partir de um prompt de comando.

_**NOTA: Comando Winsock Reset irá essencialmente redefinir configurações de rede importantes para seus valores padrão. Aqui estão as etapas sobre como realizar um procedimento de redefinição do Winsock.**_

1. Pressione a tecla **Windows + R** para abrir uma caixa de diálogo **Executar**. Em seguida, dentro da caixa, digite **`cmd`** e pressione **`Ctrl + Shift + Enter`** para abrir um Prompt de Comando com privilégios de administrador. Depois disso, você precisará clicar em **Sim** para conceder acesso de administrador.
2.  Depois que o prompt de comando aparecer na tela, digite os seguintes comandos em ordem e pressione **Enter** após cada comando que usar:

    ```
    ipconfig /flushdns
    netsh int ipv4 reset
    netsh int ipv6 reset
    netsh winhttp reset proxy
    netsh winsock reset
    ipconfig /registerdns
    ```
3. Depois de certificar-se de que todos os comandos foram processados ​​com êxito, feche o Prompt de Comando.
4. Em seguida, reinicie o PC e depois que ele inicializar, abra o CS:GO novamente e teste-o para ver se o erro **Host\_Error Recursively Entered** ainda ocorre.

### \*\*Limpando Cache Steam \*\*

Lembre-se de limpar o cache steam também, para isso siga estas etapas:

* Pressione a tecla **Windows + R** para abrir uma caixa de diálogo **Executar**. Depois disso, digite na caixa **`steam://flushconfig`** e pressione **Enter** para prosseguir com a ação.

![](<../.gitbook/assets/image (17).png>)

* Depois que a janela **Steam - Limpar dados de download** for exibida na tela, clique em **OK** para limpar o cache de download local.

![](<../.gitbook/assets/image (18).png>)

* Depois de fazer isso, abra a **Steam** novamente e faça login com sua conta.
* Depois de fazer login, inicie o jogo e teste-o para ver se você ainda encontra o erro **Host\_Error Recursively Entered** ao iniciar o **CS:GO.**

Se nenhum dos métodos mencionados antes corrigiu o erro, em ultimo caso somente desinstalando e instalando o game para corrigir.

Qualquer dúvida não hesite em nos contatar!
