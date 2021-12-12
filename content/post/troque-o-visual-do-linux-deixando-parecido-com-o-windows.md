---
title: 'Troque o visual do Linux deixando-o parecido com o Windows'
date: 2016-12-30T01:23:00.000-02:00
draft: false
url: /2016/12/troque-o-visual-do-linux-deixando-parecido-com-o-windows.html
tags: 
- Linux
- Tutoriais
---

Esta dica é uma ótima maneira de introduzir usuários Windows ao universo Linux, sem causar estranheza aos mesmos.  
Mas como? A resposta é bem simples, veja na sequência:  
  
Muita gente que está acostumada com o Windows mal conhecem detalhes do mesmo, pois utilizam apenas o navegador para acessar a internet, logo, não sentirão diferença pois o seu sistema Linux ficará com a mesma aparência do Windows 7 ou 8.  
Faremos a transformação em 3 passos apenas instalando um tema do Windows e alterando este mesmo tema para o padrão do sistema. Veja como é simples:

  

1º Passo: Baixe o tema no link abaixo:  
  
[Tema Windows 7/Windows 8](https://www.dropbox.com/s/5heavk0lzj21b9s/temawindows.tar.gz?dl=0)  
  
Descompacte na sua pasta /home e você verá 3 pastas: Win7, Win8 e windows.  
  
2º Passo: Instale o tema. Para isto abra o terminal e, como super usuário mova as pastas Win7 e Win8 para a pasta /usr/share/themes/  
  
sudo mv Win7 /usr/share/themes  
sudo mv Win8 /usr/share/themes  
  
A pasta Windows deve ser movida da mesma forma, mas para a pasta /usr/share/icons  
  
sudo mv windows /usr/share/icons  
  
3º Passo: Troque o tema pelo tema do Windows.  
  
Instale o Gnome-Tweak-Tool, necessário para trocar o tema. _(A dica foi elaborada utilizando o Gnome)_.  
  
sudo apt-get install gnome-tweak-tool  
  
Abra o Gnome-Tweak-Tool. Você o encontrará  no menu Sistema>>Preferências>>Configurações avançadas, que abrirá a tela abaixo:  
  

[![http://info.wsouza.com.br](https://3.bp.blogspot.com/-Z1xRHArdsZQ/WGXN94EslnI/AAAAAAAACF8/ZZ5pQssi_18SPgeDaBJTW0U5oTovZuDHwCLcB/s400/Captura%2Bde%2Btela%2Bde%2B2016-12-29%2B19_22_36.png "http://info.wsouza.com.br")](https://3.bp.blogspot.com/-Z1xRHArdsZQ/WGXN94EslnI/AAAAAAAACF8/ZZ5pQssi_18SPgeDaBJTW0U5oTovZuDHwCLcB/s1600/Captura%2Bde%2Btela%2Bde%2B2016-12-29%2B19_22_36.png)

  
  
Modifique o tema de janelas, tema de ícones e tema gtk, deixando-os como na imagem acima.

  

Veja alguns exemplos de como ficará seu Desktop.  
  

[![http://info.wsouza.com.br](https://4.bp.blogspot.com/-7E10-x7dAOo/WGXPUGKQ52I/AAAAAAAACGM/nogkg1msLM0bIdVJP8KUNPHLMwrBqQ3yQCLcB/s400/Captura%2Bde%2Btela%2Bde%2B2016-12-29%2B19_23_47.png "http://info.wsouza.com.br")](https://4.bp.blogspot.com/-7E10-x7dAOo/WGXPUGKQ52I/AAAAAAAACGM/nogkg1msLM0bIdVJP8KUNPHLMwrBqQ3yQCLcB/s1600/Captura%2Bde%2Btela%2Bde%2B2016-12-29%2B19_23_47.png)

[![http://info.wsouza.com.br](https://1.bp.blogspot.com/-ItTEsvFajRU/WGXPUAvYQ1I/AAAAAAAACGE/_z8d50YOUEM6GLAyTpAsLEyZu9WYYPrpQCLcB/s400/Captura%2Bde%2Btela%2Bde%2B2016-12-29%2B19_24_55.png "http://info.wsouza.com.br")](https://1.bp.blogspot.com/-ItTEsvFajRU/WGXPUAvYQ1I/AAAAAAAACGE/_z8d50YOUEM6GLAyTpAsLEyZu9WYYPrpQCLcB/s1600/Captura%2Bde%2Btela%2Bde%2B2016-12-29%2B19_24_55.png)

[![http://info.wsouza.com.br](https://3.bp.blogspot.com/-76tvYrfip3Y/WGXPUbJc52I/AAAAAAAACGQ/gpvOlN6Nvh0tztPj-Y6IaPNdFILzOECLACLcB/s400/Captura%2Bde%2Btela%2Bde%2B2016-12-29%2B19_25_55.png "http://info.wsouza.com.br")](https://3.bp.blogspot.com/-76tvYrfip3Y/WGXPUbJc52I/AAAAAAAACGQ/gpvOlN6Nvh0tztPj-Y6IaPNdFILzOECLACLcB/s1600/Captura%2Bde%2Btela%2Bde%2B2016-12-29%2B19_25_55.png)

[![http://info.wsouza.com.br](https://3.bp.blogspot.com/-HC5pmwhrrig/WGXPUYknXlI/AAAAAAAACGU/omXhucKf1LMAxfzhIFk9ZhoyvZHk61kcACLcB/s400/Captura%2Bde%2Btela%2Bde%2B2016-12-29%2B19_26_09.png "http://info.wsouza.com.br")](https://3.bp.blogspot.com/-HC5pmwhrrig/WGXPUYknXlI/AAAAAAAACGU/omXhucKf1LMAxfzhIFk9ZhoyvZHk61kcACLcB/s1600/Captura%2Bde%2Btela%2Bde%2B2016-12-29%2B19_26_09.png)

[![http://info.wsouza.com.br](https://2.bp.blogspot.com/-Z4lLQPUMsys/WGXPUuxfAyI/AAAAAAAACGY/oWSk3e7-QIEKHbbUetR0429Pg1EHqHjTwCLcB/s400/Captura%2Bde%2Btela%2Bde%2B2016-12-29%2B19_27_24.png "http://info.wsouza.com.br")](https://2.bp.blogspot.com/-Z4lLQPUMsys/WGXPUuxfAyI/AAAAAAAACGY/oWSk3e7-QIEKHbbUetR0429Pg1EHqHjTwCLcB/s1600/Captura%2Bde%2Btela%2Bde%2B2016-12-29%2B19_27_24.png)

  
  
Detalhe: o papel de parede padrão do Windows 7 não está neste tema, mas poderá se encontrado facilmente no Google e adicionado como plano de fundo.