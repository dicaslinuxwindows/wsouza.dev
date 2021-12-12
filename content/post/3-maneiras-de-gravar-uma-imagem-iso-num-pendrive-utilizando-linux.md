---
title: '3 maneiras de gravar uma imagem ISO num pendrive utilizando Linux'
date: 2020-04-20T02:17:00.002-03:00
draft: false
url: /2020/04/3-maneiras-de-gravar-uma-imagem-iso-num-pendrive-utilizando-linux.html
tags: 
- Linux
- Ubuntu
- Tutoriais Debian
- Ferramentas Linux
---

![3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux - Dicas Linux e Windows](https://1.bp.blogspot.com/-BvVHCc2Py6c/Xuq7ibvvA-I/AAAAAAAAPIc/zq_t2NWaIXMBfRc5BbQwxbiVJwAmxqGMQCNcBGAsYHQ/s1600/Pendrive_Linux.png "3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux - Dicas Linux e Windows")

Nesta matéria mostro 3 opções para gravar imagens ISO num pendrive, tornando possível "rodar" sua distribuição Linux diretamente nele.

  
  
  
  
  
  
  

### Se preferir, vá direto ao tutorial.

  
[DD](https://info.wsouza.com.br/2020/04/3-maneiras-de-gravar-uma-imagem-iso-num-pendrive-utilizando-linux.html#dd)  
[UNETbootin](https://info.wsouza.com.br/2020/04/3-maneiras-de-gravar-uma-imagem-iso-num-pendrive-utilizando-linux.html#unetbootin)  
[Etcher](https://info.wsouza.com.br/2020/04/3-maneiras-de-gravar-uma-imagem-iso-num-pendrive-utilizando-linux.html#etcher)

  
  

### Por que eu preciso disso?

  
Devido à ausência de drives de DVD nos notebooks mais recentes tornou-se ainda mais necessária a utilização de pendrives para gerar um pendrive bootável _(Live USB)_ e iniciar o sistema a partir dele, ou mesmo criar uma imagem de instalação. Há tempos atrás isso era feito em Cds ou DVDs, que eram facilmente gravados em qualquer software gravador de CD/DVD, sempre disponível em qualquer sistema. A utilização do pendrive trouxe, entre outras vantagens, o ganho de velocidade quando utilizado o sistema rodando a partir dele.  
Diferente dos gravadores de CD/DVD, que como citei anteriormente, estavam disponíveis _(ou eram facilmente encontrados)_ em qualquer sistema operacional, os softwares para gravar uma ISO num pendrive nem sempre estão acessíveis. Veja a seguir 3 opções para criar uma Live USB.  
  
[](https://draft.blogger.com/null)  

### DD

  
O dd é uma ferramenta que tem diversas utilidades como cópia de partições, discos inteiros, da MBR, etc...  
Uma das mais interessantes funções desta poderosa ferramenta é permitir a gravação de imagens ISO num pendrive, ideal para criar um Live USB.  
Tudo é executado no terminal de maneira bem simples. Para iniciar insira um pendrive no computador. Após, abra o terminal e logue como super usuário com o comando abaixo:  
  

 sudo su

  
Com o comando abaixo podemos identificar o caminho do pendrive que será utilizado.  
  

 lsblk

  
É importante saber exatamente o caminho correto pois, se escolher o caminho incorreto, você poderá gravar no disco onde o sistema está instalado. Se não conseguiu identificar na primeira tentativa, experimente tirar o pendrive, executar o comando e ver o que aparece. Depois, insira o pendrive e veja o que apareceu de diferente e isto será o que está procurando. Nota: No exemplo abaixo é mostrado sdb e sdb1, onde sdb1 pode ser uma partição. Sempre utilize o dispositivo sem indicar a partição, neste caso, _/sdb_.  
  

 NAME MAJ:MIN RM SIZE RO TYPE MOUNTPOINT  
 sda 8:0 0 931,5G 0 disk  
 ├─sda1 8:1 0 260M 0 part  
 ├─sda2 8:2 0 16M 0 part  
 ├─sda3 8:3 0 583,4G 0 part  
 ├─sda4 8:4 0 850M 0 part  
 ├─sda5 8:5 0 16,1G 0 part  
 ├─sda6 8:6 0 1G 0 part  
 ├─sda7 8:7 0 286G 0 part /media/Dados  
 ├─sda8 8:8 0 40G 0 part /  
 └─sda9 8:9 0 4G 0 part \[SWAP\]  
  sdb 8:16 1 7,5G 0 disk  
 └─sdb1 8:17 1 7,5G 0 part  

  
O pendrive precisa estar formatado no formato fat32, faça isto com o comando abaixo.  
  

 mkfs.vfat /dev/sdb -I

  
Após identificar o caminho, vamos executar o dd e finalmente gravar a ISO no pendrive. Ainda no terminal, rode o comando a seguir.  
  

 dd if=/home/dlw/debian-live-10.3.0-amd64-cinnamon.iso of=/dev/sdb status=progress && sync

  
Sobre a sintaxe do comando:  

*   dd if= é o caminho de origem, onde está a ISO que deseja gravar;
*   dd of= é o caminho de destino. É o local onde está o pendrive que receberá a ISO e que foi identificado no passo anterior;
*   status=progress - mostra o progresso da gravação;
*   sync - copia os dados imediatamente para o pendrive.

O tempo de duração depende de alguns fatores, principalmente do tamanho da imagem ISO escolhida. Aguarde até o final e se a saída for parecida com a saída abaixo significa que deu tudo certo.  
  

 4896000+0 registros de entrada  
 4896000+0 registros de saída  
 2506752000 bytes (2,5 GB, 2,3 GiB) copiados, 1465,48 s, 1,7 MB/s

  
  
[](https://draft.blogger.com/null)  

### UNetbootin

  
Diferente do dd, que funciona no terminal, o UNetbootin é uma ferramenta que possui uma interface gráfica e possui a função de gerar um Live USB.  
Vá ao site oficial [https://unetbootin.github.io](https://unetbootin.github.io/linux_download.html) e faça o download na arquitetura que desejar _(32 ou 64 bits)_. A versão utilizada neste tutorial foi a _.bin_, que é bem simples de executar e não necessita instalação.  
Para executar o programa é preciso dar permissão de execução. Supondo que o programa foi baixado na pasta _Downloads_ execute o comando abaixo. _(Troque o que está em vermelho pelo nome do arquivo baixado)_  
  

 sudo chmod +x Downloads/unetbootin-linux64-677.bin

  
Como o UNetbootin só permite a execução utilizando o superusuário _(root)_, quando buscamos a ISO apenas a pasta /root é habilitada, não permitindo a busca nas outras pastas. A maneira mais simples que encontrei para contornar este problema: Crie um link da pasta onde está a ISO, apontando para a pasta /root/. Supondo que você tenha uma pasta chamada ISOS em sua home _(/home/seu-nome-de-usuario/ISOS/)_ faça da seguinte maneira:  
  

 sudo ln -s $HOME/ISOS/ /root/

  
O comando abaixo executa o UNetbootin. _(Não feche o terminal, pois o UNetbootin será fechado também)._  
  

 sudo ./Downloads/unetbootin-linux64-677.bin

  
Eis a tela principal do programa. Temos duas opções para gravar o pendrive Live USB. A primeira é baixar a ISO _(Na opção distribuição escolha a que preferir)_, porém, é uma opção demorada e acho que não vale a pena, portanto, vamos à 2º opção. Utilizaremos uma ISO que já foi baixada anteriormente.  

*   Em _"Imagem de disco"_ escolha a opção ISO, clique nos 3 pontos para procurar e selecione a ISO desejada;
*   Se você estiver fazendo uma Live USB do Ubuntu, na opção _"Espaço usado para preservar os arquivos após a reinicialização"_ defina um valor (ex: 512 Mb, 1024 Mb...). Assim você poderá salvar arquivos no Live USB para utilizá-los num outro momento após reiniciar o sistema rodando no Live USB. Esta função é conhecida como persistência;
*   Na opção _Tipo_ escolha Unidade USB e na opção _Unidade_ escolha o pendrive _(que precisa estar formatado)_. Após o _"Ok"_ o processo será iniciado.

  

[![3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux - Dicas Linux e Windows](https://1.bp.blogspot.com/-_muQ38cZ8ko/XpvW3XytiAI/AAAAAAAAOp0/exXkMDL8og0Q7T59aUdAK80G_csHocIigCNcBGAsYHQ/s1600/unet002.png "3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux - Dicas Linux e Windows")](https://1.bp.blogspot.com/-_muQ38cZ8ko/XpvW3XytiAI/AAAAAAAAOp0/exXkMDL8og0Q7T59aUdAK80G_csHocIigCNcBGAsYHQ/s1600/unet002.png)

[![3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux - Dicas Linux e Windows](https://4.bp.blogspot.com/-16PfeUrPqdI/XpvW3eloLtI/AAAAAAAAOp4/uFcj_djvQx0cAYwFSudF1JTQYEIzZ66FwCNcBGAsYHQ/s1600/unet003.png "3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux - Dicas Linux e Windows")](https://4.bp.blogspot.com/-16PfeUrPqdI/XpvW3eloLtI/AAAAAAAAOp4/uFcj_djvQx0cAYwFSudF1JTQYEIzZ66FwCNcBGAsYHQ/s1600/unet003.png)

[![3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux - Dicas Linux e Windows](https://3.bp.blogspot.com/--u8aJHGVVl0/XpvW4Fw3NeI/AAAAAAAAOp8/vg-XoH7XW8otThp6pW9dBjIkHmpz7By5QCNcBGAsYHQ/s1600/unet004.png "3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux - Dicas Linux e Windows")](https://3.bp.blogspot.com/--u8aJHGVVl0/XpvW4Fw3NeI/AAAAAAAAOp8/vg-XoH7XW8otThp6pW9dBjIkHmpz7By5QCNcBGAsYHQ/s1600/unet004.png)

  
Após alguns minutos, o processo está finalizado.  
  
[](https://draft.blogger.com/null)  

### Etcher

  
O Etcher _(ou Balena Etcher)_ é outra opção para gerar Live USB, talvez a mais fácil das 3 apresentadas aqui. É bem simples de ser utilizado, até mais simples que o UNetbootin, porém, não possui opção de persistência.  
Para baixar, acesse [https://www.balena.io/etcher/](https://www.balena.io/etcher/). A opção padrão de download é a x64, para sistemas 64 bits, mas caso precise da versão 32 bits basta escolher esta versão. Descompacte o aquivo baixado com o comando: _(Troque o que está em vermelho pelo nome do arquivo baixado)_  
  

 unzip balena-etcher-electron-1.5.81-linux-x64.zip

  
O arquivo descompactado é no formato _AppImage_, e não necessita instalação. Porém, antes de executar o programa é preciso dar permissão de execução. Supondo que foi baixado na pasta _Downloads_ execute o comando abaixo.  
  

 sudo chmod +x Downloads/balenaEtcher-1.5.81-x64.AppImage

  
O comando abaixo executa o Etcher. _(Não feche o terminal, pois o Etcher será fechado também)._  
  

 sudo ./Downloads/balenaEtcher-1.5.81-x64.AppImage

  
A tela do Etcher é apresentada abaixo. Para iniciar o processo:  

*   Em _Select image_ selecione a imagem ISO que deseja gravar;
*   Em _Change_ escolha o drive onde está o Pendrive;
*   A opção _Flash_ inicia o processo de gravação.

  

[![3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux - Dicas Linux e Windows](https://1.bp.blogspot.com/-4Xjj4ajUl4Q/XpZ1jh6FfOI/AAAAAAAAOm0/lOzC5YoP0Dov0SyGbfa4yUtayPNZbxRXgCNcBGAsYHQ/s640/Etcher1.png "3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux - Dicas Linux e Windows")](https://1.bp.blogspot.com/-4Xjj4ajUl4Q/XpZ1jh6FfOI/AAAAAAAAOm0/lOzC5YoP0Dov0SyGbfa4yUtayPNZbxRXgCNcBGAsYHQ/s1600/Etcher1.png)

  
Processo em andamento. Aguarde alguns minutos até concluir.  
  

[![3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux - Dicas Linux e Windows](https://3.bp.blogspot.com/-fmPIjcFJDsU/Xpvrrb9GCEI/AAAAAAAAOqY/f_IbV6IDXpgRfKhs0hh3ALe5oHd0WSh5gCNcBGAsYHQ/s640/etcher02.png "3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux - Dicas Linux e Windows")](https://3.bp.blogspot.com/-fmPIjcFJDsU/Xpvrrb9GCEI/AAAAAAAAOqY/f_IbV6IDXpgRfKhs0hh3ALe5oHd0WSh5gCNcBGAsYHQ/s1600/etcher02.png)

  
Processo concluído, Live USB criada e o pendrive já foi desmontado.  
  

[![3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux - Dicas Linux e Windows](https://2.bp.blogspot.com/-QcH5yCvidBQ/XpvrrSCopoI/AAAAAAAAOqU/yVEA3eth_oUeRXJLkDo3U7gesQBACrRlQCNcBGAsYHQ/s640/etcher03.png "3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux - Dicas Linux e Windows")](https://2.bp.blogspot.com/-QcH5yCvidBQ/XpvrrSCopoI/AAAAAAAAOqU/yVEA3eth_oUeRXJLkDo3U7gesQBACrRlQCNcBGAsYHQ/s1600/etcher03.png)