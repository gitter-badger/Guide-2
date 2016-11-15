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

+ **Antes de comenzar esta guia, usted debe saber que esta bajo su propio riezgo hackear el 3DS: SIEMPRE que se modifique tu sistema, hay un potencial de que llegue a un brick IRRECUPERABLE. Estas son raras, pero siempre existe la posiblidad, por eso trata de seguir siempre TODOS LOS PASOS EXACTAMENTE COMO EN LA GUIA**
+ Si usted tiene su 3DS hackeado con una configuracion de EmuNand, y usted desea mover todo su contenido de su Emunand hacia su nuevo SysNand CFW, usted debe seguir todas las instrucciones y recuperar su EmuNand cuando se le solicite que llegue a [Instalando arm9loaderhax](installing-arm9loaderhax).
+ Esta guia funcionara en New 3DS, Old 3DS, y en 2DS en todas las regiones con firmware 11.2.0 o menor *(exceptuando CHN / TWN en New 3DS y Old 3DS, y KOR New 3DS)*.
+ Si todo sigue acorde al plan, usted no perdera ningun dato y al final terminaras con todo con lo que comenzaste la guia (Juegos, NNID, guardados de partidas, etc seran preservados).
+ Una gran parte de esta guia tiene grandes dumpeos de NAND y downgrades, por esto el proceso puede tomar *muchisimas horas* gracias a el lento procesador de la 3DS.
+ **¡Mantenga siempre conectado y cargando durante todo el proceso para evitar la perdida de datos por algun posible apagado!**
+ Su tarjeta SD debe ser [MBR, no GPT](http://www.howtogeek.com/245610/) (La tarjeta SD que viene con el dispositivo viene como MRB por defecto).
+ Si necesita fomatear alguna nueva tarjeta SD, puede usar [`guiformat`](http://www.ridgecrop.demon.co.uk/index.htm?guiformat.htm) y configurar el tamaño de la unidad asignada a 32K.
+ La 2DS es esencialmente identica a la Old 3DS en terminos de software, por eso cada paso que diga "OLD 3DS" tambien aplica para la 2DS.
