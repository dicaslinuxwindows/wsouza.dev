---
title: 'Navegador Microsoft Edge para Linux liberado no canal dev'
date: 2020-10-21T23:57:00.013-03:00
draft: false
url: /2020/10/navegador-microsoft-edge-para-linux.html
tags: 
- Linux
- Microsoft Edge
---

![Navegador Microsoft Edge para Linux liberado no canal dev - Dicas Linux e Windows](https://1.bp.blogspot.com/-MwrS0SBtQP8/X5Dz-Th40WI/AAAAAAAAQio/YFW00BlYD_wPhjeqzB76dvxVG_jPbjI1ACNcBGAsYHQ/s16000/Egde_Dev.png "Navegador Microsoft Edge para Linux liberado no canal dev - Dicas Linux e Windows")

A Microsoft liberou o seu navegador para Linux, o Microsoft Edge, para download no canal de desenvolvedores. Mais detalhes na matéria a seguir.

  
  
  
  
  
  
  

### Microsoft Edge

  
O Microsoft Edge em questão é a segunda geração do navegador da Microsoft, totalmente remodelado e baseado no navegador Chromium, que também é a base para o Google Chrome. A Microsoft vem há um certo tempo anunciando o lançamento de uma versão deste navegador para Linux. Como a dona do Windows tem se aproximado do "mundo" do open source, software livre, do linux, etc... era questão de tempo para que o Edge chegasse ao Linux. O assunto até foi tratado aqui no blog na matéria [Microsoft cada vez mais perto do open source](https://info.wsouza.com.br/2019/05/microsoft-cada-vez-mais-perto-do-open-source.html).  
Também já falamos por aqui algumas vezes sobre o Edge para Linux, como podemos ver nas matérias [Navegador Edge baseado no Chromium será lançado em janeiro de 2020 e terá versão para Linux](https://info.wsouza.com.br/2020/09/microsoft-edge-chegando-no-linux.html) e [Microsoft Edge chegando no Linux](Microsoft%20Edge%20chegando%20no%20Linux).  
Levando em consideração que atualmente o navegador Web é utilizado para uma grande parte do trabalho realizado pelos usuários, a estratégia da Microsoft é bucar um lugar no mercado dos navegadores e abocanhar o espaço conquistado pelo Google Chrome e que, durante muitos anos já foi seu com o navegador Internet Explorer. Esta situação explica o lançamento de um produto para sistemas baseados no Linux, pois sua base de usuários aumentará.  
  

### Edge no Canal DEV e primeiras impressões

  
O lançamento desta semana trata-se de uma versão de testes para que os desenvolvedores adaptem suas ferramnetas, seus sites ao novo navegador. Ela foi disponibilizada no canal destinado aos desenvolvedores _(dev)_. Ainda é uma versão em desenvolvimento e, portanto, algumas funcionalidades não estão disponíveis.  
Dentre algumas das funcionalidades que ainda não estão disponíveis está a integração com a conta microsoft onde é possível sincronizar as configurações, salvar favoritos e senhas para futuras utilizações.  
Não sei se foi só comigo, mas achei que algumas fontes de menus estão desproporcionais. Pode até ser algo referente à configuração do tema que utilizo no meu sistema, porém, comparei com o Chromium e nele e não há este problema.  
Quando se trata de extensões, já é possível instalar extensões da loja da Microsoft e da loja do Google Chrome.  
No quesito desempenho tive boas impressões, sendo rápido ao carregar as páginas e sem travamentos nos sites que utilizo.  
  

### Download

  
O instalador da versão em desenvolvimento foi disponibilizado nos formatos _.deb_ para Debian/Ubuntu e _.rpm_ para Fedora/OpenSuse. Se você é curioso e quer testá-lo antes da versão beta, baixe no site do canal insider dev da microsoft ou diretamente pelos links abaixo.  
  

Microsoft Edge Dev

[ Debian/Ubuntu](https://www.microsoftedgeinsider.com/pt-br/download?platform=linux-deb)

[ Fedora/OpenSuse](https://www.microsoftedgeinsider.com/pt-br/download?platform=linux-rpm)

[Mais...](https://www.microsoftedgeinsider.com/pt-br/download/)

  

### Instalação

  
Supondo que o arquivo foi baixado na pasta /home/downloads, abra a mesma e dê um duplo clique no arquivo **microsoft-edge-dev\_88.0.673.0-1\_amd64.deb** ou **microsoft-edge-dev\_88.0.673.0-1.x86\_64.rpm**. Caso não funcione assim, abra o terminal e digite os comando abaixo.  
  
No Debian ou Ubuntu:  
  

  

 sudo downloads

  

  

 sudo dpkg -i microsoft-edge-dev\_88.0.673.0-1\_amd64.deb

  
Caso dê algum erro de dependências, execute:  
  

  

 sudo apt -f install

  
No Fedora:  
  

  

 sudo downloads

  

  

 sudo dnf install microsoft-edge-dev\_88.0.673.0-1.x86\_64.rpm

  
  
Microsoft Edge rodando no Debian Buster  

[![Navegador Microsoft Edge para Linux liberado no canal dev - Dicas Linux e Windows](https://1.bp.blogspot.com/-wInL1N15l3g/X5DsmxTLfYI/AAAAAAAAQiU/iXUO1OmO7-Iih3s4ElRStENBv5Q_wU5SACNcBGAsYHQ/s600/Captura%2Bde%2Btela%2Bde%2B2020-10-21%2B23-15-25.png "Navegador Microsoft Edge para Linux liberado no canal dev - Dicas Linux e Windows")](https://1.bp.blogspot.com/-wInL1N15l3g/X5DsmxTLfYI/AAAAAAAAQiU/iXUO1OmO7-Iih3s4ElRStENBv5Q_wU5SACNcBGAsYHQ/s1366/Captura%2Bde%2Btela%2Bde%2B2020-10-21%2B23-15-25.png)

  
Microsoft Egde rodando no Fedora 33  

[![Navegador Microsoft Edge para Linux liberado no canal dev - Dicas Linux e Windows](https://1.bp.blogspot.com/-aNNS2L-JKxo/X5Dy-0XMgkI/AAAAAAAAQig/w84jKCmRhzcuEKP65I2yKmOOsazmvm-7ACNcBGAsYHQ/s600/VirtualBox_Fedora%2B33_21_10_2020_23_43_33.png "Navegador Microsoft Edge para Linux liberado no canal dev - Dicas Linux e Windows")](https://1.bp.blogspot.com/-aNNS2L-JKxo/X5Dy-0XMgkI/AAAAAAAAQig/w84jKCmRhzcuEKP65I2yKmOOsazmvm-7ACNcBGAsYHQ/s1366/VirtualBox_Fedora%2B33_21_10_2020_23_43_33.png)

  

### Algumas considerações

  
Por se tratar de uma versão em desenvolvimento, o software ainda estará sujeito à bugs.  
Esta versão é atualizada semanalmente e será atualizada automaticamente.