---
title: 'Remastersys - Um ótimo utilitário de backup para Ubuntu'
date: 2013-01-27T00:02:00.000-02:00
draft: false
url: /2013/01/remastersys-um-otimo-utilitario-de.html
tags: 
- Criar Backup do Sistema
- Ubuntu
- Tutoriais
- Remastersys
---

  
O Remastersys foi descontinuado, porém, existe o Remaster-GTK, um fork do Remastersys.  
Leia em [Backup com Remaster-GTK](https://info.wsouza.com.br/2018/07/backup-com-remaster-gtk.html)  
  
Após muito trabalho você finalmente conseguiu configurar seu Ubuntu da maneira que desejava, instalou programas que você gosta, removeu programas desnecessários, instalou temas e ícones, modificou as fontes,enfim, deixou o Ubuntu com a sua cara. Então, surge a necessidade de você formatar seu Notebook/PC e você fica desesperado pois precisará configurar tudo novamente e sabe que a trabalheira não será fácil.  
Para resolver este problema existe o [Remastersys](http://www.remastersys.com/), um utilitário para Debian/Ubuntu que, além de outras funções, realiza um backup completo de seu sistema e gera numa ISO um Live Cd onde você pode acessar o sistema sem instalar no HD, mas também tornando possível a reinstalação do sistema operacional, deixando-o do mesmo modo que ele estava antes da formatação.  
O objetivo desta dica é mostrar como funciona o processo de backup utilizando o [Remastersys](http://www.remastersys.com/) para o Ubuntu mas o processo para Debian praticamente o mesmo.

Primeiramente baixe a versão equivalente à versão de seu Ubuntu. Para versões acima da 12.04 (Precise) a dica é a seguinte:  
No terminal, logado como root _(sudo su)_ utilize o comando:  
**wget -O - http://www.remastersys.com/ubuntu/remastersys.gpg.key | apt-key add -**  
Este comando baixa as chaves do software.  
  
Edite o arquivo /etc/apt/sources.list com o comando **sudo gedit /etc/apt/sources.list** e no final do arquivo insira os comandos a seguir:  
**_#Remastersys Precise  
deb http://www.remastersys.com/ubuntu precise main_**  
Salve o arquivo.  
  
Para atualizar os pacotes digite:  
**sudo apt-get update **  
Para iniciar, procure pelo remastersys no painel inicial do Unity ou, simplesmente, digite **sudo remastersys-gtk** no terminal e interface principal estará aberta. Como aqui o foco é apenas a opção de backup a utilização torna-se bem simples, mas é necessário fazer algumas pequenas configurações, então vamos vê-las.

Na figura abaixo estamos na aba **_Settings_** e, é nesta aba que configuramos praticamente tudo.  
  

[![remastersys](https://lh3.ggpht.com/-UivhKFtCTIg/UQR_NFJS08I/AAAAAAAAALI/qpy9qfq5rXc/s400/remaster02.png "remastersys")](http://1.bp.blogspot.com/-UivhKFtCTIg/UQR_NFJS08I/AAAAAAAAALI/qpy9qfq5rXc/s1600/remaster02.png)

No campo **Username** você pode inserir o nome do usuário principal do sistema operacional que deseja fazer backup, na verdade é desejável que você coloque o mesmo nome pois, poderá ter problemas quando tentar utilizar o backup.  
No campo **CD Label** você pode colocar o nome que deseja dar à sua ISO, que posteriormente, será o nome de seu Cd/Dvd de backup.  
No campo **Filename** vocẽ pode colocar um nome personalizado para o arquivo ISO gerado _Ex: Backup\_Ubuntu.iso_ mas, vale lembrar que você sempre deve dar um nome com a extensão **.iso** no final.  
Outro campo importante é o **Working directory**. Aqui você deve escolher uma pasta onde irá salvar a image ISO gerada, comedo que deixe-o como está e assim sua imagem gerada será salva na pasta /home/remastersys/...  
Nas opções seguintes você pode deixar tudo como está e volte para a aba **Actions**, que é a aba principal.  

[![remastersys](https://lh3.ggpht.com/-UmqR-Z0ydGo/UQSCWS8TkpI/AAAAAAAAALg/S1GAzqnMk20/s400/remaster01.png "remastersys")](http://3.bp.blogspot.com/-UmqR-Z0ydGo/UQSCWS8TkpI/AAAAAAAAALg/S1GAzqnMk20/s1600/remaster01.png)

Nesta aba, você pode escolher o usuário que será iniciado como usuário principal e todas as suas configurações serão aplicadas quando você iniciar o Cd/DVD de Backup. Você deve ter cuidado de utilizar um usuário que possua um arquivo _/home_ não muito grande pois a ISO poderá não caber num DVD. O ideal é que você possua seus dados (fotos, músicas, vídeos, arquivos grandes) salvos em outra partição de seu disco rígido.  
Realizadas todas as configurações, vamos finalmente realizar o backup. Feche todos os programas, arquivos e janelas abertas e deixe apenas a janela do remastersys. Clique na opção **Backup** , dê OK na mensagem e aguarde o final do processo, que será um pouco demorado. Detalhe: Não interrompa o processo.  
Ao final do processo você terá um backup completo o seu sistema e serão gerados 2 arquivos com o nome que você escolheu lá em cima no campo Filename. Estes arquivos estarão na pasta /home/remastersys/remastersys (ou outra que você tenha escolhido no campo working directory). Você deve gravar o arquivo com a extensão .iso num CD/DVD (sugiro gravar num DVD regravável) após isto, utilize a opção **Limpar** para remover o arquivos temporários que provavelmente estarão ocupando bastante espaço em seu HD.

Se quiser testar, é só reiniciar o PC/Notebook com o CD/DVD gerado. Você irá se deparar com o gerenciador de inicialização, escolha a opção de live cd se quiser apenas rodar como um live cd, mas também poderá escolher a opção de instalar.  
Dica preciosa: Não recomendo que você grave a ISO num Pendrive pois, na hora da instalação dá um erro, não instala o Grub e a instalação não termina, isto não ocorre quando gravado num CD/DVD.