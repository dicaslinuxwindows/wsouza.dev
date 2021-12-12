---
title: 'Backup com Remaster GTK'
date: 2018-07-16T22:00:00.001-03:00
draft: false
url: /2018/07/backup-com-remaster-gtk.html
tags: 
- Linux
- Tutoriais
- Backup do Sistema
- Remaster
- Ferramentas Linux
---

  

Iniciarei uma série de postagens sobre algumas ferramentas Linux.  
E neste primeiro post vou falar do Remaster GTK, um ótimo utilitário que, entre outras funções, permite o backup do sistema operacional instalado em seu dispositivo. Veremos a seguir como utilizá-lo.

  

#### 1 - O que é o Remaster-GTK?

  

O Remaster é um fork do descontinuado [Remastersys-GTK](https://info.wsouza.com.br/2013/01/remastersys-um-otimo-utilitario-de.html), desenvolvido e mantido pelo Lobo do site [Linux Dicas e Suporte](https://linuxdicasesuporte.blogspot.com/). Com ele é possível realizar um backup completo do seu sistema operacional, mantendo seus dados, programas e configurações pessoais. Será gerado uma ISO Live e poderá ser gravada num DVD ou pendrive podendo ser executado diretamente ou mesmo instalado num outro dispositivo.  
No Remaster há versões para Debian e Ubuntu e a dica a seguir será mostrada com a versão para Debian, executada e testada no Debian 9.

  

#### 2 - Instalação

  

Baixe o Remaster Debian, e siga os passos para a instalação em: [https://linuxdicasesuporte.blogspot.com/p/remaster\_31.html](https://linuxdicasesuporte.blogspot.com/p/remaster_31.html)

  

#### 3 - Configuração e utilização

  

Após instalado, você pode encontrá-lo no menu ou, se preferir, no terminal execute o comando:

  

sudo remaster-gtk

  

A imagem abaixo mostra a tela inicial do Remaster.

  

[![Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows](https://1.bp.blogspot.com/-U0Jq_wVBMxM/W00q3EpK56I/AAAAAAAAIkU/98DsJ7cm6B4BJKxl7qyF-YJ_Y4OBzPZ-ACLcBGAs/s640/Captura%2Bde%2Btela%2Bde%2B2018-07-15%2B23-43-44.png "Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows")](https://1.bp.blogspot.com/-U0Jq_wVBMxM/W00q3EpK56I/AAAAAAAAIkU/98DsJ7cm6B4BJKxl7qyF-YJ_Y4OBzPZ-ACLcBGAs/s1600/Captura%2Bde%2Btela%2Bde%2B2018-07-15%2B23-43-44.png)

  

Abaixo é possível configurar os dados de seu sistema. Em _"nome de usuário"_ eu normalmente coloco o mesmo nome de usuário que estou desejo que seja o usuário padrão do backup. O nome da ISO e da remasterização fica a critério do usuário. Normalmente não altero outras opções, com exceção da _Selecionar configurações do usuário_, onde escolho as configurações do usuário de preferência. Detalhe: Deve-se escolher um usuário que tenha uma _home_ pequena, pois a ISO poderá ser muito grande e não caber num DVD.

  

[![Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows](https://1.bp.blogspot.com/-5QpyGXZFakk/W00q3LpSA5I/AAAAAAAAIkQ/93kt4mEsTQo8yxIaylmKIScMOB0v8eV5wCLcBGAs/s640/Captura%2Bde%2Btela%2Bde%2B2018-07-15%2B23-44-04.png "Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows")](https://1.bp.blogspot.com/-5QpyGXZFakk/W00q3LpSA5I/AAAAAAAAIkQ/93kt4mEsTQo8yxIaylmKIScMOB0v8eV5wCLcBGAs/s1600/Captura%2Bde%2Btela%2Bde%2B2018-07-15%2B23-44-04.png)

  

O foco da dica é o backup do sistema instalado em seu dispositivo, portanto a opção a ser escolhida é Backup, como na tela abaixo  
Vela ressaltar que normalmente testo na interface Gnome e sempre obtive os resultados esperados. Mas de acordo com as informações do desenvolvedor também funciona no Mate e KDE e XFCE4, com os gerenciadores de sessão GDM3, KDM e LightDM

  

[![Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows](https://2.bp.blogspot.com/-BZGM_L9z-QU/W00q3CXEy0I/AAAAAAAAIkY/B0WufJMwtcQraIdV0UlJqJrSTsmQI3pxwCLcBGAs/s640/Captura%2Bde%2Btela%2Bde%2B2018-07-15%2B23-44-22.png "Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows")](https://2.bp.blogspot.com/-BZGM_L9z-QU/W00q3CXEy0I/AAAAAAAAIkY/B0WufJMwtcQraIdV0UlJqJrSTsmQI3pxwCLcBGAs/s1600/Captura%2Bde%2Btela%2Bde%2B2018-07-15%2B23-44-22.png)

  

Como vemos nas duas telas abaixo, o backup iniciará. Esta opção demora bastante tempo.

  

[![Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows](https://1.bp.blogspot.com/-3tvnQi3yqBQ/W00q3lCFJSI/AAAAAAAAIkc/qhQg2Rvc6LIBpvWhvenL3MzDMMiyyJr7ACLcBGAs/s640/Captura%2Bde%2Btela%2Bde%2B2018-07-15%2B23-44-30.png "Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows")](https://1.bp.blogspot.com/-3tvnQi3yqBQ/W00q3lCFJSI/AAAAAAAAIkc/qhQg2Rvc6LIBpvWhvenL3MzDMMiyyJr7ACLcBGAs/s1600/Captura%2Bde%2Btela%2Bde%2B2018-07-15%2B23-44-30.png)

  

[![Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows](https://3.bp.blogspot.com/-meGCL-YNs38/W00q38--OLI/AAAAAAAAIkg/t5NxyrsswsYNrxP1zVK9ooTgC9bK_WgdACLcBGAs/s640/Captura%2Bde%2Btela%2Bde%2B2018-07-15%2B23-48-09.png "Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows")](https://3.bp.blogspot.com/-meGCL-YNs38/W00q38--OLI/AAAAAAAAIkg/t5NxyrsswsYNrxP1zVK9ooTgC9bK_WgdACLcBGAs/s1600/Captura%2Bde%2Btela%2Bde%2B2018-07-15%2B23-48-09.png)

  

Após o final do backup será mostrada a janela abaixo.

  

[![Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows](https://4.bp.blogspot.com/-ZTFVn6rXj_c/W00q4P8Ab2I/AAAAAAAAIkk/rmDXE6alhpIkjbyw6O3jwzS_ienwi-AnwCLcBGAs/s640/Captura%2Bde%2Btela%2Bde%2B2018-07-16%2B01-21-24.png "Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows")](https://4.bp.blogspot.com/-ZTFVn6rXj_c/W00q4P8Ab2I/AAAAAAAAIkk/rmDXE6alhpIkjbyw6O3jwzS_ienwi-AnwCLcBGAs/s1600/Captura%2Bde%2Btela%2Bde%2B2018-07-16%2B01-21-24.png)

  

Acesse a pasta /home/remaster e a iso estará lá. Você poderá copiá-la para a sua home, já que esta pasta tem acesso somente de leitura. Ou poderá gravá-la num DVD ou pendrive.

  

[![Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows](https://3.bp.blogspot.com/-lf4MolYBAIw/W00q4ZNLUQI/AAAAAAAAIko/c2y1PR_uHyM6qKG0Xm8j373yB7Jn7jx3ACLcBGAs/s640/Captura%2Bde%2Btela%2Bde%2B2018-07-16%2B01-26-21.png "Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows")](https://3.bp.blogspot.com/-lf4MolYBAIw/W00q4ZNLUQI/AAAAAAAAIko/c2y1PR_uHyM6qKG0Xm8j373yB7Jn7jx3ACLcBGAs/s1600/Captura%2Bde%2Btela%2Bde%2B2018-07-16%2B01-26-21.png)

  

Caso deseje apagar os arquivos gerados, utilize a opção Clear. **Mas cuidado!!!** Esta opção apaga tudo, inclusive a iso. Certifique-se de gravá-la num DVD ou Pendrive antes de utilizar esta opção.

  

[![Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows](https://2.bp.blogspot.com/-y0Y-6rBLBU4/W00q4mOXDDI/AAAAAAAAIks/vZLn8DfUD5ILN8TvjcZYIG8E_5FHoebDQCLcBGAs/s640/Captura%2Bde%2Btela%2Bde%2B2018-07-16%2B01-26-42.png "Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows")](https://2.bp.blogspot.com/-y0Y-6rBLBU4/W00q4mOXDDI/AAAAAAAAIks/vZLn8DfUD5ILN8TvjcZYIG8E_5FHoebDQCLcBGAs/s1600/Captura%2Bde%2Btela%2Bde%2B2018-07-16%2B01-26-42.png)

  

[![Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows](https://2.bp.blogspot.com/-4O_0GBz3IVk/W00q4x-Z3qI/AAAAAAAAIkw/PKtwThUSWcERrnyrfSGCuVpp5EPAIvsSQCLcBGAs/s640/Captura%2Bde%2Btela%2Bde%2B2018-07-16%2B01-27-00.png "Ferramentas Linux 1 - Backup com Remaster GTK - Dicas Linux e Windows")](https://2.bp.blogspot.com/-4O_0GBz3IVk/W00q4x-Z3qI/AAAAAAAAIkw/PKtwThUSWcERrnyrfSGCuVpp5EPAIvsSQCLcBGAs/s1600/Captura%2Bde%2Btela%2Bde%2B2018-07-16%2B01-27-00.png)

  

#### 4 - Considerações finais.

  

Após o backup você pode utilizá-lo como um live DVD e depois instalar em seu computador. Também é possível instalar numa máquina virtual.  
No início citei que há uma versão para Ubuntu. Baixe-a [aqui](https://linuxdicasesuporte.blogspot.com/p/remaster-gtk-ubuntu-e-derivados.html).