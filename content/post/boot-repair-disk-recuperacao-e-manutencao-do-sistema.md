---
title: 'Boot-Repair-Disk - Recuperação e Manutenção do Sistema'
date: 2018-12-21T23:00:00.000-02:00
draft: false
url: /2018/12/boot-repair-disk-recuperacao-e-manutencao-do-sistema.html
tags: 
- Linux
- Tutoriais
- Recuperar Grub
- Ferramentas Linux
---

Boot-Repair-Disk é um conjunto de ferramentas Linux voltadas para manutenção e recuperação de sistemas operacionais. Dentre estas ferramentas estão o GParted, scripts para instalação, edição e recuperação do GRUB, ferramenta de remoção de sistema operacional, ferramenta de diagnóstico do boot, restauração da MBR entre outras. Mais detalhes a seguir.

  

#### 1 - Introdução

Creio que quase todo mundo, enquanto usuário de sistemas GNU/Linux, já deve ter passado por algum aperto perder o gerenciador de inicialização _(GRUB)_ ao atualizar ou instalar um novo sistema para trabalhar em Dual Boot, ou tentando remover versões antigas do Kernel. Só quem já passou por isso sabe o quão é chato, e, não sabendo a maneira correta de resolver, pode causar uma grande quantidade de trabalho levando até à reinstalação do sistema operacional.  
O Boot-Repair-Disk _(Boot-Repair)_ evita todos estes transtornos, pois fornece ferramentas de recuperação do GRUB.

  

#### 2 - Como obter o Boot-Repair

A melhor forma de utilizar o Boot-Repair é a partir de um Live CD ou Pendrive inicializável, pois se você perdeu o acesso ao GRUB, não terá como acessar o sistema operacional instalado na sua máquina. As imagens para gravar no CD ou Pendrive podem ser obtidas nos links abaixo, de acordo com seu processador.  
  
[32 Bits](https://sourceforge.net/projects/boot-repair-cd/files/boot-repair-disk-32bit.iso/download)  
[64 Bits](https://sourceforge.net/projects/boot-repair-cd/files/boot-repair-disk-64bit.iso/download)  
  
Grave a imagem baixada num CD ou Pendrive _(Para gravar num pendrive, utilize o [Universal USB Installer](https://www.pendrivelinux.com/universal-usb-installer-easy-as-1-2-3/), [UnetBootIn](https://unetbootin.github.io/), [YUMI](https://info.wsouza.com.br/2015/01/criar-um-pendrive-multiboot-linux.html) ou qualquer aplicativo semelhante)_

  

#### 3 - Recuperando o GRUB

Ao iniciar o computador, já com o CD no drive ou pendrive inserido, escolha o idioma e ao terminar o Boot, será mostrada a tela abaixo. Aguarde a finalização.  
  

[![Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows](https://1.bp.blogspot.com/-6Rb9xCaowqw/XBw-VPK5r7I/AAAAAAAAJ40/QPHrSr40jTsyQH9OUwFKhjFH0CDJenC1QCLcBGAs/s1600/01.png "Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows")](https://1.bp.blogspot.com/-6Rb9xCaowqw/XBw-VPK5r7I/AAAAAAAAJ40/QPHrSr40jTsyQH9OUwFKhjFH0CDJenC1QCLcBGAs/s1600/01.png)

  
Após a detecção dos sistemas operacionais instalados, a tela abaixo será mostrada. Em casos de perda do GRUB, utilize as opções padrão _(Reparação recomendada)_ e aguarde a conclusão. Reinicie a máquina e provavelmente o GRUB estará recuperado.  
  

[![Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows](https://1.bp.blogspot.com/-BCGU-FYl5RI/XBw-VAVSFsI/AAAAAAAAJ4s/UdJlF4DjVPsagPQhOXWcXLqu0crTeAAvQCLcBGAs/s1600/02.png "Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows")](https://1.bp.blogspot.com/-BCGU-FYl5RI/XBw-VAVSFsI/AAAAAAAAJ4s/UdJlF4DjVPsagPQhOXWcXLqu0crTeAAvQCLcBGAs/s1600/02.png)

  
Nas opções avançadas é possível, além de recuperar o GRUB, alterar algumas opções a fim de obter um melhor resultado. Mas preste muita atenção no que está fazendo, pois poderá causar vários outros problemas.  
  

[![Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows](https://3.bp.blogspot.com/-sRmkMZg_MP4/XBw-VA6WOcI/AAAAAAAAJ4w/S7US6vTibHAy8pvGr-DNlIOZoG_DqBLwgCLcBGAs/s1600/03.png "Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e WindowsBoot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows")](https://3.bp.blogspot.com/-sRmkMZg_MP4/XBw-VA6WOcI/AAAAAAAAJ4w/S7US6vTibHAy8pvGr-DNlIOZoG_DqBLwgCLcBGAs/s1600/03.png)

  
Caso tenha mais de um sistema instalado, antes de recuperar, você poderá escolher a ordem de inicialização. Na opção _Sistema a iniciar por padrão_ escolha o sistema desejado. Também é possível colocar o GRUB em outra unidade, ou partição.  
  

[![Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows](https://3.bp.blogspot.com/-nR1sLr4GFUY/XBw-VpzrDpI/AAAAAAAAJ44/HJHewpMv1Q0XkWHUUn-vTE9BNlFNKsWSwCLcBGAs/s1600/04.png "Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows")](https://3.bp.blogspot.com/-nR1sLr4GFUY/XBw-VpzrDpI/AAAAAAAAJ44/HJHewpMv1Q0XkWHUUn-vTE9BNlFNKsWSwCLcBGAs/s1600/04.png)

  
No exemplo que estou utilizando tenho 5 sistemas operacionais instalados. Como visto na tela acima deixei o Debian 9 como padrão para iniciar. Na tela abaixo vemos todas as opções disponíveis. Podemos alterar para qualquer opção para ser a padrão de inicialização.  
  

[![Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows](https://1.bp.blogspot.com/-e2Jjo2eTeIo/XBw-VzzSMWI/AAAAAAAAJ5A/AIbFMLmSxN4nDw7qQrsYwo7TL_8mfXmZQCLcBGAs/s1600/05.png "Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows")](https://1.bp.blogspot.com/-e2Jjo2eTeIo/XBw-VzzSMWI/AAAAAAAAJ5A/AIbFMLmSxN4nDw7qQrsYwo7TL_8mfXmZQCLcBGAs/s1600/05.png)

  
Nas telas abaixo temos mais opções avançadas. Aqui podemos, por exemplo, remover o GRUB totalmente antes de reinstalá-lo. Mas ao fazer isto, deve-se ter estar conectado à internet, pois será necessário baixar o pacote novamente. Também é possível salvar os logs, para buscar ajuda em caso de algum erro que impeça a recuperação. Antes de reiniciar o Boot- Repair, copie estes logs para outro lugar _(e-mail, por exemplo)._  
  

[![Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows](https://4.bp.blogspot.com/-vLjGUEd1fsM/XBw-V-Di4LI/AAAAAAAAJ48/uR6zSvYG49QUCZEpt7sVFReOhmq78peYgCLcBGAs/s1600/06.png "Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows")](https://4.bp.blogspot.com/-vLjGUEd1fsM/XBw-V-Di4LI/AAAAAAAAJ48/uR6zSvYG49QUCZEpt7sVFReOhmq78peYgCLcBGAs/s1600/06.png)

  

[![Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows](https://1.bp.blogspot.com/-wVDSXVcuSI4/XBw-WOowu2I/AAAAAAAAJ5E/w9APj50lLZ0Sjhj0q1UjIyY_1172OD0_wCLcBGAs/s1600/07.png "Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows")](https://1.bp.blogspot.com/-wVDSXVcuSI4/XBw-WOowu2I/AAAAAAAAJ5E/w9APj50lLZ0Sjhj0q1UjIyY_1172OD0_wCLcBGAs/s1600/07.png)

  
Terminado  o processo, reinicie o sistema e o GRUB estará recuperado, como podemos ver na tela abaixo.  
  

[![Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows](https://3.bp.blogspot.com/-9U-9glaQ_4g/XBw-WeKOnjI/AAAAAAAAJ5I/iGeNIlxt9wcliqZG-2oANK-L13hzZ1X_wCLcBGAs/s1600/09.png "Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e WindowsBoot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows")](https://3.bp.blogspot.com/-9U-9glaQ_4g/XBw-WeKOnjI/AAAAAAAAJ5I/iGeNIlxt9wcliqZG-2oANK-L13hzZ1X_wCLcBGAs/s1600/09.png)

  

#### 4 - Ferramentas de Manutenção de Sistema

Além de possibilitar a recuperação do GRUB, o Boot-Repair possui outras ferramentas que podem ser úteis para manipular partições [_(Gparted)_](https://info.wsouza.com.br/2018/07/ferramentas-linux-2-gparted-particionador-grafico.html), diagnosticar problemas, recuperar sistemas operacionais ou mesmo para obter informações sobre o computador, como podemos ver na imagem abaixo.  
  

[![Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows](https://4.bp.blogspot.com/-6Ame7eg4WLE/XB2AboPthuI/AAAAAAAAJ6M/TOzUcmg88sQPO4AJwuaI2liFpYLXVnsSgCLcBGAs/s1600/10.png "Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows")](https://4.bp.blogspot.com/-6Ame7eg4WLE/XB2AboPthuI/AAAAAAAAJ6M/TOzUcmg88sQPO4AJwuaI2liFpYLXVnsSgCLcBGAs/s1600/10.png)

  
Ferramenta para verificar as informações do computador. Muito útil obter informações de memória, processador e periféricos.  
  

[![Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows](https://3.bp.blogspot.com/-AafkxJJAbuQ/XB2AbXOmOQI/AAAAAAAAJ6I/b2PpBYok57A3qqpV7bsNYheQqh7_ehb1gCLcBGAs/s1600/11.png "Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows")](https://3.bp.blogspot.com/-AafkxJJAbuQ/XB2AbXOmOQI/AAAAAAAAJ6I/b2PpBYok57A3qqpV7bsNYheQqh7_ehb1gCLcBGAs/s1600/11.png)

  
Ferramenta para desinstalar um sistema operacional.  
  

[![Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows](https://4.bp.blogspot.com/-cDLBO5opM80/XB2AbJpw26I/AAAAAAAAJ6E/_pALhzC5QdINnlR6xhOv6o_P-jjAkYcuQCLcBGAs/s1600/12.png "Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows")](https://4.bp.blogspot.com/-cDLBO5opM80/XB2AbJpw26I/AAAAAAAAJ6E/_pALhzC5QdINnlR6xhOv6o_P-jjAkYcuQCLcBGAs/s1600/12.png)

  
Ferramenta para diagnosticar a inicialização do computador. Cria um arquivo de log com o diagnóstico realizado, possibilitando que as informações estejam disponíveis para procurar ajuda em fóruns e e outros sites na internet.  
  

[![Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e WindowsBoot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows](https://4.bp.blogspot.com/-MEEotfHUjyY/XBw-Xd7DfQI/AAAAAAAAJ5c/5qWsl_nAl9Q033rdEly0xtPwcq_SmbgpACLcBGAs/s1600/13.png "Boot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e WindowsBoot-Repair-Disk - Recuperação e Manutenção do Sistema - Dicas Linux e Windows")](https://4.bp.blogspot.com/-MEEotfHUjyY/XBw-Xd7DfQI/AAAAAAAAJ5c/5qWsl_nAl9Q033rdEly0xtPwcq_SmbgpACLcBGAs/s1600/13.png)

  

#### 5 - Considerações finais

É indispensável ter em mãos este conjunto de ferramentas pois, a qualquer momento, podemos ser surpreendidos com algum problema.