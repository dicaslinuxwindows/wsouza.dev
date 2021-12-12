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

#### Cara gostei do seu post. Bem escrito simples enten...
[Cleyton](https://www.blogger.com/profile/03477545733520925234 "noreply@blogger.com") - <time datetime="2019-07-10T13:26:57.280-03:00">Jul 3, 2019</time>

Cara gostei do seu post. Bem escrito simples entendimento, parabéns  
So que infelizmente não funciona no debian 9 De forma alguma.
<hr />
#### Valeu pelo elogio. Pode explicar melhor? O que exa...
[W. Souza](https://www.blogger.com/profile/13145950875273640819 "noreply@blogger.com") - <time datetime="2019-07-10T16:12:29.615-03:00">Jul 3, 2019</time>

Valeu pelo elogio. Pode explicar melhor? O que exatamente não funcionou? A instalação do Remaster? A geração da ISO?  
Esecifique melhor para eu ver onde posso ajudar.
<hr />
#### Comigo não foi. Gerou uma ISO de mais de 8Gb.
[Marcello Marinho Costa de Oliveira](https://www.blogger.com/profile/06219126256559999109 "noreply@blogger.com") - <time datetime="2019-11-02T09:43:09.440-03:00">Nov 6, 2019</time>

Comigo não foi. Gerou uma ISO de mais de 8Gb.
<hr />
#### Tudo depende do tamanho da pasta /home e dos aplic...
[W. Souza](https://www.blogger.com/profile/13145950875273640819 "noreply@blogger.com") - <time datetime="2019-11-02T18:23:44.968-03:00">Nov 6, 2019</time>

Tudo depende do tamanho da pasta /home e dos aplicativos instalados.  
Eu geralmente deixo os documentos, músicas, fotos, vídeos numa partição de dados separada da /home, assim, quando faço o backup a ISO fica bem menor, com cerca de 3 a 4 GB. Neste exemplo da matéria ficou com 1,2 GB porque eu havia acabado de instalar o sistema.
<hr />
#### Olá, tenho uma ISO realizada com a opção backup, p...
[Unknown](https://www.blogger.com/profile/02260106677985214865 "noreply@blogger.com") - <time datetime="2020-06-05T15:45:21.332-03:00">Jun 5, 2020</time>

Olá, tenho uma ISO realizada com a opção backup, porém, fui tentar instalar de volta esse sistema em outro HD, o sistema voltou normal, mas o usuário "antigo" simplesmente some na nova instalação. Alguma dica do que pode ser?
<hr />
#### No momento da instalação crie um usuário qualquer....
[W. Souza](https://www.blogger.com/profile/13145950875273640819 "noreply@blogger.com") - <time datetime="2020-06-05T16:23:14.485-03:00">Jun 5, 2020</time>

No momento da instalação crie um usuário qualquer. Após instalado, entre com o usuário antigo.
<hr />
#### Boa noite. Comigo na pasta remaster gerou todas as...
[fui eu](https://www.blogger.com/profile/18180194879820369853 "noreply@blogger.com") - <time datetime="2020-08-23T22:07:58.015-03:00">Aug 0, 2020</time>

Boa noite.  
Comigo na pasta remaster gerou todas as pastas e o arquivo remaster.iso.md5 e remaster.log, mas não o remaster.iso.  
O que pode ser?
<hr />
#### Boa noite. Está usando a versão do Debian ou do Ub...
[W. Souza](https://www.blogger.com/profile/13145950875273640819 "noreply@blogger.com") - <time datetime="2020-08-25T23:31:48.874-03:00">Aug 2, 2020</time>

Boa noite.  
Está usando a versão do Debian ou do Ubuntu? Utilizou a versão mais recente?
<hr />
#### Bom dia amigo! É possivel gerar uma iso sem a int...
[Luiz](https://www.blogger.com/profile/12477095589055187241 "noreply@blogger.com") - <time datetime="2020-11-05T07:18:59.680-03:00">Nov 4, 2020</time>

Bom dia amigo!  
  
É possivel gerar uma iso sem a interface gráfica?
<hr />
#### Deixa eu explicar melhor aqui. Eu tenho um uma VM ...
[Luiz](https://www.blogger.com/profile/12477095589055187241 "noreply@blogger.com") - <time datetime="2020-11-05T07:36:01.612-03:00">Nov 4, 2020</time>

Deixa eu explicar melhor aqui. Eu tenho um uma VM com o Debian 10 sem interface gráfica e instalei o Remaster GTK, até ai tudo bem, consegui instalar tranquilo. Encontrei alguns tutoriais que ensinam a criar a ISO para distribuição via linha de comando e a executei, onde foi gerado uma ISO e ao subir em outra VM, rodou como live uma maravilha. Porem não consegui instalar essa live no disco. No boot não dá nenhuma opção para instalação, só para ser usado como live e o meu intuito é justamente instalar em outra maquina. Como eu faria isso? Teria alguma forma de instalar no disco?  
  
Desde já parabéns pelo artigo. Grato.
<hr />
#### Boa noite. Eu sei que existe uma forma de gerar a ...
[W. Souza](https://www.blogger.com/profile/13145950875273640819 "noreply@blogger.com") - <time datetime="2020-11-05T21:47:25.478-03:00">Nov 4, 2020</time>

Boa noite.  
Eu sei que existe uma forma de gerar a ISO pelo terminal, porém nunca utilizei, daí não sei o resultado no momento de instalar.  
Mas passei por uma situação como a sua e resolvi da seguinte forma:  
Instalei a interface LXDE, que gera o download de pouca coisa. Depois gerei a ISO e instalei no servidor. Depois de instalado, removi a interface gráfica e deixei apenas o terminal.
<hr />
#### Obrigado W. Souza. Acabei fazendo isso mesmo em se...
[Luiz](https://www.blogger.com/profile/12477095589055187241 "noreply@blogger.com") - <time datetime="2021-03-23T15:15:11.545-03:00">Mar 2, 2021</time>

Obrigado W. Souza. Acabei fazendo isso mesmo em seguida. Pois, tentei de todas as formas mas na hora de instalar a ISO gerada não encontrei uma solução já que quem faz a instalação é o Calamares e não encontrei em nenhum local nas profundezas da internet, algo para instalar sem ser o bendito Calamares que só funciona com interface gráfica. Uma pena mas funcionou de boas.
<hr />
#### As versões mais antigas, antes da versão para o De...
[W. Souza](https://www.blogger.com/profile/13145950875273640819 "noreply@blogger.com") - <time datetime="2021-04-05T23:51:20.853-03:00">Apr 1, 2021</time>

As versões mais antigas, antes da versão para o Debian 10, vinham sem o Calamares.
<hr />
