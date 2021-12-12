---
title: 'GParted, Particionador Gráfico'
date: 2018-07-19T20:28:00.001-03:00
draft: false
url: /2018/07/gparted-particionador-grafico.html
tags: 
- Linux
- Tutoriais
- Particionar Disco
- GParted
- Ferramentas Linux
---

Dando continuidade à série de postagens sobre algumas ferramentas Linux vou falar do Gparted.  
O GParted é um particionador gráfico. Com ele é possível redimensionar, excluir, criar e formatar partições mas, primeiramente devemos saber: O que é, o porquê e como particionar um disco?  
Confira a resposta a seguir e conheça algumas funções deste poderoso utilitário.

  
  

#### 1 - Introdução

Particionar um disco significa dividir o mesmo em partes que podem ser gerenciadas separadamente. Num disco de 500 GB, por exemplo, não há a necessidade de utilizá-lo totalmente como um único setor. Ao particionar o disco, cada parte funciona como um setor independente, como se fossem vários discos, trazendo várias vantagens como a possibilidade de instalar mais de um sistema operacional ao mesmo tempo, manter os arquivos pessoais separados dos arquivos do sistema, separar os arquivos de boot...  
A seguir vou mostrar como particionar um disco utilizando o gerenciador de partições GParted, rodando no Debian 9.4.

  

#### 2 - Instalação e execução

Para abrir o Gparted procure no menu por Editor de partições Gparted _(como mostra a imagem abaixo)_, ou no terminal, execute o comando:  
  

sudo gparted

  

[![Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows](https://1.bp.blogspot.com/-xYynfo_WItM/W1DyBiASAaI/AAAAAAAAImc/Fe5XCPNweSg14j0bRsaYmWz7RH3LT7QUgCLcBGAs/s640/01.png "Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows")](https://1.bp.blogspot.com/-xYynfo_WItM/W1DyBiASAaI/AAAAAAAAImc/Fe5XCPNweSg14j0bRsaYmWz7RH3LT7QUgCLcBGAs/s1600/01.png)

  

Caso não esteja instalado, execute o comando a seguir para instalação:  
  

sudo apt-get install gparted

  

A imagem abaixo mostra a opção dispositivos onde vemos 3 discos: /dev/sda (20GB), /dev/sdb (2GB) e /dev/sdc (10GB). Cada letra significa um dispositivo físico, isto significa que temos 3 discos reais.  
Para mostrar o funcionamento iremos utilizar o /dev/sdc _(selecionado)_, que está vazio, pois no /dev/sda estão os arquivos do sistema e /dev/sdb está a swap.

  

[![Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows](https://4.bp.blogspot.com/-mYSJY9A5DlI/W1D8YrEbxsI/AAAAAAAAImo/852g8FAINdYFfMkhWmSZEQk6822P0JdyACLcBGAs/s640/02.png "Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows")](https://4.bp.blogspot.com/-mYSJY9A5DlI/W1D8YrEbxsI/AAAAAAAAImo/852g8FAINdYFfMkhWmSZEQk6822P0JdyACLcBGAs/s1600/02.png)

  

#### 3 - Criando uma partição num disco vazio

O disco /dev/sdc está sem nenhuma partição criada portanto vamos criar uma. Para isto basta clicar com o botão direito do mouse em cima da partição não alocada e clicar em novo, como mostra a imagem abaixo.

  

[![Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows](https://4.bp.blogspot.com/-ZR3sgIhR3j0/W1EOjTBOr6I/AAAAAAAAIm0/lnxglEM0jY4ZoHabC-Pb3RJPTmbqM-TXgCLcBGAs/s640/03.png "Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows")](https://4.bp.blogspot.com/-ZR3sgIhR3j0/W1EOjTBOr6I/AAAAAAAAIm0/lnxglEM0jY4ZoHabC-Pb3RJPTmbqM-TXgCLcBGAs/s1600/03.png)

  

Caso não haja nenhuma tabela de partições, será solicitada a criação de uma, como na imagem abaixo.

  

[![Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows](https://2.bp.blogspot.com/-XOD72eZol7Y/W1EQkpxOBOI/AAAAAAAAInA/5vPH4LUf0msP87JKh5snWD_alM3xBmoIgCLcBGAs/s640/14.png "Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows")](https://2.bp.blogspot.com/-XOD72eZol7Y/W1EQkpxOBOI/AAAAAAAAInA/5vPH4LUf0msP87JKh5snWD_alM3xBmoIgCLcBGAs/s1600/14.png)

  

Vá no menu Dispositivo>>Criar tabela de partição, deixe como a imagem abaixo e aplique.

  

[![Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows](https://2.bp.blogspot.com/-rNHVmLeHvXw/W1EQ0gfXS9I/AAAAAAAAInI/XXgETUVWfdoqkP7BRxxDxG7xJHZ_RxdwgCLcBGAs/s640/15.png "Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows")](https://2.bp.blogspot.com/-rNHVmLeHvXw/W1EQ0gfXS9I/AAAAAAAAInI/XXgETUVWfdoqkP7BRxxDxG7xJHZ_RxdwgCLcBGAs/s1600/15.png)

  

Após a criação da tabela de partições, ou caso já haja uma, a janela abaixo se abrirá. Neste caso criaremos apenas uma partição, utilizando todos os 10GB do disco. Escolheremos o sistema de arquivos padrão do Debian, que é o ext4 . Para prosseguir clique em Adicionar.

  

[![Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows](https://4.bp.blogspot.com/-d_i0nI__2zQ/W05qP7zu-9I/AAAAAAAAIlc/EiBDm41k_SEIdZcrHL0WImOuqtDNuX5kACLcBGAs/s640/04.png "Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows")](https://4.bp.blogspot.com/-d_i0nI__2zQ/W05qP7zu-9I/AAAAAAAAIlc/EiBDm41k_SEIdZcrHL0WImOuqtDNuX5kACLcBGAs/s1600/04.png)

  

Clique no "botão" verde para aplicar a operação de criação da partição, confirme a aplicação da operação e aguarde a conclusão.

  

[![Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows](https://2.bp.blogspot.com/-J3O_rXbEvYk/W1EalRw9VxI/AAAAAAAAIoM/KQ3gGwnBiwQ8ELcX3N-ZWVjUJB8lG91zwCLcBGAs/s640/05.png "Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows")](https://2.bp.blogspot.com/-J3O_rXbEvYk/W1EalRw9VxI/AAAAAAAAIoM/KQ3gGwnBiwQ8ELcX3N-ZWVjUJB8lG91zwCLcBGAs/s1600/05.png)

  

#### 4 - Criando uma segunda partição no mesmo disco

Como vemos abaixo, a partição /dev/sdc1 foi criada com as configurações escolhidas. Veja que o nome do disco é /dev/sdc porém, o nome da partição  é /dev/sdc1. Agora iremos criar uma segunda partição. Para isto basta clicar com o botão direito e escolher a opção Redimensionar/Mover.

  

[![Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows](https://2.bp.blogspot.com/-wbehzK65tW0/W05qQ6_3aqI/AAAAAAAAIls/-JQAfExRFrQ-5WpHpe2OzS2xFkonh3bigCLcBGAs/s640/08.png "Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows")](https://2.bp.blogspot.com/-wbehzK65tW0/W05qQ6_3aqI/AAAAAAAAIls/-JQAfExRFrQ-5WpHpe2OzS2xFkonh3bigCLcBGAs/s1600/08.png)

  

A imagem abaixo mostra o disco dividido em dois. A opção _Espaço livre antes (MB)_ será uma partição e a opção _Novo tamanho (MB)_ será o novo tamanho da partição criada anteriormente, ou seja, ela foi dividida exatamente pela metade.  Basta confirmar a operação no botão _Redimensionar/Mover._

  

[![Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows](https://3.bp.blogspot.com/-BMyCPZ_fhno/W05qReNKEjI/AAAAAAAAIl0/HErQb61fvHgIqxxugZO_4TpgredEXV-0ACLcBGAs/s640/10.png "Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows")](https://3.bp.blogspot.com/-BMyCPZ_fhno/W05qReNKEjI/AAAAAAAAIl0/HErQb61fvHgIqxxugZO_4TpgredEXV-0ACLcBGAs/s1600/10.png)

  

Ficará assim: A partição /dev/sdc1, criada anteriormente ficou com as mesmas configurações mas com tamanho 5 GB. Foi criada uma outra partição, também com 5 GB. Esta nova partição ainda não está alocada, ou seja, não tem sistema de arquivos. Para criar o sistema de arquivos clique com o botão direito em cima dela e clique em _Novo._

  

[![Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows](https://1.bp.blogspot.com/-sRS2UKGwoek/W1ETbSC2YhI/AAAAAAAAInc/vm1MhpNk8FgxMfKE_uE0kudwJ_fe7Ej6ACLcBGAs/s640/17.png "Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows")](https://1.bp.blogspot.com/-sRS2UKGwoek/W1ETbSC2YhI/AAAAAAAAInc/vm1MhpNk8FgxMfKE_uE0kudwJ_fe7Ej6ACLcBGAs/s1600/17.png)

  

Abrirá a janela abaixo, vá em _Sistema de arquivos_, onde será possível escolher qual o sistema de arquivos que a nova partição terá e clique em _Adicionar_. Note que o GParted suporta partições Windows _(ntfs, fat16 e fat 32)._

  

[![Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows](https://4.bp.blogspot.com/-Qfo87PBN4g4/W1EVALVt6LI/AAAAAAAAIno/kQiQLzZhiOkEsqIeEQI7lBeb-tyahvvgACLcBGAs/s640/18.png "Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows")](https://4.bp.blogspot.com/-Qfo87PBN4g4/W1EVALVt6LI/AAAAAAAAIno/kQiQLzZhiOkEsqIeEQI7lBeb-tyahvvgACLcBGAs/s1600/18.png)

  

Após criada, clique no "botão" verde para aplicar a operação de criação da partição e aguarde a conclusão.

  

[![Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows](https://2.bp.blogspot.com/-Nu-rrkcxvs8/W1EVlH66XoI/AAAAAAAAInw/npioxXNQ6u0hM0ZEP-u4HR8ujpn8dO9NwCLcBGAs/s640/19.png "Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows")](https://2.bp.blogspot.com/-Nu-rrkcxvs8/W1EVlH66XoI/AAAAAAAAInw/npioxXNQ6u0hM0ZEP-u4HR8ujpn8dO9NwCLcBGAs/s1600/19.png)

  

Após todos os processos concluídos ficará assim: O disco /dev/sdc com duas partições. A partição /dev/sdc1 com 5 GB e sistema de arquivos ext4 e a partição /dev/sdc2 com 5 GB e sistema de arquivos fat32.

  

[![Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows](https://3.bp.blogspot.com/-D_6nPplIT0w/W1EWiXZPivI/AAAAAAAAIoA/J8v7e4kr59Ipry3eLfDMuQaNmsgUpb_aQCLcBGAs/s640/20.png "Ferramentas Linux 2 - GParted, Particionador Gráfico - Dicas Linux e Windows")](https://3.bp.blogspot.com/-D_6nPplIT0w/W1EWiXZPivI/AAAAAAAAIoA/J8v7e4kr59Ipry3eLfDMuQaNmsgUpb_aQCLcBGAs/s1600/20.png)

  

#### 5 - Considerações finais

Como vimos, o Gparted é uma ferramenta indispensável quando precisamos redimensionar ou particionar discos. Porém, são necessários alguns cuidados para não perder os arquivos pessoais ou os arquivos de boot _(o que impediria o sistema de iniciar). _  
Alguns cuidados necessários:  

*   Ao manipular um disco onde o sistema já esteja instalado, esteja ciente que poderá perder o acesso ao sistema, portanto faça backup de seus dados.
*   Dê preferência em particionar um disco vazio, criando partições para o (s) sistema (s)  e deixando uma partição maior para arquivos pessoais. Fazendo assim, poderá manipular normalmente as outras partições, correndo um risco menor de perder seus arquivos.
*   Teste a utilização numa máquina virtual para se adaptar ao uso do Gparted. 
*   Dê preferência para utilizar o Gparted num Live CD. _(Futuramente será mostrado como fazer isso.)_

  

Para mais detalhes, acesse o [manual do GParted](https://gparted.org/display-doc.php?name=help-manual&lang=pt_BR).