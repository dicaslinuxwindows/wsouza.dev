---
title: 'Como resolver o erro ao instalar extensões no Firefox'
date: 2019-05-07T23:30:00.000-03:00
draft: false
url: /2019/05/como-resolver-o-erro-ao-instalar-extensoes-no-firefox.html
tags: 
- Dicas
- Firefox
---

Nos últimos dias o Firefox não permitiu a instalação de nenhuma extensão. O problema já foi resolvido com uma atualização lançada, mas, se você ainda está com este problema, veja a solução a seguir.

  
  

[![Como resolver o erro ao instalar extensões no Firefox - Dicas Linux e Windows](https://4.bp.blogspot.com/-RM_lw4-pxgU/XNSv8VOSPfI/AAAAAAAALNE/5RKXjF5HgRUDXl07_jSECJUZShroRfT8QCLcBGAs/s1600/firefox.png "Como resolver o erro ao instalar extensões no Firefox - Dicas Linux e Windows")](https://4.bp.blogspot.com/-RM_lw4-pxgU/XNSv8VOSPfI/AAAAAAAALNE/5RKXjF5HgRUDXl07_jSECJUZShroRfT8QCLcBGAs/s1600/firefox.png)

  

### Firefox e Firefox ESR

O Firefox é um navegador web multi-plataforma desenvolvido pela fundação Mozilla e por colaboradores. A versão padrão, chamada apenas de Firefox _(ou Firefox Quantum)_ atualmente está na casa das versões 66 e é a versão disponível no repositório do Ubuntu. Já a versão chamada Firefox ESR é uma versão de suporte estendido, ainda possui alguns recursos - _como o leitor de RSS_ \- que já não está mais disponível no Firefox padrão. É a versão que está disponível no repositório do Debian e está na casa da versão 60.

  

### Extensões desativadas

Após a atualização para a versão 66.0.4 do Firefox e 60.6.2 do Firefox-ESR, todas as extensões foram desativadas e não estava sendo permitida nenhuma outra instalação de extensões. O problema ocorreu devido ao vencimento e a não renovação dos certificados de segurança.

  

### Resolvendo o problema

 Para resolver o problema foram disponibilizadas novas versões dos navegadores, a 60.6.3 do ESR e a  66.0.5 do padrão. Abra o terminal _(CTRL + ALT + T)_ e insira os comando abaixo:

  

**sudo su**

**apt update**

**No Debian**

**No Ubuntu**

**apt install firefox-esr**

**apt install firefox**

Pronto, o Firefox estará atualizado e com extensões funcionando de maneira correta novamente.  
  

### Como garantir sempre a versão mais recente?

Se por qualquer motivo você não conseguir atualizar, ou se deseja receber sempre a versão mais recente direto da Mozilla, volte ao terminal e siga os passos abaixo:

  

**sudo su**

Primeiramente desinstale a versão que veio instalada na sua distribuição.  
  

**No Debian**

**No Ubuntu**

**apt remove firefox-esr**

**apt remove firefox**

Agora, faça o download da última versão, de acordo com a sua preferência. Salve em sua pasta home. Como exemplo vou utilizar a instalação do Firefox-ESR, mas é o mesmo princípio com o Firefox Padrão, o que altera é apenas o nome do arquivo baixado.  
  
**Firefox ESR**  
  

**wget https://download.mozilla.org/?product=firefox-esr-latest-ssl&os=linux64&lang=pt-BR**

Mova a pasta de sua pasta home para a pasta /opt.  
  

**mv firefox-60.6.3esr.tar.bz2 /opt**

Acesse a pasta Opt e descompacte o arquivo.  
  

**cd /opt**

**tar -jxvf firefox-60.6.3esr.tar.bz2**

Para permitir a atualização automática para as novas versões dê permissão ao seu usuário na pasta /opt/firefox. Desta maneira, quando logado com seu usuário, a atualização ocorrerá de forma automática, da mesma forma que acontece no Firefox do Windows.  
  

**chown -R nomedousuario.nomedogrupo firefox**

Como o arquivo gerado anteriormente não será mais necessário, exclua-o.  
  

**rm -rf firefox-60.6.3esr.tar.bz2**

Para criar o atalho no menu:  
  

**sudo \*nome\*do\*editor\* /usr/share/applications/Firefox.desktop**

O editor pode ser qualquer um, tanto em modo texto, quanto em modo gráfico. Ex: _nano vi joe gedit kedit pluma_. Copie os dados abaixo, cole no arquivo aberto e salve.  
  
\[Desktop Entry\] Name=Firefox ESR Exec=/opt/firefox/firefox %u Icon=/opt/firefox/browser/chrome/icons/default/default48.png Type=Application Categories=Network;