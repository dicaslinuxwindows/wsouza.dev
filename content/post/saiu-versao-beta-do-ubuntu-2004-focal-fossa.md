---
title: 'Saiu a versão Beta do Ubuntu 20.04 Focal Fossa'
date: 2020-04-03T23:50:00.000-03:00
draft: false
url: /2020/04/saiu-versao-beta-do-ubuntu-2004-focal-fossa.html
tags: 
- Linux
- Ubuntu
- Ubuntu 20.04
---

![Saiu a versão Beta do Ubuntu 20.04 Focal Fossa - Dicas Linux e Windows](https://2.bp.blogspot.com/-I-iLyINfwzI/Xuq7gYhfxeI/AAAAAAAAPIE/lzlQtpHwQKcBO1XWyLFVl5YMpSLG1aXBgCNcBGAsYHQ/s1600/Focal_Fossa_Beta.png "Saiu a versão Beta do Ubuntu 20.04 Focal Fossa - Dicas Linux e Windows")

No dia 02/04/2020 saiu a versão beta do Ubuntu 20.04 Focal Fossa. Veja nesta matéria o que falta para a versão final e como obter esta versão.

  
  
  
  
  
  
  

O Ubuntu 20.04, codinome Focal Fossa, é a próxima versão LTS e será lançado oficialmente no dia 23 de abril. Seguindo o cronograma de lançamento _(ver imagem abaixo)_ foi lançada a versão Beta no dia 02 de abril, sendo esta uma das últimas fases antes da versão final.  
  

[![Saiu a versão Beta do Ubuntu 20.04 Focal Fossa - Dicas Linux e Windows](https://3.bp.blogspot.com/-X30A2rfPnrk/XlxDcxSdXMI/AAAAAAAAOGs/eYJEXchznEsf07hUkpdJfG7THCX8ZD67wCNcBGAsYHQ/s1600/Release.png "Saiu a versão Beta do Ubuntu 20.04 Focal Fossa - Dicas Linux e Windows")](https://3.bp.blogspot.com/-X30A2rfPnrk/XlxDcxSdXMI/AAAAAAAAOGs/eYJEXchznEsf07hUkpdJfG7THCX8ZD67wCNcBGAsYHQ/s1600/Release.png)

  

### O que falta para a versão final

  
Do que foi comentado nas _[notícias sobre o Ubuntu 20.04](https://info.wsouza.com.br/2020/03/noticias-sobre-o-ubuntu-20-04-lts.html)_ o Gnome já está na versão 3.36, o Kernel está com a versão 5.4.0-21, tema Yaru e Wallpapers em dia e a Snap Store está presente, assim como a Ubuntu Software.  
Alguns programas já estão em suas últimas versões como o Firefox 74, LibreOffice 6.4. Estas são algumas alterações, porém há outas e conforme se aproxima a data de congelamento, mais alterações e atualizações vão aparecendo.  
O próximo passo imediato é o congelamento do kernel _(Kernel Freeze)_, já no dia 09 de abril. Neste ponto o Kernel deixa de receber atualizações, entrando na fase de testes até o lançamento.  
  

### Como obter a versão beta

  
Existem várias maneiras de obter a versão Beta do Ubuntu 20.04. Uma delas é baixando uma ISO e instalando através de um DVD ou Pendrive, a outra é atualizando a partir de versões anteriores. Abaixo mostrarei como fazer das duas maneiras.  
Porém, se vai instalar esta versão, ou atualizar para a mesma, saiba que podem ocorrer bugs, travamentos e outras coisas estranhas, pois se trata de uma versão inacabada. Se estiver lendo este post após o dia 23 de abril, ao seguir os passos para atualização, você já estará atualizando para a versão final.  
  

#### Instalação limpa

  
Se você não tem nenhuma versão do Ubuntu instalada, ou sua versão é muito antiga, ou não deseja manter os dados existentes no HD você fará o que podemos chamar de instalação limpa. Para fazer este tipo de instalação você vai precisar baixar a imagem ISO da versão beta, disponível no link abaixo.  
  

[ Baixe aqui o Ubuntu 20.04 Focal Fossa Beta](http://cdimage.ubuntu.com/daily-live/current/focal-desktop-amd64.iso)

  
  

#### Atualizando a partir do Ubuntu 18.04 Bionic Beaver

  
O Ubuntu 18.04 é a versão LTS atual, lançada há 2 anos. Como o Focal Fossa será o próximo LTS, é possível atualizar diretamente. Para isto, precisa seguir alguns passos, que serão mostrados na sequência:  

*   Primeiramente vamos verificar se o sistema atual está atualizado, para isto, abra o terminal _(CTRL+Alt+T)_ e digite os comandos:
  

 sudo apt update && sudo apt upgrade

  
*   Após a atualização do sistema atual, vamos aos passos para atualizar a versão. Ainda no terminal, insira o próximo comando.
  

 sudo do-release-upgrade -d

  
*   Este comando verifica se há uma nova versão em desenvolvimento. Após, desativa os repositórios de terceiros _(PPAs)_ e altera os repositórios de _bionic_ para _focal_, tornando possível a busca pela nova versão do sistema.
*   Após iniciada a verificação e busca, aguarde. Após o fim, haverá uma solicitação para confirmar _(ou não)_ a atualização.
*   Caso confirme a atualização esta será iniciada. O tempo vai depender da velocidade da sua internet. Fique atento pois poderão haver solicitações de confirmação de ações, confirme-as e aguarde a finalização. Após finalizado reinicie o sistema e você terá o Ubuntu Focal Fossa instalado.
*   Caso não confirme, será preciso alterar os repositórios manualmente de _focal_ para _bionic_. Para fazer isso, abra o arquivo _sources.list_ com o comando abaixo:
  

 sudo gedit /etc/apt/sources.list

  
*   No arquivo aberto, altere onde houver o nome _focal_ para _bionic_ e salve o arquivo.

  

#### Atualizando a partir do Ubuntu 19.10 Eoan Ermine

  
O Ubuntu 19.10 é uma versão intermediária, lançada em outubro de 2019 e com suporte até julho de 2020. A atualização funciona da mesma forma como foi a anterior, portanto serei sucinto.  

*   Verificando se o sistema está atualizado. Abra o terminal _(CTRL+Alt+T)_ e digite os comandos:
  

 sudo apt update && sudo apt upgrade

  
*   Após, atualize a versão com o comando:
  

 sudo do-release-upgrade -d

  
*   Iniciada a verificação e busca, aguarde a solicitação para confirmar _(ou não)_ a atualização.
*   Confirmando, a atualização esta será iniciada. Aguarde as eventuais solicitações de confirmação de ações, confirme-as e aguarde a finalização. Após finalizado reinicie o sistema e você terá o Ubuntu Focal Fossa instalado.
*   Caso não confirme, será preciso alterar os repositórios manualmente de _focal_ para _eoan_. Abra o arquivo _sources.list_ com o comando abaixo. Altere onde houver o nome _focal_ para _eoan_ e salve o arquivo.
  

 sudo gedit /etc/apt/sources.list

  

  

### Considerações Finais

  
As dicas postadas aqui valem para quem não quer esperar o lançamento da versão final, no dia 23 de abril.  
Vamos aguardar mais notícias e novidades até o dia do lançamento e você que atualizou para a versão Beta, divirta-se.  
  
Fonte: [omgubuntu](https://www.omgubuntu.co.uk/2020/04/how-to-upgrade-to-ubuntu-20-04#upgrade-from-19.10)