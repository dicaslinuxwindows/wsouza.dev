---
title: 'Reinstalar o Grub 2 utilizando um Live Cd do Ubuntu'
date: 2013-01-08T03:26:00.003-02:00
draft: false
url: /2013/01/reinstalando-o-grub2-utilizando-um-live.html
tags: 
- Linux
- Tutoriais
- Recuperar Grub
---

Esta dica serve para quem precisou reinstalar o Windows e, quando reiniciou, percebeu que havia perdido o acesso ao Ubuntu. Isto é muito comum de acontecer e muitas pessoas, no desespero, acabam reinstalando o Ubuntu sem necessidade, perdendo tempo e às vezes, arquivos importantes. Existem diversas maneiras de instalar o Grub, mas a dica que segue foi a mais simples que utilizei até hoje e com alguns ajustes sempre funcionou.  
  
Então, vamos começar: Você vai precisar de um Live Cd/Dvd do Ubuntu, utlilize uma versão acima da 9.10 (Karmic Koala) pois, foi a partir desta versão que o Grub2 passou a fazer parte do Ubuntu.  
Inicie o seu computador com o Live Cd.  
Após iniciado o sistema abra o terminal e digite o seguinte comando:  
**sudo fdisk -l**  
Você verá as partições existentes em seu disco, como está na imagem abaixo.  
  

[![Recuperar o Grub](https://1.bp.blogspot.com/-mT381UN6cLQ/UTidYFuPtGI/AAAAAAAAAQ8/t8-J1HdVbo0/s640/img01.png "Recuperar o Grub")](http://1.bp.blogspot.com/-mT381UN6cLQ/UTidYFuPtGI/AAAAAAAAAQ8/t8-J1HdVbo0/s1600/img01.png)

  

  
Descubra em qual partição seu Ubuntu está instalado. Neste caso a partição onde o Ubuntu está instalado é /dev/sda4, mas provavelmente não será este o seu caso. Monte o sistema de arquivos com o comando:  
**sudo mount /dev/sda4 /mnt**  
Neste ponto, o sistema antigo já está montado, então aproveite e monte os outros dispositivos dentro dele.  
**sudo mount --bind /dev /mnt/dev**  
Agora vamos acessar o diretório raíz do sistema antigo com o comando chroot, desta maneira você consegue administrá-lo via terminal.  
**sudo chroot /mnt**  
O próximo passo é atualizar o arquivo de configuração do grub.  
**sudo update-grub**  
Agora vamos efetivamente reinstalar o Grub2 na MBR. A MBR é o local onde ficam guardadas as informações de boot e sempre que instalamos o Windows ela é apagada, ficando apenas as informações do Windows  
O primeiro passo é reinstalar o Grub2 na MBR. Preste atenção que é apenas /dev/sda, e não sda1, sda2, sda4...  
**sudo grub-install /dev/sda**  
Pressione **Ctrl+D** para sair do sistema antigo.  
Desmonte os todos os dispositivos montados anteriormente.  
**sudo umount /mnt/dev**  
**sudo umount /mnt**  
Reinicie o sistema e retire o Live Cd da bandeja. **sudo reboot**  
Ao reiniciar você perceberá que o Grub está instalado mas, em alguns casos haverá um problema: o Windows não aparece, aparece apenas o Ubuntu.  
Para resolver este problema reinicie normalmente, faça o login, abra o terminal atualize o arquivo de configuração do Grub novamente com o comando:  
**sudo update-grub**  
Reinicie novamente o sistema.  
**sudo reboot**  
  
Pronto! Você agora estará com o Windows e o Ubuntu instalados e poderá escolher o qual desejar. Creio que esta dica funcione com outras distribuições, e não apenas com o Ubuntu, mas não testei, que tal tentar?