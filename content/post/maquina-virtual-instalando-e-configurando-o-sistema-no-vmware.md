---
title: 'Máquina Virtual: Instalando e configurando o sistema no VMware'
date: 2018-08-14T16:22:00.000-03:00
draft: false
url: /2018/08/maquina-virtual-instalando-e-configurando-o-sistema-no-vmware.html
tags: 
- Linux
- Máquina Virtual
- Tutoriais
- VMware Player
- Ferramentas Linux
---

Neste post vou mostrar como instalar e configurar o sistema operacional na máquina virtual (VM). Este post é uma continuação direta do [Máquina Virtual: Instalando e configurando o VMware Player](https://info.wsouza.com.br/2018/07/maquina-virtual-instalando-e-configurando-o-wmware-player.html).  
Confira a seguir.  
  

#### 1 - Introdução

A configuração da VM já foi mostrada na matéria anterior. A partir daqui será mostrado o processo de boot para instalação do sistema, instalação e configuração do mesmo na VM. O sistema operacional escolhido foi o Lubuntu 18.04 _([baixe-o aqui](http://cdimage.ubuntu.com/lubuntu/releases/18.04/release/lubuntu-18.04-desktop-i386.iso))_, versão do Ubuntu com a interface LXDE. Mas a escolha do sistema fica a critério de cada um, e os processos para instalar e configurar são iguais. _Dica: Você poderá utilizar a mesma ISO gerada no tópico [Backup com Remaster GTK](https://info.wsouza.com.br/2018/07/backup-com-remaster-gtk.html)_

  

#### 2 - Instalação

Para instalação do sistema você pode escolher uma das duas maneiras:  
  
1 - Instalar a partir de uma mídia de DVD no drive físico do hospedeiro;  
2 - Instalar a partir de uma imagem ISO previamente salva numa pasta do computador.  
  

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://1.bp.blogspot.com/-_AROF1AmGtM/W3MAnF7TQwI/AAAAAAAAI7w/Vpe3JGpo5iwOwM0hdivsFKQJ10utBqVjACLcBGAs/s640/02.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://1.bp.blogspot.com/-_AROF1AmGtM/W3MAnF7TQwI/AAAAAAAAI7w/Vpe3JGpo5iwOwM0hdivsFKQJ10utBqVjACLcBGAs/s1600/02.png)

  
Escolhida uma das duas opções, inicie a VM e será iniciada a instalação do sistema operacional.

  

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://4.bp.blogspot.com/-yHfvcp46kkM/W1fr3vVRSAI/AAAAAAAAIwE/YucBam6YUFoO_6xjOdtAVgDwGV_iPuL0ACLcBGAs/s320/18.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://4.bp.blogspot.com/-yHfvcp46kkM/W1fr3vVRSAI/AAAAAAAAIwE/YucBam6YUFoO_6xjOdtAVgDwGV_iPuL0ACLcBGAs/s1600/18.png)

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://3.bp.blogspot.com/-DG6T58JeSAE/W1gH6SQCecI/AAAAAAAAIww/jnBhY2bCtKYNpNnci3wA3doYay7WOB-QACLcBGAs/s320/01.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://3.bp.blogspot.com/-DG6T58JeSAE/W1gH6SQCecI/AAAAAAAAIww/jnBhY2bCtKYNpNnci3wA3doYay7WOB-QACLcBGAs/s1600/01.png)

  
A instalação do sistema numa VM ocorre da mesma maneira que numa máquina real, sendo assim, não entrarei em detalhes sobre a instalação. Após o boot escolha o idioma de preferência e instalar o Lubuntu.  
  

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://2.bp.blogspot.com/-jVg6WOK_XtE/W1gH6pKNwOI/AAAAAAAAIw0/IN7HknrQQGkDL6PPjsXcdfC2z31r7hN_ACLcBGAs/s200/02.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://2.bp.blogspot.com/-jVg6WOK_XtE/W1gH6pKNwOI/AAAAAAAAIw0/IN7HknrQQGkDL6PPjsXcdfC2z31r7hN_ACLcBGAs/s1600/02.png)

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://3.bp.blogspot.com/-yINED7pwca4/W1gH6riKcnI/AAAAAAAAIw4/pUQu2Al6T1M416bvVAaPlsZwYs1DIp5OgCLcBGAs/s200/03.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://3.bp.blogspot.com/-yINED7pwca4/W1gH6riKcnI/AAAAAAAAIw4/pUQu2Al6T1M416bvVAaPlsZwYs1DIp5OgCLcBGAs/s1600/03.png)

  
As telas abaixo mostram o início e o final da instalação. Reinicie o sistema para concluir a instalação.  
  

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://2.bp.blogspot.com/-4tVstPbTpvc/W1gH65IqFVI/AAAAAAAAIw8/0fGeoNBSMGgVS0AFbwaaTCl9-_I661gOQCLcBGAs/s320/04.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://2.bp.blogspot.com/-4tVstPbTpvc/W1gH65IqFVI/AAAAAAAAIw8/0fGeoNBSMGgVS0AFbwaaTCl9-_I661gOQCLcBGAs/s1600/04.png)

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://4.bp.blogspot.com/-AuiqIVVEgXo/W1gH7ePeXWI/AAAAAAAAIxA/Ep84NkAfwjQrrC-acihr56ysqA3fPk8CACLcBGAs/s320/05.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://4.bp.blogspot.com/-AuiqIVVEgXo/W1gH7ePeXWI/AAAAAAAAIxA/Ep84NkAfwjQrrC-acihr56ysqA3fPk8CACLcBGAs/s1600/05.png)

  
O sistema está instalado. basta inserir o login e senha criados no momento da instalação e você terá acesso ao sistema instalado em sua VM.  
  

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://3.bp.blogspot.com/-zj84D7NHk8w/W1gH7RNsqdI/AAAAAAAAIxE/ILD9nWcGH38mXU_dR_9IkP_d26uisoa-QCLcBGAs/s320/06.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://3.bp.blogspot.com/-zj84D7NHk8w/W1gH7RNsqdI/AAAAAAAAIxE/ILD9nWcGH38mXU_dR_9IkP_d26uisoa-QCLcBGAs/s1600/06.png)

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://2.bp.blogspot.com/-fnTIoJnY9vE/W1gH7vxUboI/AAAAAAAAIxI/KfveL9gaARM8mpgzjpCWWpfI2TEy3uP7gCLcBGAs/s320/07.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://2.bp.blogspot.com/-fnTIoJnY9vE/W1gH7vxUboI/AAAAAAAAIxI/KfveL9gaARM8mpgzjpCWWpfI2TEy3uP7gCLcBGAs/s1600/07.png)

#### 3 - Configuração

Para que o sistema tenha o máximo de funcionalidade na VM, como rodar em tela cheia com resolução igual a do hospedeiro, é preciso instalar uma ferramenta chamada VMware Tools, que pode ser acessada conforme mostra a imagem abaixo.  
  

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://4.bp.blogspot.com/-zlWd2-L_a2w/W1uW2TrmdhI/AAAAAAAAI10/jaqNKskKYwESuTjJbLyc2sR0_rcIeIZ8gCLcBGAs/s640/09.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://4.bp.blogspot.com/-zlWd2-L_a2w/W1uW2TrmdhI/AAAAAAAAI10/jaqNKskKYwESuTjJbLyc2sR0_rcIeIZ8gCLcBGAs/s1600/09.png)

  
Faça o download e aguarde...  
  

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://1.bp.blogspot.com/-32jYbbrAIcs/W1gH9PCglBI/AAAAAAAAIxU/VcfIWiqSxHoJDRktRQDXGvCDfKy3rGfuwCLcBGAs/s400/10.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://1.bp.blogspot.com/-32jYbbrAIcs/W1gH9PCglBI/AAAAAAAAIxU/VcfIWiqSxHoJDRktRQDXGvCDfKy3rGfuwCLcBGAs/s1600/10.png)

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://2.bp.blogspot.com/-vO9d4nnRQVo/W1gH9vbaCdI/AAAAAAAAIyQ/4tCCL8Dp4-ougg-LGZBvi1c2URjm1uQfgCPcBGAYYCw/s1600/12.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://2.bp.blogspot.com/-vO9d4nnRQVo/W1gH9vbaCdI/AAAAAAAAIyQ/4tCCL8Dp4-ougg-LGZBvi1c2URjm1uQfgCPcBGAYYCw/s1600/12.png)

  
Será montada uma unidade de rede com o nome VMwareTools. Abra esta unidade, copie a pasta  VMwareTools-10.1.6.5214329.tar.gz para sua home, descompacte e renomeie para vmware-tools-distrib, caso não tenha este nome.  
  

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://4.bp.blogspot.com/-OB9jRmzIcOU/W3MZGhEjeUI/AAAAAAAAI78/_-zBFwiysP8FbwhlCGRGFEaVp1IFRFQ1QCLcBGAs/s640/13.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://4.bp.blogspot.com/-OB9jRmzIcOU/W3MZGhEjeUI/AAAAAAAAI78/_-zBFwiysP8FbwhlCGRGFEaVp1IFRFQ1QCLcBGAs/s1600/13.png)

  

A partir de agora vamos utilizar o terminal. Faça o login como root.  
  

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://2.bp.blogspot.com/-rF3jHc_iDCI/W1uXPT86YlI/AAAAAAAAI2I/c5PvvsZNj448c8yZxwzI5OVUrzEfK_eOQCLcBGAs/s640/14.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://2.bp.blogspot.com/-rF3jHc_iDCI/W1uXPT86YlI/AAAAAAAAI2I/c5PvvsZNj448c8yZxwzI5OVUrzEfK_eOQCLcBGAs/s1600/14.png)

  
Antes de iniciar a instalação, instale o gnome-nettool. Com ele serão instaladas algumas ferramentas de rede que serão necessárias para os próximos passos.  
  

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://1.bp.blogspot.com/-vgxERC422ik/W1uXPWspBSI/AAAAAAAAI18/SU2ZFvpvj9sq9uEl7qEtF39fO_nBQnMawCLcBGAs/s640/15.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://1.bp.blogspot.com/-vgxERC422ik/W1uXPWspBSI/AAAAAAAAI18/SU2ZFvpvj9sq9uEl7qEtF39fO_nBQnMawCLcBGAs/s1600/15.png)

  
Acesse a vmware-tools-distrib, recém criada.  
  

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://4.bp.blogspot.com/-14m3xp5H5gQ/W1uXPZFYuoI/AAAAAAAAI2A/LCBiN1aJF1QBO_8JYN26UAyP8iYazLLQgCLcBGAs/s640/16.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://4.bp.blogspot.com/-14m3xp5H5gQ/W1uXPZFYuoI/AAAAAAAAI2A/LCBiN1aJF1QBO_8JYN26UAyP8iYazLLQgCLcBGAs/s1600/16.png)

  
Dê permissão de execução ao arquivo vmware-install.pl com o comando chmod +x vmware-install.pl e execute o mesmo com o comando ./vmware-install.pl  
A partir deste momento surgirão várias linhas de confirmação. Sempre digite yes até o final.  
  

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://4.bp.blogspot.com/-2Vx7oiv1sJE/W1uXPwwfRZI/AAAAAAAAI2E/tXBrSUv9mN0t_nzKmeJbX9lX8zd-CeWZACLcBGAs/s640/17.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://4.bp.blogspot.com/-2Vx7oiv1sJE/W1uXPwwfRZI/AAAAAAAAI2E/tXBrSUv9mN0t_nzKmeJbX9lX8zd-CeWZACLcBGAs/s1600/17.png)

  
Finalizada a instalação reinicie a VM e o sistema virtual estará funcionando perfeitamente.  
  

[![Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows](https://4.bp.blogspot.com/-VNsczlLxP6U/W1gH-7uX_gI/AAAAAAAAIx0/Fwg4Zc_aYKM8UnL-J_5Q6_6muh3A8xPSgCLcBGAs/s640/18.png "Ferramentas Linux 4 - Máquina Virtual: Instalando e configurando o sistema  no ambiente virtualizado - Dicas Linux e Windows")](https://4.bp.blogspot.com/-VNsczlLxP6U/W1gH-7uX_gI/AAAAAAAAIx0/Fwg4Zc_aYKM8UnL-J_5Q6_6muh3A8xPSgCLcBGAs/s1600/18.png)

  

#### 4 - Conclusão

Utilizar um sistema operacional instalado numa VM torna-se muito interessante quando precisamos utilizar mais de um sistema por vez (Ex: Windows e Linux, ou quando precisamos realizar testes que possam comprometer a integridade de nosso sistema operacional principal.