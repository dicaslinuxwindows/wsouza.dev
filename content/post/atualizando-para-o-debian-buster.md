---
title: 'Atualizando para o Debian Buster '
date: 2019-07-02T21:19:00.001-03:00
draft: false
url: /2019/07/atualizando-para-o-debian-buster.html
tags: 
- Debian
- Linux
- Debian Buster
- Tutoriais
---

Se você está utilizando o Debian Jessie ou Stretch e deseja utilizar o Buster, mas não quer fazer uma instalação do zero e perder seus dados ou ter que configurar tudo novamente, veja nesta matéria como fazer.

  
  

[![Atualizando para o Debian Buster  -  Dicas Linux e Windows](https://4.bp.blogspot.com/-qu3NOriLr3M/XRvzo7b9LII/AAAAAAAALvs/HFqs9IZTw5EHUOVXhoMf6x1JvHiV1Uw6QCLcBGAs/s200/atualizar_para_buster.png "Atualizando para o Debian Buster  -  Dicas Linux e Windows")](https://4.bp.blogspot.com/-qu3NOriLr3M/XRvzo7b9LII/AAAAAAAALvs/HFqs9IZTw5EHUOVXhoMf6x1JvHiV1Uw6QCLcBGAs/s1600/atualizar_para_buster.png)

  

### Considerações iniciais

  

*   Este tutorial foi elaborado através da atualização do Debian Jessie diretamente para o Debian Buster, mas pode ser aplicado na atualização do Debian Stretch para o Buster.

*   Antes de atualizar para uma nova versão sugiro que faça um backup do sistema para uma eventual de necessidade de voltar à versão anterior¹. Uma boa maneira de efefuar um backup completo do sistema foi mostrada em [Backup com Remaster-GTK](https://info.wsouza.com.br/2018/07/backup-com-remaster-gtk.html).
*   Se em seu sistema houverem muitos programas de terceiros instalados, você poderá ter problemas na atualização. Considere desinstalar estes programas e instale-os após o fim da atualização.

  

### Preparando o sistema

  
Vamos garantir que a versão instalada está com todos os pacotes atualizados. Abra o terminal e execute os comandos abaixo.  
  

 sudo apt update && sudo apt full-upgrade

  
O próximo passo é atualizar a _sources.list_, que é a lista de repositórios onde estão os pacotes do Debian Buster. Faça um backup da lista antiga e depois crie um arquivo vazio utilizando os comandos abaixo:  
  

 sudo mv /etc/apt/sources.list /etc/apt/sources.list.bak

  

 touch /etc/apt/sources.list

  
Após, com seu editor de texto preferido² execute o comando abaixo. Este comando abrirá o arquivo criado anteriormente. Copie todo o conteúdo da _sources.list_ que está logo após o comando e cole. Após, salve o arquivo apertando as teclas CTRL+K+X, se estiver utilizando o Joe.  
  

 sudo joe /etc/apt/sources.list

  
```
  
`  
#sources.list Debian Buster  
  
deb http://deb.debian.org/debian/ buster main non-free contrib  
deb-src http://deb.debian.org/debian/ buster main non-free contrib  
  
deb http://security.debian.org/debian-security buster/updates main contrib non-free  
deb-src http://security.debian.org/debian-security buster/updates main contrib non-free  
  
# buster-updates, previously known as 'volatile'  
deb http://deb.debian.org/debian/ buster-updates main contrib non-free  
deb-src http://deb.debian.org/debian/ buster-updates main contrib non-free  
  
# buster-backports, previously on backports.debian.org  
deb http://deb.debian.org/debian/ buster-backports main contrib non-free  
deb-src http://deb.debian.org/debian/ buster-backports main contrib non-free  
`  

```  

### Atualizando o sistema

  
Utilizando os comando abaixo você vai atualizar os repositórios e será listada a quantidade de pacotes que será atualizada.  
  

 sudo apt update && sudo apt full-upgrade

  
Confirme e o processo de atualização será iniciado. O processo poderá ser bem demorado, pois a quantidade de pacotes que serão baixado é alta e a instalação também demora. Durante a instalação você precisa ficar atento às perguntas que o instalador fará. Em caso de dúvidas utilize a opção padrão, apertando enter.  
  
Se em algum momento aparecer a mensagem abaixo:  
```
  
`  
Repository 'http://security.debian.org/debian-security buster/updates InRelease'   
changed its 'Suite' value from 'testing' to 'stable'  
  
N: This must be accepted explicitly before updates for this repository can be applied.  
See apt-secure(8) manpage for details.  
`  

```  
Utilize o comando abaixo para solucionar.  
  

 apt --allow-releaseinfo-change update

  

### Notas

¹ Geralmente a atualização ocorre com sucesso, mas por diversos motivos, podem ocorrer alguns problemas. Por este motivo é importante ter em mãos um backup.  
² Utilizo o editor **joe** _(sudo apt install joe)_ por questão de costume mesmo, mas você pode utilizar qualquer outro editor como o Vi/Vim, Nano, ou editores gráficos como Gedit, Kate, Pluma, Geany...