---
title: 'Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu'
date: 2019-08-19T13:25:00.004-03:00
draft: false
url: /2019/08/gosta-das-fontes-ubuntu-veja-como-instalar-em-seu-sistema-linux-e-deixa-lo-com-a-mesma-aparencia-do-ubuntu.html
tags: 
- Linux
- Ubuntu
- Fontes Ubuntu
---

Veja nesta matéria como personalizar o visual de seu sistema operacional instalando as fontes do Ubuntu.

  
  
  
  

[![Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu  - Dicas Linux e Windows](https://2.bp.blogspot.com/-aqmZDV6EQFA/XVttNTxYMOI/AAAAAAAAMKw/lJkltw1I9ccA1jjJ4XbEIquKGGmerVB4ACLcBGAs/s1600/Ubuntu-Fonts.png "Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu  - Dicas Linux e Windows")](https://2.bp.blogspot.com/-aqmZDV6EQFA/XVttNTxYMOI/AAAAAAAAMKw/lJkltw1I9ccA1jjJ4XbEIquKGGmerVB4ACLcBGAs/s1600/Ubuntu-Fonts.png)

  

Uma das coisas mais legais do Ubuntu é o visual, e boa parte desta beleza visual deve-se às suas fontes.  
Se você não é usuário do Ubuntu e deseja deixar utilizar as fontes veja como instalar em dois passos.  
  
1º passo: Abra o terminal e insira o comando:  
  

 wget -O ubuntufonts.tar.gz https://www.dropbox.com/s/ge12zkzsosfsc24/ubuntufonts.tar.gz?dl=1

  
2º passo: Ainda no terminal, primeiramente vamos criar a pasta _ubuntu-font_ dentro da pasta de fontes do sistema. Depois vamos descompactar o arquivo gerado anteriormente e movê-lo para a pasta criada.  
  

 sudo mkdir /usr/share/fonts/ubuntu-font/

  

 sudo tar -vzxf ubuntufonts.tar.gz -C /usr/share/fonts/ubuntu-font/

  
Pronto. As fontes estão instaladas.  
Se preferir instalar via interface gráfica descompacte o arquivo que foi baixado no primeiro passo, abra um a um os arquivos gerados e, como mostrado na imagem abaixo, clique em _Instalar Fonte._  
  

[![Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu  - Dicas Linux e Windows](https://4.bp.blogspot.com/-mMvBF4pcrvA/XVjeV2-AaRI/AAAAAAAAMJY/afJ_A3Kh9Eo1NycU9l6YgfuCjIt1nxLrwCLcBGAs/s640/Captura%2Bde%2Btela%2Bem%2B2019-08-18%2B02-09-58.png "Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu  - Dicas Linux e Windows")](https://4.bp.blogspot.com/-mMvBF4pcrvA/XVjeV2-AaRI/AAAAAAAAMJY/afJ_A3Kh9Eo1NycU9l6YgfuCjIt1nxLrwCLcBGAs/s1600/Captura%2Bde%2Btela%2Bem%2B2019-08-18%2B02-09-58.png)

  

### Alterando as fontes

Agora já é possível configurar a fonte Ubuntu como padrão do ambiente gráfico. Testei apenas no GNOME e no MATE, mas nos outros ambientes gráficos, mas a ideia é a mesma.  
Se você utiliza o ambiente gráfico GNOME você precisará do Gnome Tweak Tool _(ou Gnome Tweaks)_.  
No GNOME, procure no menu por Ajustes.  
  

[![Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu  - Dicas Linux e Windows](https://2.bp.blogspot.com/-51b9AxgXRkU/XVoPhwwpk0I/AAAAAAAAMJ4/JuOSeUS_op06VX0asPK874vr6z0_UBXhgCLcBGAs/s640/06.png "Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu  - Dicas Linux e Windows")](https://2.bp.blogspot.com/-51b9AxgXRkU/XVoPhwwpk0I/AAAAAAAAMJ4/JuOSeUS_op06VX0asPK874vr6z0_UBXhgCLcBGAs/s1600/06.png)

  
E deixe configurado como a imagem abaixo  
  

[![Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu  - Dicas Linux e Windows](https://2.bp.blogspot.com/-ZDyGxyVDlcw/XVoPh-WD3LI/AAAAAAAAMKA/5qgKuS-Ba0cn2aoGeXr199qQhZDZM72CwCLcBGAs/s640/05.png "Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu  - Dicas Linux e Windows")](https://2.bp.blogspot.com/-ZDyGxyVDlcw/XVoPh-WD3LI/AAAAAAAAMKA/5qgKuS-Ba0cn2aoGeXr199qQhZDZM72CwCLcBGAs/s1600/05.png)

Se a ferramenta não estiver instalada instale-a:  
  
sudo apt install gnome-tweak-tool  
No MATE a alteração é feita acessando o menu Aparência >> Fontes  
Deixe como está na imagem abaixo, variando o tamanho da fonte de acordo com seu gosto.  
  

[![Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu  - Dicas Linux e Windows](https://2.bp.blogspot.com/-N_R8qon2IHY/XVjlwWcVCWI/AAAAAAAAMJo/k0H3_zISNyQv8BijjGGw78mMHe1ARi8IACLcBGAs/s640/03.png "Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu  - Dicas Linux e Windows")](https://2.bp.blogspot.com/-N_R8qon2IHY/XVjlwWcVCWI/AAAAAAAAMJo/k0H3_zISNyQv8BijjGGw78mMHe1ARi8IACLcBGAs/s1600/03.png)

  
Como podemos ver nas imagens acima a fonte das janelas, menus, nomes dos aplicativos e da área de trabalho já estão no padrão Ubuntu. Compare:

  
Debian MATE  

[![Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu  - Dicas Linux e Windows](https://1.bp.blogspot.com/-bY6AuceQwnQ/XVjluKfK5lI/AAAAAAAAMJk/lygI1Rbfl7UuQ86Z24uoaKlOwg7h8dhKwCLcBGAs/s640/02.png "Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu  - Dicas Linux e Windows")](https://1.bp.blogspot.com/-bY6AuceQwnQ/XVjluKfK5lI/AAAAAAAAMJk/lygI1Rbfl7UuQ86Z24uoaKlOwg7h8dhKwCLcBGAs/s1600/02.png)

  
Ubuntu MATE  

[![Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu  - Dicas Linux e Windows](https://1.bp.blogspot.com/-IbntIqvl2n4/XVrHGBP40rI/AAAAAAAAMKg/bOAj4aiwq5k7xy8pIgIb24ufwbchdUwIwCLcBGAs/s640/004.png "Gosta das fontes do Ubuntu? Veja como instalar em seu sistema Linux e deixá-lo com a mesma aparência do Ubuntu  - Dicas Linux e Windows")](https://1.bp.blogspot.com/-IbntIqvl2n4/XVrHGBP40rI/AAAAAAAAMKg/bOAj4aiwq5k7xy8pIgIb24ufwbchdUwIwCLcBGAs/s1600/004.png)

  
Obs: Caso tenha interesse em utilizar o tema do Ubuntu (cores, imagens...), instale o tema  [Ambiance](https://www.dropbox.com/s/6qvzt7ufz7somr1/ubuntu-theme.tar.gz?dl=1) para Gnome ou [Ambiant-MATE](https://www.dropbox.com/s/q056kwyr3a5soln/ambiant-mate-orange.tar.gz?dl=1) para o MATE.