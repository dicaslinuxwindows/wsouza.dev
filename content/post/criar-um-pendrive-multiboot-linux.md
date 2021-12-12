---
title: 'Criando um Pendrive Multiboot com o Yumi'
date: 2015-01-03T03:15:00.000-02:00
draft: false
url: /2015/01/criar-um-pendrive-multiboot-linux.html
tags: 
- Linux
- Pendrive Multiboot
- Tutoriais
- Windows
- Yumi
---

Hoje trago um pequeno tutorial de como criar um pendrive bootável com várias distribuições Linux. Num pendrive multiboot é possível instalar distribuições Linux, discos de recuperação, discos de antivírus, e mesmo versões do Windows. Graças à esta versatilidade de sistemas torna-se interessante e importante possuir um pendrive deste pois pode ser utilizado para testes e recuperação de sistemas instalados no HD. Confira a seguir:

  
  

Para criar este pendrive utilizaremos o Yumi, [disponível aqui](http://www.pendrivelinux.com/yumi-multiboot-usb-creator/), **apenas para Windows**. Se precisa criar uma Live USB e está utilizado um sistema Linux, veja como fazer em [3 maneiras de gravar uma imagem ISO num Pendrive utilizando Linux](https://info.wsouza.com.br/2020/04/3-maneiras-de-gravar-uma-imagem-iso-num-pendrive-utilizando-linux.html).  

  
  

Para utilizar o Yumi não é necessário instalar nada, apenas clique no executável e vamos iniciar.  
Será apresentada a tela abaixo onde escolhemos qual unidade usb utilizaremos, se desejar pode marcar a opção de formatar o pendrive (certifique-se que não haja nenhum arquivo importante neste pendrive antes de formatar). O passo 2 é onde se escolhe a distro que se deseja instalar. Podemos obter a iso marcando a opção "Download Link" que fará o diretamente download e a instalação no pendrive. A outra opção é buscar uma iso que já foi previamente baixada e está numa pasta, para isto utilizamos a opção "Browse".

  

[![multiboot com Yumi](https://1.bp.blogspot.com/-nfFJAn6OygA/VKiz_G6P5-I/AAAAAAAABF8/ZZ2obEIRvrY/s1600/yumi3.png "multiboot com Yumi")](http://1.bp.blogspot.com/-nfFJAn6OygA/VKiz_G6P5-I/AAAAAAAABF8/ZZ2obEIRvrY/s1600/yumi3.png)

  
Vamos escolher uma ISO que está em uma pasta, neste caso o Ubuntu 14.04 64 Bits. Na opção 3 podemos escolher o tamanho para um arquivo persistente, onde ficarão salvas toda as modificações realizadas na ISO quando iniciada pelo pendrive. Normalmente, quando reiniciamos, todas as alterações são perdidas mas, fazendo desta maneira, não ocorre perda _(das distros que testei funcionou com Ubuntu, Xubuntu, e Linux Mint, Debian não deu certo)_. Vamos à instalação da primeira distro no pendrive, clique em "Create" e aguarde.

  

[![multiboot com Yumi](https://2.bp.blogspot.com/--Bv-0lyBwvE/VKiz_7FaOTI/AAAAAAAABGI/GHBijzI6gxE/s1600/yumi5.png "multiboot com Yumi")](http://2.bp.blogspot.com/--Bv-0lyBwvE/VKiz_7FaOTI/AAAAAAAABGI/GHBijzI6gxE/s1600/yumi5.png)

  

Quando chegamos nas  duas telas abaixo pode parecer que  está travado, mas é só aguardar que termina. A primeira tela é da instalação do sistema, e a segunda é da criação do arquivo persistente.

  

[![multiboot com Yumi](https://1.bp.blogspot.com/-_3K5NCl41oQ/VKi0AADnzBI/AAAAAAAABGg/Osa7SJqEMZg/s1600/yumi7.png "multiboot com Yumi")](http://1.bp.blogspot.com/-_3K5NCl41oQ/VKi0AADnzBI/AAAAAAAABGg/Osa7SJqEMZg/s1600/yumi7.png)

  

[![multiboot com Yumi](https://1.bp.blogspot.com/-E90ygn2ebNk/VKi0AH-LbuI/AAAAAAAABGU/A2s1g0ghbeU/s1600/yumi8.png "multiboot com Yumi")](http://1.bp.blogspot.com/-E90ygn2ebNk/VKi0AH-LbuI/AAAAAAAABGU/A2s1g0ghbeU/s1600/yumi8.png)

  

Ao acabar, clicando em "Next" aparece uma janela perguntando se deseja adicionar mais uma distro ao pendrive. Caso queira adicionar  escolha "Sim". Caso não queira instalar, escolha "Não" e estará encerrado. Mas a qualquer momento você poderá adicionar outra distro sem precisar refazer tudo do começo.

  

[![multiboot com Yumi](https://1.bp.blogspot.com/-h7O-Suk000I/VKiz-LQR7FI/AAAAAAAABFk/Ktivy2PYGtI/s1600/yumi10.png "multiboot com Yumi")](http://1.bp.blogspot.com/-h7O-Suk000I/VKiz-LQR7FI/AAAAAAAABFk/Ktivy2PYGtI/s1600/yumi10.png)

  

Se sua escolha foi sim, faça novamente como fez no começo, só não formate o pendrive.

  

[![multiboot com Yumi](https://1.bp.blogspot.com/-XyqrCh89mRY/VKiz-Xf3b3I/AAAAAAAABFg/-XOZSWAd6ak/s1600/yumi11.png "multiboot com Yumi")](http://1.bp.blogspot.com/-XyqrCh89mRY/VKiz-Xf3b3I/AAAAAAAABFg/-XOZSWAd6ak/s1600/yumi11.png)

  

O limite para adicionar distros é o tamanho do pendrive. Para teste utilizei um pendrive pequeno de 8 Gb e instalei o Linux Mint 13, o Xubuntu 14.04 e o Linux Mint 17 cada um com arquivo persistente de 516 Mb e ainda sobrou espaço para pelo menos mais uma distro. Após a instalação podemos encerrar o Yumi.

  

[![multiboot com Yumi](https://4.bp.blogspot.com/-gcAp7ycnEZA/VKiz-4FjaYI/AAAAAAAABFw/ZGWaDK9hFH0/s1600/yumi12.png "multiboot com Yumi")](http://4.bp.blogspot.com/-gcAp7ycnEZA/VKiz-4FjaYI/AAAAAAAABFw/ZGWaDK9hFH0/s1600/yumi12.png)

  

Também é possível remover qualquer distro instalada sem comprometer o funcionamento das outras. Para isto basta escolher o "Uninstaller Mode", depois escolher a distro a ser removida e clicar em "Remove".

  

[![multiboot com Yumi](https://3.bp.blogspot.com/-lkfkIF-17Sk/VKiz_onVVdI/AAAAAAAABGE/xFtHcohGS1Q/s1600/yumi40.png "multiboot com Yumi")](http://3.bp.blogspot.com/-lkfkIF-17Sk/VKiz_onVVdI/AAAAAAAABGE/xFtHcohGS1Q/s1600/yumi40.png)

  

Em um outro teste instalei junto com o Mint e o Xubuntu o Boot Repair, uma distro de recuperação do gerenciador de inicialização Grub. Também, graças à criação do arquivo persistente, foi possível a realização de testes de instalação de hardware (driver de placa de vídeo) sem precisar instalar o sistema no Hd, podendo reiniciar pelo pendrive sem perder as configurações realizadas para o driver.  
  
Conclusão: Criar um pendrive multiboot é uma tarefa relativamente fácil e que pode ajudar usuários experientes, novos e usuários curiosos dispostos a conhecer as diversas distribuições Linux existentes. Mas aí pode surgir uma pergunta: "Não seria mais interessante realizar testes numa máquina virtual?" A resposta é não pois, enquanto numa máquina virtual você emula um hardware e instala o sistema num hardware diferente do seu, fazendo da maneira indicada aqui você está testando seu próprio hardware e poderá ter mais certeza sobre qual distro ou interface utilizar num futura instalação no HD.