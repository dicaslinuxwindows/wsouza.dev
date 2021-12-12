---
title: 'Dropbox - Mudança de requisitos para sistemas Linux'
date: 2018-08-26T19:26:00.001-03:00
draft: false
url: /2018/08/dropbox-mudanca-de-requisitos-para-sistemas-linux.html
tags: 
- Linux
- Dicas
- Dropbox
---

Foi anunciado nesta semana que o cliente do Dropbox para Linux passará por algumas ações necessárias, que farão com que o mesmo não funcione em sistemas Linux mais antigos. Veja a seguir como será e o que fazer para continuar utilizando o Dropbox no Linux.

  
  
  

   [![](https://2.bp.blogspot.com/-OL4hXCZDAx8/W4NF2mzcPsI/AAAAAAAAJHE/-yPwGi_iZCs0yBoXUmJpKZYyuKutDlhMQCLcBGAs/s200/dropbox.png)](https://2.bp.blogspot.com/-OL4hXCZDAx8/W4NF2mzcPsI/AAAAAAAAJHE/-yPwGi_iZCs0yBoXUmJpKZYyuKutDlhMQCLcBGAs/s1600/dropbox.png)

  

**Desde já fica claro que o Dropbox não encerrará o suporte à sistemas Linux.**  
Veja o comunicado do Dropbox enviado aos usuários:  
_"Em 15 de outubro, o Dropbox encerrará a compatibilidade com o Ubuntu 13.10, Fedora 20 e versões anteriores. Você precisará do glibc 2.19 ou superior para continuar usando o aplicativo do Dropbox para desktop. Pedimos que atualize o sistema operacional para uma versão compatível do Linux (Ubuntu 14.04+ ou Fedora 21+) ou atenda aos [novos requisitos de sistema](https://www.dropbox.com/l/AABx5WsUv19St0HR6Ewmcp-Bp0u8Rc0zXa4#linux).  
A partir de 7 de novembro, o aplicativo do Dropbox para desktop no Linux será compatível apenas com o sistema de arquivos ext4. O Dropbox continuará sincronizando com os sistemas de arquivos compatíveis que usam criptografia de disco completo (por exemplo, LUKS). Note que ecryptfs não é compatível. Para garantir que seus arquivos continuem sincronizando corretamente, sua pasta do Dropbox precisará estar em um disco rígido ou partição que atenda aos novos [requisitos de sistema de arquivos](https://www.dropbox.com/l/AAD4xeRciRp_zNxeAo84W6t4rzDlfWqqfWA#desktop).  
Os dispositivos que não atendam aos requisitos de sistema operacional ou sistema de arquivos não poderão usar o aplicativo do Dropbox para desktop.  
Mas não se preocupe! Seus arquivos não vão desaparecer. Além dos sistemas operacionais Linux compatíveis, você ainda poderá acessar arquivos pelos aplicativos para Windows, Mac, iOS e Android ou pelo [dropbox.com](https://www.dropbox.com/) ..."_  

Devido a atualização do cliente Dropbox para a biblioteca _glibc 2.19_ não será mais possível a utilização do mesmo nas versões citadas dos sistemas citados acima e nas versões abaixo do Debian Jessie, por exemplo. Não chega a ser um problema que afetará tantos usuários se levarmos em conta que o Debian Jessie já é oldstable há 1 ano e sua versão anterior, o Debian Wheezy, já não recebe mais atualizações. No Ubuntu é a mesma idéia, já que a versão 13.10 também não recebe mais suporte. Quanto aos sistemas de arquivos pode ser que ocorram mais problemas, mas nada que não possa ser contornado - com um pouco de trabalho - só que será necessária uma reinstalação do sistema e mudança no sistema de arquivos e criptografia.  
Segue abaixo a lista de requisitos completa para sistemas Linux:  
Ambientes Desktop: Ubuntu (Unity) e GNOME Classic, XFCE, GNOME Shell. Se não houver suporte para seu ambiente, você poderá utilizar a linha de comando (_Veja [aqui](https://www.dropbox.com/help/desktop-web/linux-commands) como utilizar)_.  
Programas necessários: Glibc 2.19 ou superior, GTK 2.24 ou superior, Glib 2.40 ou superior, Libappindicator 12.10 ou superior, Nautilus 3.10.1 ou superior.

Resumindo: Quem deseja continuar utilizado o cliente Dropbox em sistemas Linux deverá atualizar o sistema para versões mais recentes. Debian >= Jessie; Ubuntu >=14.04; Fedora >=21.