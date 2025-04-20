---
title: "Revisitando o Debian-Edu (Skolelinux)"
url: /2025/04/revisitando-o-debian-edu-skolelinux.html
description: ""
date: "2025-04-20T000:02:48-03:00"
thumbnail: "https://info.wsouza.com.br/img/posts/thumbs/thumb-skolelinux.png"
categories:
  - Educacional
tags:
  - Debian-Edu
socialshare: true
draft: false
---
Em **2019**, publiquei <a href="https://info.wsouza.com.br/2019/10/skolelinux-o-debian-educacional.html" target="_blank">um artigo sobre o Skolelinux</a>, destacando sua proposta de facilitar a implementação de ambientes escolares com software livre. Desde então, o projeto evoluiu significativamente, acompanhando os avanços do Debian e incorporando novas funcionalidades para atender às demandas educacionais contemporâneas.
<!--more-->
## O Que é o Debian Edu / Skolelinux?

O **Debian Edu**, também conhecido como **Skolelinux**, é uma distribuição baseada no Debian, projetada para fornecer um ambiente de rede escolar pré-configurado. Após a instalação, um servidor escolar já está pronto para uso com todos os serviços essenciais:

- Autenticação LDAP + Kerberos  
- Servidor de arquivos e diretórios home centralizados  
- Servidor DHCP, proxy web, RADIUS e muito mais  

Além disso, o sistema vem com mais de **70 pacotes de softwares educacionais**, cobrindo desde ferramentas de ensino básico até programação e robótica. O usuário pode escolher entre ambientes como **Xfce, GNOME, LXDE, MATE, KDE Plasma, Cinnamon** e **LXQt**.

---

## O Debian Edu no Debian 11 “Bullseye”: Um Passo Além do que foi mostrado aqui no ano de 2019

Comparando com o cenário apresentado no artigo de 2019 — que tinha como base o Debian 10, codinome Buster — o **Debian Edu 11**, lançado em **2021**, trouxe melhorias marcantes:

- Suporte aprimorado a terminais burros via **X2Go**  
- Substituição do PXELINUX por **iPXE**, compatível com boot gráfico  
- Samba com suporte para **SMB2/SMB3**  
- Ferramentas para configuração de gateways mínimos e RADIUS com EAP-TTLS/PEAP  
- Integração de **DuckDuckGo** como padrão nos navegadores  

O Debian Edu 11.11, lançado em agosto de 2024, encerrou o ciclo do Bullseye com foco em **correções de segurança** e **estabilidade**.

---

## O Presente: Debian Edu com Debian 12 “Bookworm”

O **Debian Edu 12 "Bookworm"** representa um avanço significativo para ambientes educacionais, incorporando melhorias substanciais em instalação, software e documentação.

### 1. Principais Novidades

- **Instalação Aprimorada**: Utiliza o novo instalador do Debian 12, agora com suporte à seção "non-free-firmware", facilitando a instalação em uma gama mais ampla de hardwares. Além disso, apresenta uma nova arte baseada no tema Emerald, padrão do Debian 12.

- **Atualizações de Software**:
  - Kernel Linux 6.1
  - Ambientes de desktop atualizados: KDE Plasma 5.27, GNOME 43, Xfce 4.18, LXDE 11, MATE 1.26
  - LibreOffice 7.4
  - GOsa² 2.8
  - GCompris 3.1 (ferramenta educacional)
  - Rosegarden 22.12 (criação musical)
  - LTSP 23.01 (suporte a terminais leves)
  - Mais de 64.000 pacotes disponíveis para instalação.

- **Documentação e Traduções**:

  - Durante a instalação, a página de escolha de perfil está disponível em 29 idiomas, dos quais 22 estão totalmente traduzidos.
  - O manual do Debian Edu Bookworm foi traduzido para diversos idiomas, incluindo Português do Brasil.

### 2. Status Atual

Embora o desenvolvimento do Debian Edu 12 tenha começado em agosto de 2021, até o momento, a versão oficial ainda não foi lançada. O projeto continua em desenvolvimento ativo, com atualizações frequentes na documentação e nos recursos disponíveis.

### 3. Download

| Arquitetura| CD | DVD-BD |
:------ | :------: | :------: |
 i386 | [ 654 MB](https://get.debian.org/cdimage/release/current/i386/iso-cd/debian-edu-12.10.0-i386-netinst.iso) | [ 7.7 GB](https://get.debian.org/cdimage/release/current/i386/iso-bd/debian-edu-12.10.0-i386-BD-1.iso) | 
 amd64 | [ 640 MB](https://get.debian.org/cdimage/release/current/amd64/iso-cd/debian-edu-12.10.0-amd64-netinst.iso) | [ 7.6 GB](https://get.debian.org/cdimage/release/current/amd64/iso-bd/debian-edu-12.10.0-amd64-BD-1.iso) | 
---

## O Futuro: O Que Esperar do Skolelinux no Debian 13 “Trixie”

Com o **Debian 13 "Trixie"** previsto para **junho de 2025**, a comunidade Debian Edu já começa a se preparar para a próxima geração da distribuição voltada ao ambiente escolar. Embora ainda esteja em fase de desenvolvimento inicial, alguns direcionamentos e expectativas começam a tomar forma com base nas discussões e planos atuais.

### 1. Expectativas e Possíveis Melhorias

- **Suporte a Hardware Mais Recente**: Espera-se compatibilidade com novos dispositivos, como o **Raspberry Pi 5**, Chromebooks e placas ARM modernas, facilitando implantações econômicas em salas de aula.  
- **Atualizações nos Ambientes de Desktop**: KDE Plasma 6, GNOME 46 e atualizações incrementais nos outros ambientes deverão oferecer interfaces mais modernas e responsivas para alunos e professores.  
- **Melhorias no LTSP**: Continuação do suporte e evolução do **LTSP (Linux Terminal Server Project)**, especialmente com foco em rede local de baixa latência e inicialização por PXE/iPXE.  
- **Integração com Plataformas de Ensino Online**: Avanços esperados na integração com ferramentas como **Moodle**, **Nextcloud** e **Jitsi**, refletindo a tendência de ambientes de ensino híbridos.  
- **Administração Centralizada e Interface Web Moderna**: Investimentos contínuos em ferramentas como o **GOsa²**, com melhorias na usabilidade para facilitar a gestão de usuários, grupos e serviços via navegador.  
- **Gamificação e Realidade Aumentada (RA)**: Embora ainda experimentais, existem propostas para integrar softwares voltados à **gamificação da aprendizagem**, RA e laboratórios virtuais.  

---

### 2. Desenvolvimento Comunitário

O desenvolvimento do Debian Edu permanece 100% comunitário, com participação ativa de educadores, desenvolvedores e voluntários do mundo todo. As decisões são tomadas de forma colaborativa, e qualquer contribuição — de documentação a tradução, teste ou código — é bem-vinda.

Você pode acompanhar o andamento do projeto, relatórios de status e planejamento da versão “Trixie” diretamente na wiki oficial: <a href="https://wiki.debian.org/DebianEdu/Status/Trixie" target="_blank">https://wiki.debian.org/DebianEdu/Status/Trixie</a>

## Referências

- <a href="https://info.wsouza.com.br/2019/10/skolelinux-o-debian-educacional.html" target="_blank">Skolelinux, o Debian Educacional (2019)</a>  
- <a href="https://os.watch/skolelinux/11.11" target="_blank">Debian Edu/Skolelinux 11.11 - os.watch</a>  
- <a href="https://www.debian.org/News/2023/20230610.pt.html" target="_blank">Debian -- Anúncio do Debian 12 "Bookworm"</a>  
- <a href="https://www.debian.org/releases/bookworm/" target="_blank">Debian Releases</a>  
- <a href="https://www.debian.org/News/2021/20210815.pt.html" target="_blank">Debian Project - Notícias</a>  
- <a href="https://wiki.debian.org/pt_BR/DebianEdu" target="_blank">https://wiki.debian.org/pt_BR</a>  


