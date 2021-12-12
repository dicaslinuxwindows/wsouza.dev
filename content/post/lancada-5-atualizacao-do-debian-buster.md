---
title: 'Lançada a 5º atualização do Debian Buster'
date: 2020-08-01T22:51:00.000-03:00
draft: false
url: /2020/08/lancada-5-atualizacao-do-debian-buster.html
tags: 
- Debian
- Linux
- Debian Buster
---

![Lançada a 5º atualização do Debian Buster - Dicas Linux e Windows](https://2.bp.blogspot.com/-csKVfolxpQs/XydCFntY5lI/AAAAAAAAPg8/UmVcIMHKyE8vT0vTEvtw2xVtXkhKOXjZACNcBGAsYHQ/s1600/Buster_10.5.png "Lançada a 5º atualização do Debian Buster - Dicas Linux e Windows")

Foi lançado o 5º upgrade do Debian Buster, chamado de Debian 10.5. Confira aqui quais foram as atualizações disponibilizadas neste upgrade e como atualizar seu Debian Buster.

  
  
  
  
  
  

O sistema de atualizações do Debian consiste em atualizações pontuais, com apenas um ou poucos pacotes, e de tempos em tempos saem atualizações maiores, com um maior número de pacotes atualizados. Estas versões não são consideradas um lançamento, mas sim complementos com melhorias e/ou atualizações de segurança. Entre o lançamento das versões são lançados vários upgrades. No Debian Stretch, por exemplo, foram lançadas 9 pacotes até o lançamento do Debian Buster e mais 4 até o momento, totalizando 13.  
  

### Como atualizar

  
Se você já está utilizando o Debian Buster, para obter este pacote de atualizações, basta atualizar pelo terminal, através do _apt_. A quantidade de pacotes a serem atualizados depende dos seus hábitos de usuário. Por exemplo, se você tem o costume de atualizar o sistema com frequência, provavelmente serão poucos pacotes à atualizar. Caso contrário, serão bastante pacotes.  
  
Insira o comando abaixo para atualizar a lista de pacotes.  
  

 sudo apt update

  
Com o comando abaixo você irá instalar as atualizações disponíveis.  
  

 sudo apt full-upgrade

  
Aguarde o fim da instalação e seu sistema estará atualizado e com todas as correções de segurança.  
  
Se não utiliza o Debian, mas ficou interessado, instale através da imagem ISO de instalação, que já está atualizada para a versão 10.5. Download abaixo:  
  

Debian Buster 10.5 amd64 _(Gnome)_

[ Live](https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-10.5.0-amd64-gnome.iso)

[ Torrent](https://cdimage.debian.org/debian-cd/current-live/amd64/bt-hybrid/debian-live-10.5.0-amd64-gnome.iso.torrent)

[Mais...](https://www.debian.org/distrib/)

  

### Pacotes atualizados

  
Segundo o que foi publicado no anúncio [https://www.debian.org/News/2020/20200801](https://www.debian.org/News/2020/20200801) a lista de pacotes atualizados é a que está mostrada abaixo:  
  
Todas as correções  
```
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  

Package

               

Reason

[appstream-glib](https://packages.debian.org/src:appstream-glib)

              

Fix build failures in 2020 and later

[asunder](https://packages.debian.org/src:asunder)

              

Use gnudb instead of freedb by default

[b43-fwcutter](https://packages.debian.org/src:b43-fwcutter)

              

Ensure removal succeeds under non-English locales; do not fail removal if some files no longer exist; fix missing dependencies on pciutils and ca-certificates

[balsa](https://packages.debian.org/src:balsa)

              

Provide server identity when validating certificates, allowing successful validation when using the glib-networking patch for CVE-2020-13645

[base-files](https://packages.debian.org/src:base-files)

              

Update for the point release

[batik](https://packages.debian.org/src:batik)

              

Fix server-side request forgery via xlink:href attributes \[CVE-2019-17566\]

[borgbackup](https://packages.debian.org/src:borgbackup)

              

Fix index corruption bug leading to data loss

[bundler](https://packages.debian.org/src:bundler)

              

Update required version of ruby-molinillo

[c-icap-modules](https://packages.debian.org/src:c-icap-modules)

              

Add support for ClamAV 0.102

[cacti](https://packages.debian.org/src:cacti)

              

Fix issue where UNIX timestamps after September 13th 2020 were rejected as graph start / end; fix remote code execution \[CVE-2020-7237\], cross-site scripting \[CVE-2020-7106\], CSRF issue \[CVE-2020-13231\]; disabling a user account does not immediately invalidate permissions \[CVE-2020-13230\]

[calamares-settings-debian](https://packages.debian.org/src:calamares-settings-debian)

              

Enable displaymanager module, fixing autologin options; use xdg-user-dir to specify Desktop directory

[clamav](https://packages.debian.org/src:clamav)

              

New upstream release; security fixes \[CVE-2020-3327 CVE-2020-3341 CVE-2020-3350 CVE-2020-3327 CVE-2020-3481\]

[cloud-init](https://packages.debian.org/src:cloud-init)

              

New upstream release

[commons-configuration2](https://packages.debian.org/src:commons-configuration2)

              

Prevent object creation when loading YAML files \[CVE-2020-1953\]

[confget](https://packages.debian.org/src:confget)

              

Fix the Python module's handling of values containing \=

[dbus](https://packages.debian.org/src:dbus)

              

New upstream stable release; prevent a denial of service issue \[CVE-2020-12049\]; prevent use-after-free if two usernames share a uid

[debian-edu-config](https://packages.debian.org/src:debian-edu-config)

              

Fix loss of dynamically allocated IPv4 address

[debian-installer](https://packages.debian.org/src:debian-installer)

              

Update Linux ABI to 4.19.0-10

[debian-installer-netboot-images](https://packages.debian.org/src:debian-installer-netboot-images)

              

Rebuild against proposed-updates

[debian-ports-archive-keyring](https://packages.debian.org/src:debian-ports-archive-keyring)

              

Increase the expiration date of the 2020 key (84C573CD4E1AFD6C) by one year; add Debian Ports Archive Automatic Signing Key (2021); move the 2018 key (ID: 06AED62430CB581C) to the removed keyring

[debian-security-support](https://packages.debian.org/src:debian-security-support)

              

Update support status of several packages

[dpdk](https://packages.debian.org/src:dpdk)

              

New upstream release

[exiv2](https://packages.debian.org/src:exiv2)

              

Adjust overly restrictive security patch \[CVE-2018-10958 and CVE-2018-10999\]; fix denial of service issue \[CVE-2018-16336\]

[fdroidserver](https://packages.debian.org/src:fdroidserver)

              

Fix Litecoin address validation

[file-roller](https://packages.debian.org/src:file-roller)

              

Security fix \[CVE-2020-11736\]

[freerdp2](https://packages.debian.org/src:freerdp2)

              

Fix smartcard logins; security fixes \[CVE-2020-11521 CVE-2020-11522 CVE-2020-11523 CVE-2020-11524 CVE-2020-11525 CVE-2020-11526\]

[fwupd](https://packages.debian.org/src:fwupd)

              

New upstream release; fix possible signature verification issue \[CVE-2020-10759\]; use rotated Debian signing keys

[fwupd-amd64-signed](https://packages.debian.org/src:fwupd-amd64-signed)

              

New upstream release; fix possible signature verification issue \[CVE-2020-10759\]; use rotated Debian signing keys

[fwupd-arm64-signed](https://packages.debian.org/src:fwupd-arm64-signed)

              

New upstream release; fix possible signature verification issue \[CVE-2020-10759\]; use rotated Debian signing keys

[fwupd-armhf-signed](https://packages.debian.org/src:fwupd-armhf-signed)

              

New upstream release; fix possible signature verification issue \[CVE-2020-10759\]; use rotated Debian signing keys

[fwupd-i386-signed](https://packages.debian.org/src:fwupd-i386-signed)

              

New upstream release; fix possible signature verification issue \[CVE-2020-10759\]; use rotated Debian signing keys

[fwupdate](https://packages.debian.org/src:fwupdate)

              

Use rotated Debian signing keys

[fwupdate-amd64-signed](https://packages.debian.org/src:fwupdate-amd64-signed)

              

Use rotated Debian signing keys

[fwupdate-arm64-signed](https://packages.debian.org/src:fwupdate-arm64-signed)

              

Use rotated Debian signing keys

[fwupdate-armhf-signed](https://packages.debian.org/src:fwupdate-armhf-signed)

              

Use rotated Debian signing keys

[fwupdate-i386-signed](https://packages.debian.org/src:fwupdate-i386-signed)

              

Use rotated Debian signing keys

[gist](https://packages.debian.org/src:gist)

              

Avoid deprecated authorization API

[glib-networking](https://packages.debian.org/src:glib-networking)

              

Return bad identity error if identity is unset \[CVE-2020-13645\]; break balsa older than 2.5.6-2+deb10u1 as the fix for CVE-2020-13645 breaks balsa's certificate verification

[gnutls28](https://packages.debian.org/src:gnutls28)

              

Fix TL1.2 resumption errors; fix memory leak; handle zero length session tickets, fixing connection errors on TLS1.2 sessions to some big hosting providers; fix verification error with alternate chains

[intel-microcode](https://packages.debian.org/src:intel-microcode)

              

Downgrade some microcodes to previously issued versions, working around hangs on boot on Skylake-U/Y and Skylake Xeon E3

[jackson-databind](https://packages.debian.org/src:jackson-databind)

              

Fix multiple security issues affecting BeanDeserializerFactory \[CVE-2020-9548 CVE-2020-9547 CVE-2020-9546 CVE-2020-8840 CVE-2020-14195 CVE-2020-14062 CVE-2020-14061 CVE-2020-14060 CVE-2020-11620 CVE-2020-11619 CVE-2020-11113 CVE-2020-11112 CVE-2020-11111 CVE-2020-10969 CVE-2020-10968 CVE-2020-10673 CVE-2020-10672 CVE-2019-20330 CVE-2019-17531 and CVE-2019-17267\]

[jameica](https://packages.debian.org/src:jameica)

              

Add mckoisqldb to classpath, allowing use of SynTAX plugin

[jigdo](https://packages.debian.org/src:jigdo)

              

Fix HTTPS support in jigdo-lite and jigdo-mirror

[ksh](https://packages.debian.org/src:ksh)

              

Fix environment variable restriction issue \[CVE-2019-14868\]

[lemonldap-ng](https://packages.debian.org/src:lemonldap-ng)

              

Fix nginx configuration regression introduced by the fix for CVE-2019-19791

[libapache-mod-jk](https://packages.debian.org/src:libapache-mod-jk)

              

Rename Apache configuration file so it can be automatically enabled and disabled

[libclamunrar](https://packages.debian.org/src:libclamunrar)

              

New upstream stable release; add an unversioned meta-package

[libembperl-perl](https://packages.debian.org/src:libembperl-perl)

              

Handle error pages from Apache >= 2.4.40

[libexif](https://packages.debian.org/src:libexif)

              

Security fixes \[CVE-2020-12767 CVE-2020-0093 CVE-2020-13112 CVE-2020-13113 CVE-2020-13114\]; fix buffer overflow \[CVE-2020-0182\] and integer overflow \[CVE-2020-0198\]

[libinput](https://packages.debian.org/src:libinput)

              

Quirks: add trackpoint integration attribute

[libntlm](https://packages.debian.org/src:libntlm)

              

Fix buffer overflow \[CVE-2019-17455\]

[libpam-radius-auth](https://packages.debian.org/src:libpam-radius-auth)

              

Fix buffer overflow in password field \[CVE-2015-9542\]

[libunwind](https://packages.debian.org/src:libunwind)

              

Fix segfaults on mips; manually enable C++ exception support only on i386 and amd64

[libyang](https://packages.debian.org/src:libyang)

              

Fix cache corruption crash, CVE-2019-19333, CVE-2019-19334

[linux](https://packages.debian.org/src:linux)

              

New upstream stable release

[linux-latest](https://packages.debian.org/src:linux-latest)

              

Update for 4.19.0-10 kernel ABI

[linux-signed-amd64](https://packages.debian.org/src:linux-signed-amd64)

              

New upstream stable release

[linux-signed-arm64](https://packages.debian.org/src:linux-signed-arm64)

              

New upstream stable release

[linux-signed-i386](https://packages.debian.org/src:linux-signed-i386)

              

New upstream stable release

[lirc](https://packages.debian.org/src:lirc)

              

Fix conffile management

[mailutils](https://packages.debian.org/src:mailutils)

              

maidag: drop setuid privileges for all delivery operations but mda \[CVE-2019-18862\]

[mariadb-10.3](https://packages.debian.org/src:mariadb-10.3)

              

New upstream stable release; security fixes \[CVE-2020-2752 CVE-2020-2760 CVE-2020-2812 CVE-2020-2814 CVE-2020-13249\]; fix regression in RocksDB ZSTD detection

[mod-gnutls](https://packages.debian.org/src:mod-gnutls)

              

Fix a possible segfault on failed TLS handshake; fix test failures

[multipath-tools](https://packages.debian.org/src:multipath-tools)

              

kpartx: use correct path to partx in udev rule

[mutt](https://packages.debian.org/src:mutt)

              

Don't check IMAP PREAUTH encryption if $tunnel is in use

[mydumper](https://packages.debian.org/src:mydumper)

              

Link against libm

[nfs-utils](https://packages.debian.org/src:nfs-utils)

              

statd: take user-id from /var/lib/nfs/sm \[CVE-2019-3689\]; don't make /var/lib/nfs owned by statd

[nginx](https://packages.debian.org/src:nginx)

              

Fix error page request smuggling vulnerability \[CVE-2019-20372\]

[nmap](https://packages.debian.org/src:nmap)

              

Update default key size to 2048 bits

[node-dot-prop](https://packages.debian.org/src:node-dot-prop)

              

Fix regression introduced in CVE-2020-8116 fix

[node-handlebars](https://packages.debian.org/src:node-handlebars)

              

Disallow calling helperMissing and blockHelperMissing directly \[CVE-2019-19919\]

[node-minimist](https://packages.debian.org/src:node-minimist)

              

Fix prototype pollution \[CVE-2020-7598\]

[nvidia-graphics-drivers](https://packages.debian.org/src:nvidia-graphics-drivers)

              

New upstream stable release; security fixes \[CVE-2020-5963 CVE-2020-5967\]

[nvidia-graphics-drivers-legacy-390xx](https://packages.debian.org/src:nvidia-graphics-drivers-legacy-390xx)

              

New upstream stable release; security fixes \[CVE-2020-5963 CVE-2020-5967\]

[openstack-debian-images](https://packages.debian.org/src:openstack-debian-images)

              

Install resolvconf if installing cloud-init

[pagekite](https://packages.debian.org/src:pagekite)

              

Avoid issues with expiry of shipped SSL certificates by using those from the ca-certificates package

[pdfchain](https://packages.debian.org/src:pdfchain)

              

Fix crash at startup

[perl](https://packages.debian.org/src:perl)

              

Fix multiple regular expression related security issues \[CVE-2020-10543 CVE-2020-10878 CVE-2020-12723\]

[php-horde](https://packages.debian.org/src:php-horde)

              

Fix cross-site scripting vulnerability \[CVE-2020-8035\]

[php-horde-gollem](https://packages.debian.org/src:php-horde-gollem)

              

Fix cross-site scripting vulnerability in breadcrumb output \[CVE-2020-8034\]

[pillow](https://packages.debian.org/src:pillow)

              

Fix multiple out-of-bounds read issues \[CVE-2020-11538 CVE-2020-10378 CVE-2020-10177\]

[policyd-rate-limit](https://packages.debian.org/src:policyd-rate-limit)

              

Fix issues in accounting due to socket reuse

[postfix](https://packages.debian.org/src:postfix)

              

New upstream stable release; fix segfault in the tlsproxy client role when the server role was disabled; fix maillog\_file\_rotate\_suffix default value used the minute instead of the month; fix several TLS related issues; README.Debian fixes

[python-markdown2](https://packages.debian.org/src:python-markdown2)

              

Fix cross-site scripting issue \[CVE-2020-11888\]

[python3.7](https://packages.debian.org/src:python3.7)

              

Avoid infinite loop when reading specially crafted TAR files using the tarfile module \[CVE-2019-20907\]; resolve hash collisions for IPv4Interface and IPv6Interface \[CVE-2020-14422\]; fix denial of service issue in urllib.request.AbstractBasicAuthHandler \[CVE-2020-8492\]

[qdirstat](https://packages.debian.org/src:qdirstat)

              

Fix saving of user-configured MIME categories

[raspi3-firmware](https://packages.debian.org/src:raspi3-firmware)

              

Fix typo that could lead to unbootable systems

[resource-agents](https://packages.debian.org/src:resource-agents)

              

IPsrcaddr: make proto optional to fix regression when used without NetworkManager

[ruby-json](https://packages.debian.org/src:ruby-json)

              

Fix unsafe object creation vulnerability \[CVE-2020-10663\]

[shim](https://packages.debian.org/src:shim)

              

Use rotated Debian signing keys

[shim-helpers-amd64-signed](https://packages.debian.org/src:shim-helpers-amd64-signed)

              

Use rotated Debian signing keys

[shim-helpers-arm64-signed](https://packages.debian.org/src:shim-helpers-arm64-signed)

              

Use rotated Debian signing keys

[shim-helpers-i386-signed](https://packages.debian.org/src:shim-helpers-i386-signed)

              

Use rotated Debian signing keys

[speedtest-cli](https://packages.debian.org/src:speedtest-cli)

              

Pass correct headers to fix upload speed test

[ssvnc](https://packages.debian.org/src:ssvnc)

              

Fix out-of-bounds write \[CVE-2018-20020\], infinite loop \[CVE-2018-20021\], improper initialisation \[CVE-2018-20022\], potential denial-of-service \[CVE-2018-20024\]

[storebackup](https://packages.debian.org/src:storebackup)

              

Fix possible privilege escalation vulnerability \[CVE-2020-7040\]

[suricata](https://packages.debian.org/src:suricata)

              

Fix dropping privileges in nflog runmode

[tigervnc](https://packages.debian.org/src:tigervnc)

              

Don't use libunwind on armel, armhf or arm64

[transmission](https://packages.debian.org/src:transmission)

              

Fix possible denial of service issue \[CVE-2018-10756\]

[wav2cdr](https://packages.debian.org/src:wav2cdr)

              

Use C99 fixed-size integer types to fix runtime assertion on 64bit architectures other than amd64 and alpha

[zipios++](https://packages.debian.org/src:zipios++)

              

Security fix \[CVE-2019-13453\]

  

```Atualizações de segurança  
```
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  

Advisory ID

  

Package

[DSA-4626](https://draft.blogger.com/security/2020/dsa-4626)

        

[php7.3](https://packages.debian.org/src:php7.3)

[DSA-4674](https://draft.blogger.com/security/2020/dsa-4674)

        

[roundcube](https://packages.debian.org/src:roundcube)

[DSA-4675](https://draft.blogger.com/security/2020/dsa-4675)

        

[graphicsmagick](https://packages.debian.org/src:graphicsmagick)

[DSA-4676](https://draft.blogger.com/security/2020/dsa-4676)

        

[salt](https://packages.debian.org/src:salt)

[DSA-4677](https://draft.blogger.com/security/2020/dsa-4677)

        

[wordpress](https://packages.debian.org/src:wordpress)

[DSA-4678](https://draft.blogger.com/security/2020/dsa-4678)

        

[firefox-esr](https://packages.debian.org/src:firefox-esr)

[DSA-4679](https://draft.blogger.com/security/2020/dsa-4679)

        

[keystone](https://packages.debian.org/src:keystone)

[DSA-4680](https://draft.blogger.com/security/2020/dsa-4680)

        

[tomcat9](https://packages.debian.org/src:tomcat9)

[DSA-4681](https://draft.blogger.com/security/2020/dsa-4681)

        

[webkit2gtk](https://packages.debian.org/src:webkit2gtk)

[DSA-4682](https://draft.blogger.com/security/2020/dsa-4682)

        

[squid](https://packages.debian.org/src:squid)

[DSA-4683](https://draft.blogger.com/security/2020/dsa-4683)

        

[thunderbird](https://packages.debian.org/src:thunderbird)

[DSA-4684](https://draft.blogger.com/security/2020/dsa-4684)

        

[libreswan](https://packages.debian.org/src:libreswan)

[DSA-4685](https://draft.blogger.com/security/2020/dsa-4685)

        

[apt](https://packages.debian.org/src:apt)

[DSA-4686](https://draft.blogger.com/security/2020/dsa-4686)

        

[apache-log4j1.2](https://packages.debian.org/src:apache-log4j1.2)

[DSA-4687](https://draft.blogger.com/security/2020/dsa-4687)

        

[exim4](https://packages.debian.org/src:exim4)

[DSA-4688](https://draft.blogger.com/security/2020/dsa-4688)

        

[dpdk](https://packages.debian.org/src:dpdk)

[DSA-4689](https://draft.blogger.com/security/2020/dsa-4689)

        

[bind9](https://packages.debian.org/src:bind9)

[DSA-4690](https://draft.blogger.com/security/2020/dsa-4690)

        

[dovecot](https://packages.debian.org/src:dovecot)

[DSA-4691](https://draft.blogger.com/security/2020/dsa-4691)

        

[pdns-recursor](https://packages.debian.org/src:pdns-recursor)

[DSA-4692](https://draft.blogger.com/security/2020/dsa-4692)

        

[netqmail](https://packages.debian.org/src:netqmail)

[DSA-4694](https://draft.blogger.com/security/2020/dsa-4694)

        

[unbound](https://packages.debian.org/src:unbound)

[DSA-4695](https://draft.blogger.com/security/2020/dsa-4695)

        

[firefox-esr](https://packages.debian.org/src:firefox-esr)

[DSA-4696](https://draft.blogger.com/security/2020/dsa-4696)

        

[nodejs](https://packages.debian.org/src:nodejs)

[DSA-4697](https://draft.blogger.com/security/2020/dsa-4697)

        

[gnutls28](https://packages.debian.org/src:gnutls28)

[DSA-4699](https://draft.blogger.com/security/2020/dsa-4699)

        

[linux-signed-amd64](https://packages.debian.org/src:linux-signed-amd64)

[DSA-4699](https://draft.blogger.com/security/2020/dsa-4699)

        

[linux-signed-arm64](https://packages.debian.org/src:linux-signed-arm64)

[DSA-4699](https://draft.blogger.com/security/2020/dsa-4699)

        

[linux-signed-i386](https://packages.debian.org/src:linux-signed-i386)

[DSA-4699](https://draft.blogger.com/security/2020/dsa-4699)

        

[linux](https://packages.debian.org/src:linux)

[DSA-4700](https://draft.blogger.com/security/2020/dsa-4700)

        

[roundcube](https://packages.debian.org/src:roundcube)

[DSA-4701](https://draft.blogger.com/security/2020/dsa-4701)

        

[intel-microcode](https://packages.debian.org/src:intel-microcode)

[DSA-4702](https://draft.blogger.com/security/2020/dsa-4702)

        

[thunderbird](https://packages.debian.org/src:thunderbird)

[DSA-4704](https://draft.blogger.com/security/2020/dsa-4704)

        

[vlc](https://packages.debian.org/src:vlc)

[DSA-4705](https://draft.blogger.com/security/2020/dsa-4705)

        

[python-django](https://packages.debian.org/src:python-django)

[DSA-4707](https://draft.blogger.com/security/2020/dsa-4707)

        

[mutt](https://packages.debian.org/src:mutt)

[DSA-4708](https://draft.blogger.com/security/2020/dsa-4708)

        

[neomutt](https://packages.debian.org/src:neomutt)

[DSA-4709](https://draft.blogger.com/security/2020/dsa-4709)

        

[wordpress](https://packages.debian.org/src:wordpress)

[DSA-4710](https://draft.blogger.com/security/2020/dsa-4710)

        

[trafficserver](https://packages.debian.org/src:trafficserver)

[DSA-4711](https://draft.blogger.com/security/2020/dsa-4711)

        

[coturn](https://packages.debian.org/src:coturn)

[DSA-4712](https://draft.blogger.com/security/2020/dsa-4712)

        

[imagemagick](https://packages.debian.org/src:imagemagick)

[DSA-4713](https://draft.blogger.com/security/2020/dsa-4713)

        

[firefox-esr](https://packages.debian.org/src:firefox-esr)

[DSA-4714](https://draft.blogger.com/security/2020/dsa-4714)

        

[chromium](https://packages.debian.org/src:chromium)

[DSA-4716](https://draft.blogger.com/security/2020/dsa-4716)

        

[docker.io](https://packages.debian.org/src:docker.io)

[DSA-4718](https://draft.blogger.com/security/2020/dsa-4718)

        

[thunderbird](https://packages.debian.org/src:thunderbird)

[DSA-4719](https://draft.blogger.com/security/2020/dsa-4719)

        

[php7.3](https://packages.debian.org/src:php7.3)

[DSA-4720](https://draft.blogger.com/security/2020/dsa-4720)

        

[roundcube](https://packages.debian.org/src:roundcube)

[DSA-4721](https://draft.blogger.com/security/2020/dsa-4721)

        

[ruby2.5](https://packages.debian.org/src:ruby2.5)

[DSA-4722](https://draft.blogger.com/security/2020/dsa-4722)

        

[ffmpeg](https://packages.debian.org/src:ffmpeg)

[DSA-4723](https://draft.blogger.com/security/2020/dsa-4723)

        

[xen](https://packages.debian.org/src:xen)

[DSA-4724](https://draft.blogger.com/security/2020/dsa-4724)

        

[webkit2gtk](https://packages.debian.org/src:webkit2gtk)

[DSA-4725](https://draft.blogger.com/security/2020/dsa-4725)

        

[evolution-data-server](https://packages.debian.org/src:evolution-data-server)

[DSA-4726](https://draft.blogger.com/security/2020/dsa-4726)

        

[nss](https://packages.debian.org/src:nss)

[DSA-4727](https://draft.blogger.com/security/2020/dsa-4727)

        

[tomcat9](https://packages.debian.org/src:tomcat9)

[DSA-4728](https://draft.blogger.com/security/2020/dsa-4728)

        

[qemu](https://packages.debian.org/src:qemu)

[DSA-4729](https://draft.blogger.com/security/2020/dsa-4729)

        

[libopenmpt](https://packages.debian.org/src:libopenmpt)

[DSA-4730](https://draft.blogger.com/security/2020/dsa-4730)

        

[ruby-sanitize](https://packages.debian.org/src:ruby-sanitize)

[DSA-4731](https://draft.blogger.com/security/2020/dsa-4731)

        

[redis](https://packages.debian.org/src:redis)

[DSA-4732](https://draft.blogger.com/security/2020/dsa-4732)

        

[squid](https://packages.debian.org/src:squid)

[DSA-4733](https://draft.blogger.com/security/2020/dsa-4733)

        

[qemu](https://packages.debian.org/src:qemu)

[DSA-4735](https://draft.blogger.com/security/2020/dsa-4735)

        

[grub-efi-amd64-signed](https://packages.debian.org/src:grub-efi-amd64-signed)

[DSA-4735](https://draft.blogger.com/security/2020/dsa-4735)

        

[grub-efi-arm64-signed](https://packages.debian.org/src:grub-efi-arm64-signed)

[DSA-4735](https://draft.blogger.com/security/2020/dsa-4735)

        

[grub-efi-ia32-signed](https://packages.debian.org/src:grub-efi-ia32-signed)

[DSA-4735](https://draft.blogger.com/security/2020/dsa-4735)

        

[grub2](https://packages.debian.org/src:grub2)

  

```Pacotes removidos  
```
  
  
  
  
  
  
  
  

Package

               

Reason

[golang-github-unknwon-cae](https://packages.debian.org/src:golang-github-unknwon-cae)

              

Security issues; unmaintained

[janus](https://packages.debian.org/src:janus)

              

Not supportable in stable

[mathematica-fonts](https://packages.debian.org/src:mathematica-fonts)

              

Relies on unavailable download location

[matrix-synapse](https://packages.debian.org/src:matrix-synapse)

              

Security issues; unsupportable

[selenium-firefoxdriver](https://packages.debian.org/src:selenium-firefoxdriver)

              

Incompatible with newer Firefox ESR versions

  

```