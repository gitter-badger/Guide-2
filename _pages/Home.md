---
layout: splash
permalink: /
header:
  overlay_color: "#5e616c"
  overlay_image: home-page-feature.jpg
  overlay_filter: 0.5
  cta_label: "EMPEZAR"
  cta_url: "/get-started"
  caption:
excerpt: 'Una guia completa para Custom Firmwares de 3DS, <br /> desde stock a arm9loaderhax.<br />'
---

**Esta guia necesita *tu* ayuda para ser seeder de [estos](https://github.com/Plailect/Guide/archive/master.zip) ([rss](https://plailect.github.io/Guide/rss.xml)) torrents!**
{: .notice--info}

**Para poder usar los archivos [torrent](https://en.wikipedia.org/wiki/Torrent_file) en esta guia, necesitaras un cliente de torrent como: [Transmission](https://sourceforge.net/projects/trqtw/files/latest/download)**
{: .notice--info}

**LEE TODAS LAS INSTRUCCIONES ANTES DE COMENZAR EL PROCESO.**
{: .notice--warning}

## ¿Que es Homebrew?

[**Homebrew**](https://en.wikipedia.org/wiki/List_of_homebrew_video_games) Usualmente se refiere a software que no es autorizado por Nintendo. Esto te permite ejecutar juegos homebrew, herramientas como editores de archivos de guardado, y emuladores de antiguos sistemas.

En la mayoria de los casos, correr homebrew en tu consola es 100% gratuito usando justamente un navegador de internet. Hay varios exploids ("fallos de seguridad") en juegos comerciales para lograr correr homebrew. 

## ¿Que es un Custom Firmware?

**Custom Firmware** ("CFW", en español: "Firmware customizado") te permite usar tecnicas mas avanzadas de hackeo que los homebrew comunes no pueden realizar facilmente. Por ejemplo, parches significativos que te permiten instalar titulos sin firmar que aparecen justo en tu menu HOME.

CFW puede ser configurada facilmente en cualquier consola que este en 9.2.0-20 o menor. Otras versiones pueden ser downgradeadas, la mayoria gratis o con un juego que tenga un exploit. 

## ¿Que es lo que instala esta guia?

Esta guia tiene el objetivo de tomar un 3DS sin modificar con el firmware de fabrica, y ponerle arm9loaderhax optimizado con un Custom Firmware. En otras versiones, se utiliza en homebrew como punto de salto, pero el Custom Firmware sigue siendo el objetivo.

Arm9loaderhax es el nuevo y mejor metodo para ejecutar Custom Firware que te permita un acceso casi total a tu sistema con solo milisegundos de booteo, similar a el efecto del BootMii para la Wii.

Los beneficios de arm9loaderhax sobre otros launchers de CFW son numerosos, y es sumamente recomendado sobre otras guias que utilizan software desactualizados (Como son menuhax o rxTools). 

## ¿Que puedo hacer con un Custom Firmware?

+ Jugar todos los juegos de cartuchos y la eshop, sin importar la region
+ Costumizar tu menu HOME con [temas](https://3dsthem.es/) creados por usuarios y [badges](https://badges.3dsthem.es/)
+ Usar "hack ROMS" para juegos que tengas
+ Tomar gameplays y capturas de pantalla de aplicaciones
+ [Respaldar, editar, y restaurar](https://gbatemp.net/threads/release-jks-savemanager-homebrew-cia-save-manager.413143/) partidas guardadas de muchos juegos
+ Jugar juegos de sistemas antiguos, Usando RetroArch y otros emuladores independientes. (Funcionan mejor en New Nintendo 3DS)
+ Instalar titles de homebrew a tu sistema, y hacer que aparezcan en tu menu HOME
+ Dumpear tus cartuchos de juego a un formato que puedas instalar, y juegalos sin necesidad de cartucho
+ Solo para New 3DS: Haz stream de juegos en vivo a tu PC inalambricamente con NTR CFW
+ Corre muchas flash carts de Nintendo DS que tienen tiempo bloqueadas o que nunca funcionaron en Nintendo 3DS
+ Actualiza con seguridad a la ultima version del sistema sin miedo a perder acceso al homebrew

## ¿Que necesito saber antes de empezar?

+ **Before beginning the guide, you must know the risks of 3DS hacking: EVERY time you modify your system, there is always the potential for an UNRECOVERABLE brick. They're rare, but still a possibility so make sure you follow ALL directions EXACTLY.**
+ If you have already hacked your 3DS before to get an EmuNAND setup, and would like to move the contents of your previous EmuNAND to your new SysNAND CFW, you should follow all instructions and restore your existing EmuNAND when prompted once you reach [Installing arm9loaderhax](installing-arm9loaderhax).
+ This guide will work on New 3DS, Old 3DS, and 2DS in all regions on firmware 11.2.0 or below *(except CHN / TWN on both New 3DS and Old 3DS, and KOR New 3DS)*.
+ If everything goes according to plan, you will lose no data and end up with everything that you started with (games, NNID, saves, etc will be preserved).
+ A large part of this guide is lengthy NAND dumps and downgrades, so the entire process can take *several* hours thanks to the 3DS's slow processor.
+ **Keep the device plugged in and charged throughout the entire process to avoid data loss or damage from an unexpected power-off!**
+ Your SD card should be [MBR, not GPT](http://www.howtogeek.com/245610/) (the SD card that comes with the device will be MBR by default).
+ If you need to format a brand new SD card, you can use [`guiformat`](http://www.ridgecrop.demon.co.uk/index.htm?guiformat.htm) and set to an Allocation Unit Size of 32K.
+ The 2DS is essentially identical to the Old 3DS in terms of software, and that any steps which say "Old 3DS" also apply to 2DS.
