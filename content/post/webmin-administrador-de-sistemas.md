---
title: 'Webmin - Administrador de Sistemas'
date: 2019-01-22T13:35:00.000-02:00
draft: false
url: /2019/01/webmin-administrador-de-sistemas.html
tags: 
- Linux
- Tutoriais
- Ferramentas Linux
- Webmin
---

Conheça o Webmin, um administrador de sistemas via web que possui ferramentas de controle total de um dispositivo remoto.  
Uma boa alternativa frente ao Secure Shell _SSH_. Confira mais detalhes na matéria abaixo.

  
  

[![Webmin - Administrador de Sistemas - Dicas Linux e Windows](https://2.bp.blogspot.com/-sCieAZJVURo/XEbuvOSUT3I/AAAAAAAAKLs/iI9lpn95KzA8oYtpJAw3puF2J9GcFk-iwCLcBGAs/s320/webmin.png "Webmin - Administrador de Sistemas - Dicas Linux e Windows")](https://2.bp.blogspot.com/-sCieAZJVURo/XEbuvOSUT3I/AAAAAAAAKLs/iI9lpn95KzA8oYtpJAw3puF2J9GcFk-iwCLcBGAs/s1600/webmin.png)

### 1 - O que é o Webmin?

  
Segundo o site do Webmin: _"O Webmin é uma interface baseada na Web para administração do sistema para o Unix. Usando qualquer navegador moderno, você pode configurar contas de usuário, Apache, DNS, compartilhamento de arquivos e muito mais. O Webmin elimina a necessidade de editar manualmente os arquivos de configuração do Unix (...) e permite gerenciar um sistema a partir do console ou remotamente."_  
O Webmin dá controle total para o usuário realizar a administração do sistema, tanto localmente, como remotamente, de maneira rápida e prática. Além de possuir diversos módulos que já vem ativados por padrão e permitir a ativação de diversos módulos.  
No Webmin o administrador acessa o sistema pelo usuário root _(superusuário)_ ou usuário com permissão no arquivo sudo.  
Veja a lista com os [módulos padrão](http://www.webmin.com/standard.html).  
  

### 1.1 - Variações do Webmin

  
O foco aqui é o Webmin mas vamos abrir um parêntese e mostrar algumas variações do Webmin.  
Uma delas é o [Usermin](http://www.webmin.com/usermin.html), que possui ferramentas para webmail, alteração de senha, filtros de correio, fetchmail, voltada à usuários não-root.  
Outra variação é o [Virtalmin](http://www.webmin.com/virtualmin.html) que, segundo o site: _"É um módulo Webmin para gerenciar múltiplos hosts virtuais através de uma única interface, como o Plesk ou o Cpanel. Ele suporta a criação e o gerenciamento de hosts virtuais Apache, domínios DNS BIND, bancos de dados MySQL e caixas de correio e aliases com Sendmail ou Postfix."_  
Ainda podemos encontrar o [Cloudmin](http://www.webmin.com/cloudmin.html) que é uma interface de usuário construída sobre o Webmin para gerenciar sistemas virtuais, como instâncias de Xen, KVM e OpenVZ.  
  

### 2 - E a segurança?

  
A segurança depende de vários fatores. Na página do Webmin há uma seção que mostra os problemas de segurança encontrados, as versões afetadas e a solução para corrigir o problema. Veja em: [http://www.webmin.com/security.html](http://www.webmin.com/security.html)  
Porém, como o usuário que acessa o sistema tem acesso root, este deve tomar alguns cuidados ao utilizar alguns módulos. O gerenciador de arquivos, por exemplo, é um módulo que permite apagar qualquer arquivo do sistema e, dependendo do arquivo excluído, o sistema pode deixar de iniciar. Portanto, mais do que cuidados com segurança - no que diz respeito à ataques externos - deve-se ter cuidado com o que você vai fazer. Em caso de dúvidas, pesquise antes de tomar alguma atitude.  
  

### 3 - Download e instalação

  
Na página de download, em [http://www.webmin.com/download.html](http://www.webmin.com/download.html), encontramos pacotes pré-compilados para Debian/Ubuntu e derivados _(.deb)_, Redhat, Fedora, CentOS, SuSE, Mandrake Linux _(.rpm)_. Há também pacotes para Solaris e Windows, além do código fonte, compilável para qualquer distribuição Linux.  
Vou utilizar como base a instalação para Debian/Ubuntu. Para isto baixe o pacote em .deb na página de downloads, ou se preferir:  
  

wget http://prdownloads.sourceforge.net/webadmin/webmin\_1.900\_all.deb

  
O Webmin depende de algumas dependências de bibliotecas perl e python _(pois o mesmo é desenvolvido nestas linguagens)_, que podem ou não já estar instaladas no seu sistema. Também, em alguns casos, depende do sudo. Por via das dúvidas execute os comandos abaixo para instalar todas as dependências necessárias.  
Obs: No Ubuntu, ao contrário do Debian, o sudo já vem como padrão. Para instalá-lo no Debian, no terminal execute o comando:  
  

su

  
Digite a senha e você estará logado como superusuário:  
Execute o comando abaixo:  
  

apt-get install perl libnet-ssleay-perl openssl libauthen-pam-perl libpam-runtime libio-pty-perl apt-show-versions python sudo gksu

  
Agora vamos efetivamente instalar o Webmin:  
  

dpkg --install webmin\_1.900\_all.deb

  
Para testar acesse https://localhost:10000, se instalou na máquina local. Caso tenha instalado numa outra máquina acesse https://ip-do-computador-que-foi-instalado:10000. Será pedido o login e senha. Você pode utilizar tanto o usuário root, como o seu usuário (desde que este esteja no sudo).  
As eventuais atualizações aparecerão como sugestão quando você estiver na tela do Webmin. Caso deseje instalar basta confirmar e o processo correrá de forma automática.  
  

### 4 - Caso de uso

  
Como exemplo criei um servidor num computador antigo, que já não suporta mais ambiente gráfico, rodando com o Debian Jessie. Instalei o Webmin e ativei e configurei os módulos de Servidor Web Apache, SSH, Servidor Proxy Squid, Servidor e Gerenciador de Banco de Dados Mysql e Servidor de Arquivos Samba. Como a configuração da máquina utilizada é fraca, tomei o cuidado para não deixá-los todos ativados ao mesmo tempo. Abaixo vou mostrar algumas telas do Webmin rodando nesta máquina. Clique na imagem para visualizar em melhor qualidade.

  

  
A tela abaixo é a principal, onde aparecem os dados da máquina e à esquerda os menus para escolha dos módulos. No menu Webmin estão as opções de configuração do próprio Webmin. No menu sistema encontramos as opções de gerenciamento do sistema como criação e exclusão de usuários e grupos, módulo iniciar e encerrar _(que escolhe os programas que "subirão" junto com o sistema)_, entre outras.  
  

[![Webmin - Administrador de Sistemas - Dicas Linux e Windows](https://1.bp.blogspot.com/-2NsxQoZx648/XEZ8HuqdD1I/AAAAAAAAKLk/v292yJJX23Mqg6dIhB4rOxbDdk71nnVegCPcBGAYYCw/s640/Captura%2Bde%2Btela%2Bde%2B2019-01-09%2B23-52-06.png "Webmin - Administrador de Sistemas - Dicas Linux e Windows")](https://1.bp.blogspot.com/-2NsxQoZx648/XEZ8HuqdD1I/AAAAAAAAKLk/v292yJJX23Mqg6dIhB4rOxbDdk71nnVegCPcBGAYYCw/s1600/Captura%2Bde%2Btela%2Bde%2B2019-01-09%2B23-52-06.png)

  
Módulo que permite o gerenciamento total do Servidor de Arquivos Samba. Permite o compartilhamento de impressoras e pastas entre computadores com sistemas Windows ou Linux.  
  

[![Webmin - Administrador de Sistemas - Dicas Linux e Windows](https://3.bp.blogspot.com/-fiI4J-VslWw/XEZ8IKrzMxI/AAAAAAAAKLc/qWbZ4nnECi0LWSK0Ju4CT886phPrSn_AgCPcBGAYYCw/s640/Captura%2Bde%2Btela%2Bde%2B2019-01-09%2B23-55-58.png "Webmin - Administrador de Sistemas - Dicas Linux e Windows")](https://3.bp.blogspot.com/-fiI4J-VslWw/XEZ8IKrzMxI/AAAAAAAAKLc/qWbZ4nnECi0LWSK0Ju4CT886phPrSn_AgCPcBGAYYCw/s1600/Captura%2Bde%2Btela%2Bde%2B2019-01-09%2B23-55-58.png)

  
Módulo do Servidor de Proxy Squid. Neste módulo é possível criar regras para controle de acesso à sites e controle de tráfego de rede.  

[![Webmin - Administrador de Sistemas - Dicas Linux e Windows](https://2.bp.blogspot.com/-Og1qyH4d5Mc/XEZ8IkGfJZI/AAAAAAAAKLM/1NHzdaLyrLkNgUp0Bqym3kP_-M4tleK9QCPcBGAYYCw/s640/Captura%2Bde%2Btela%2Bde%2B2019-01-09%2B23-57-06.png "Webmin - Administrador de Sistemas - Dicas Linux e Windows")](https://2.bp.blogspot.com/-Og1qyH4d5Mc/XEZ8IkGfJZI/AAAAAAAAKLM/1NHzdaLyrLkNgUp0Bqym3kP_-M4tleK9QCPcBGAYYCw/s1600/Captura%2Bde%2Btela%2Bde%2B2019-01-09%2B23-57-06.png)

  
Módulo de configuração e administração do Servidor Web Apache. Permite o gerenciamento total do servidor Web.  

[![Webmin - Administrador de Sistemas - Dicas Linux e Windows](https://4.bp.blogspot.com/-thqqxk7DA1Q/XEZ8IvNHYSI/AAAAAAAAKLQ/1Na6E9DPwSo9jmXtdAwGJOsbhLfVwCWYwCPcBGAYYCw/s640/Captura%2Bde%2Btela%2Bde%2B2019-01-09%2B23-57-31.png "Webmin - Administrador de Sistemas - Dicas Linux e Windows")](https://4.bp.blogspot.com/-thqqxk7DA1Q/XEZ8IvNHYSI/AAAAAAAAKLQ/1Na6E9DPwSo9jmXtdAwGJOsbhLfVwCWYwCPcBGAYYCw/s1600/Captura%2Bde%2Btela%2Bde%2B2019-01-09%2B23-57-31.png)

  
Módulo de configuração e administração do servidor SSH.  

[![Webmin - Administrador de Sistemas - Dicas Linux e Windows](https://4.bp.blogspot.com/-H1weQr_ON5o/XEZ8I6p6SGI/AAAAAAAAKLU/DVg391HEW88x7169IPWEQNTUzSsnKeE0QCPcBGAYYCw/s640/Captura%2Bde%2Btela%2Bde%2B2019-01-09%2B23-57-46.png "Webmin - Administrador de Sistemas - Dicas Linux e Windows")](https://4.bp.blogspot.com/-H1weQr_ON5o/XEZ8I6p6SGI/AAAAAAAAKLU/DVg391HEW88x7169IPWEQNTUzSsnKeE0QCPcBGAYYCw/s1600/Captura%2Bde%2Btela%2Bde%2B2019-01-09%2B23-57-46.png)

  
Módulo gerenciador de arquivos. Este módulo permite o acesso à qualquer arquivo do sistema. Em arquivos de texto ele permite a edição. Use este módulo com cuidado, pois como citei anteriormente, qualquer descuido poderá fazer com que você perca um arquivo importante para o sistema, impedindo-o de iniciar.  

[![Webmin - Administrador de Sistemas - Dicas Linux e Windows](https://2.bp.blogspot.com/-UI4y--bG7sU/XEZ8KZgSD5I/AAAAAAAAKLg/2-SMiAITEIgdjQONaLX3IQHtc23SXW8zwCPcBGAYYCw/s640/Captura%2Bde%2Btela%2Bde%2B2019-01-09%2B23-58-58.png "Webmin - Administrador de Sistemas - Dicas Linux e Windows")](https://2.bp.blogspot.com/-UI4y--bG7sU/XEZ8KZgSD5I/AAAAAAAAKLg/2-SMiAITEIgdjQONaLX3IQHtc23SXW8zwCPcBGAYYCw/s1600/Captura%2Bde%2Btela%2Bde%2B2019-01-09%2B23-58-58.png)

  
Módulo administrador do servidor de impressão CUPS. Aqui é possível instalar, configurar e excluir impressoras, além de controlar os trabalhos de impressão.  

[![Webmin - Administrador de Sistemas - Dicas Linux e Windows](https://3.bp.blogspot.com/-q8FdQnHrU6Y/XEZ8MfUVy0I/AAAAAAAAKLY/wupgSNXUk3IwfvzZct2Bj96ijOT2CGHOwCPcBGAYYCw/s640/Captura%2Bde%2Btela%2Bde%2B2019-01-10%2B00-02-01.png "Webmin - Administrador de Sistemas - Dicas Linux e Windows")](https://3.bp.blogspot.com/-q8FdQnHrU6Y/XEZ8MfUVy0I/AAAAAAAAKLY/wupgSNXUk3IwfvzZct2Bj96ijOT2CGHOwCPcBGAYYCw/s1600/Captura%2Bde%2Btela%2Bde%2B2019-01-10%2B00-02-01.png)

  
Módulo do banco de dados MySql. Neste módulo é possível criar, administrar e excluir banco de dados e usuários. Também é possível parar e iniciar o banco de dados e alterar as mais variadas configurações.  

[![Webmin - Administrador de Sistemas - Dicas Linux e Windows](https://2.bp.blogspot.com/-diXgK3B8JXc/XEZ8IZdr5TI/AAAAAAAAKLk/EJh68SZ4TGU4ND_nPdV3r8PczuXkoZ82wCPcBGAYYCw/s640/Captura%2Bde%2Btela%2Bde%2B2019-01-09%2B23-56-37.png "Webmin - Administrador de Sistemas - Dicas Linux e Windows")](https://2.bp.blogspot.com/-diXgK3B8JXc/XEZ8IZdr5TI/AAAAAAAAKLk/EJh68SZ4TGU4ND_nPdV3r8PczuXkoZ82wCPcBGAYYCw/s1600/Captura%2Bde%2Btela%2Bde%2B2019-01-09%2B23-56-37.png)

  
As imagens acima são uma pequena amostra das possibilidades que o Webmin permite. Nos menus à esquerda vemos várias categorias e, se uma ferramenta não aparecer em algum menu, ainda podemos verificar a disponibilidade dentre do menu _Módulos não utilizados_. Se o módulo está ali significa que a ferramenta que ele controla não está instalada no sistema, mas o próprio módulo dará a opção de instalação. Esta instalação acontece por meio do APT e dos repositórios da máquina onde o Webmin está instalado, portanto, não há preocupação com instalação por fontes desconhecidas.  
  

### 5 - Considerações finais

Tenho utilizado o Webmin já há alguns anos e sempre tem me atendido bem, sua interface é intuitiva e, tomando as devidas precauções, não há como causar problemas.  
Para quem não conhecia e achou interessante, experimente instalar num sistema que está numa máquina virtual. Assim você poderá conhecer e todos os módulos e suas configurações possíveis, sem medo de causar danos à seu sistema.