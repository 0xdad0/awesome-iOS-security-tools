# awesome iOS security tools [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> Lista de todas las herramientas interesantes de iOS para fines de seguridad

### Herramientas Útiles

- [itms-services](https://www.npmjs.com/package/itms-services) Obtención del archivo IPA desde un enlace de distribución OTA

   ```shell
   npm install -g itms-services
   itms-services -u "itms-services://?action=download-manifest&url=https://s3-ap-southeast-1.amazonaws.com/test-uat/manifest.plist" -o - > out.ipa
   ```

- [ipainstaller](https://github.com/autopear/ipainstaller). El IPA también puede instalarse directamente en el dispositivo iOS a través de la línea de comandos con ipainstaller

- [Keychain-Dumper](https://github.com/ptoomey3/Keychain-Dumper)

- [frida-ios-dump](https://github.com/AloneMonkey/frida-ios-dump) Extrae un IPA descifrado desde un dispositivo con jailbreak

- [checkra1n](https://github.com/checkra1n)

- [unc0ver.dev](https://unc0ver.dev/)

- [idb](https://github.com/dmayer/idb)

- [idb-facebook](https://github.com/facebook/idb/). Herramienta para reemplazar WebDriverAgent.

- [WebDriverAgent](https://github.com/facebookarchive/WebDriverAgent). Archivo.

- [imobax](https://github.com/Siguza/imobax). El Extractor de Copias de Seguridad Móviles de iOS.

- [Clutch](https://github.com/KJCracks/Clutch). Clutch es una herramienta de descifrado de iOS de alta velocidad. Clutch es compatible con iPhone, iPod Touch e iPad, así como con todas las versiones de iOS, tipos de arquitectura y la mayoría de los binarios. Clutch está destinado únicamente a fines educativos e investigación de seguridad.

- [ish](https://github.com/ish-app/ish). Un proyecto para ejecutar un shell de Linux en iOS, utilizando emulación x86 en modo usuario y traducción de llamadas al sistema (syscall).

- [plistutil](https://manpages.debian.org/experimental/libplist-utils/plistutil.1.en.html)

   ```shell
   apt install libplist-utils
   plistutil -i Info.plist -o Info_xml.plist
   ```

- [ipatool](https://github.com/majd/ipatool)

- [bagbak](https://github.com/ChiChou/bagbak). Otra herramienta de dumpdescrypted para iOS basada en frida. También descifra extensiones de aplicaciones.


### [libimobiledevice](https://libimobiledevice.org/)

- Requisitos

   ```shell
   sudo apt-get install \
   build-essential \
   checkinstall \
   git \
   autoconf \
   automake \
   libtool-bin \
      libzip-dev \
      libxml2-dev \
   libcurl4-openssl-dev \
      zlib1g-dev \
      libfuse-dev \
   libreadline-dev \
   libusb-1.0-0-dev \
   ```

   ```shell
   sudo apt-get install \
   doxygen \
   cython
   ```

- Todos los módulos se instalan con los siguientes comandos (en el siguiente orden)

   ```shell
   ./autogen.sh
   make
   sudo make install
   sudo ldconfig 
   ```

- [ipsw](https://github.com/blacktop/ipsw). Navaja suiza de investigación para iOS/macOS

- [usbmuxd](https://github.com/libimobiledevice/usbmuxd) Un demonio de socket para multiplexar conexiones desde y hacia dispositivos iOS.

- [libplist](https://github.com/libimobiledevice/libplist) Una pequeña biblioteca C portable para manejar archivos Apple Property List en formato binario o XML.

- [libusbmuxd](https://github.com/libimobiledevice/libusbmuxd) Una biblioteca cliente para que las aplicaciones manejen conexiones del protocolo usbmux con dispositivos iOS.

- [libimobiledevice](https://github.com/libimobiledevice/libimobiledevice) Una biblioteca para comunicarse con servicios en dispositivos iOS utilizando protocolos nativos.

- [ideviceinstaller](https://github.com/libimobiledevice/ideviceinstaller) Una aplicación de línea de comandos para gestionar aplicaciones y archivos de aplicación en dispositivos iOS.

- [libideviceactivation](https://github.com/libimobiledevice/libideviceactivation) Una biblioteca para gestionar el proceso de activación de dispositivos Apple iOS.

- [ifuse](https://github.com/libimobiledevice/ifuse) Una implementación de sistema de archivos fuse para acceder al contenido de los dispositivos iOS.

- [libirecovery](https://github.com/libimobiledevice/libirecovery) La biblioteca libirecovery permite la comunicación con iBoot/iBSS de los dispositivos iOS a través de USB.

- [idevicerestore](https://github.com/libimobiledevice/idevicerestore) Una aplicación de línea de comandos para restaurar archivos de firmware en dispositivos iOS.

- [ios-app-signer](https://github.com/DanTheMan827/ios-app-signer) Esta es una aplicación para OS X que puede (re)firmar aplicaciones y empaquetarlas en archivos ipa listos para ser instalados en un dispositivo iOS.
- [ldid2](https://github.com/xerub/ldid)

### herramientas de nowsecure

- [r2frida](https://github.com/nowsecure/r2frida) Radare2 y Frida funcionan mejor juntos.

- [node-applesign](https://github.com/nowsecure/node-applesign) Módulo de NodeJS y utilidad de línea de comandos para re-firmar aplicaciones iOS (archivos IPA).

- [ipa-extract-info](https://github.com/nowsecure/ipa-extract-info) ¡Extrae el Info.plist de un IPA, en node.js y el navegador!

### ioscontrol

- [ios-deploy](https://github.com/ios-control/ios-deploy) Instala y depura aplicaciones iOS desde la línea de comandos. Diseñado para funcionar en dispositivos sin jailbreak (Requisito - MacOs)


## Análisis Estático

- [Ghidra](https://ghidra-sre.org/)
  - [Ghidra-script](https://github.com/ghidraninja/ghidra_scripts)
- [Cutter](https://cutter.re/)
- [REA](https://github.com/morluto/rea) - CLI y servidor MCP locales para inspeccionar binarios Mach-O, incluida su arquitectura y sus opciones de protección.
- [Radare2](https://rada.re/n/)
- Hooper
- [Mara Framework](https://github.com/xtiankisutsa/MARA_Framework)
- [ipa-extract-info](https://www.npmjs.com/package/ipa-extract-info)
- [DyldExtractor](https://github.com/arandomdev/DyldExtractor)
- [apfs-fuse](https://github.com/sgan81/apfs-fuse)
- [jtool2](https://newosxbook.com/tools/jtool.html)
- [jtool.ELF64](https://github.com/MobSF/Mobile-Security-Framework-MobSF/blob/master/mobsf/StaticAnalyzer/tools/ios/jtool.ELF64)
- [disarm](https://newosxbook.com/tools/disarm.html)

## Análisis Dinámico

- [Fastbot_iOS](https://github.com/bytedance/Fastbot_iOS) Fastbot es una herramienta de pruebas basada en modelos para modelar transiciones de GUI y descubrir problemas de estabilidad de la aplicación. Combina técnicas de aprendizaje automático y aprendizaje por refuerzo para asistir en el descubrimiento de manera más inteligente.

- [introspy-iOS](https://github.com/iSECPartners/Introspy-iOS) Herramienta de caja negra para ayudar a entender qué está haciendo una aplicación iOS en tiempo de ejecución y asistir en la identificación de posibles problemas de seguridad.

- [iOS-Debug-Hacks](https://github.com/aozhimin/iOS-Debug-Hacks)

- [objection](https://github.com/sensepost/objection) objection es un kit de herramientas de exploración móvil en tiempo de ejecución, impulsado por Frida, creado para ayudarte a evaluar la postura de seguridad de tus aplicaciones móviles, sin necesidad de jailbreak.

- [Grapefruit](https://github.com/ChiChou/grapefruit) Grapefruit: Instrumentos de Aplicación en Tiempo de Ejecución para iOS.

- [Frida-Mobile-Scripts](https://github.com/m0bilesecurity/Frida-Mobile-Scripts) Colección de scripts útiles de FRIDA para móviles.

- [frida-ios-hook](https://github.com/noobpk/frida-ios-hook). Un script que te ayuda a rastrear clases, funciones y modificar los valores de retorno de los métodos en la plataforma iOS.

- [iOS-Tagent](https://github.com/AirtestProject/iOS-Tagent). iOS-Tagent es un proyecto basado en WebDriverAgent de facebook y destinado a encajar en el Proyecto Airtest.

- [Frida-Script-Runner](https://github.com/z3n70/Frida-Script-Runner). Frida Script Runner v1.3 es una herramienta versátil basada en web diseñada para propósitos de pruebas de penetración en Android e iOS.

- [rvi_capture](https://github.com/gh2o/rvi_capture). rvictl para Linux y Windows: captura paquetes enviados/recibidos por dispositivos iOS. Una utilidad para crear volcados de captura de paquetes desde dispositivos iOS; útil para depurar la actividad de red a través de Wireshark.

- [iOS Developer Image](https://cgithub.com/haikieu/xcode-developer-disk-image-all-platforms/tree/master/DiskImages/iPhoneOS.platform/DeviceSupport).

- [Fridax](https://github.com/NorthwaveSecurity/fridax). Fridax te permite leer variables e interceptar/enganchar (hook) funciones en aplicaciones iOS/Android compiladas con Xamarin/Mono JIT y AOT.

- [fridump](https://github.com/Nightbringer21/fridump). Un volcado de memoria universal utilizando Frida.

- [frida-ios-hook](https://github.com/noobpk/frida-ios-hook). Una herramienta que te ayuda a rastrear fácilmente clases, funciones y modificar los valores de retorno de los métodos en la plataforma iOS.

- [appmon](https://github.com/dpnishant/appmon). AppMon es un marco automatizado para monitorear y manipular llamadas a la API del sistema de aplicaciones nativas de macOS, iOS y android. Está basado en Frida. [Documentación](https://dpnishant.github.io/appmon/).

- [reFlutter](https://github.com/Impact-I/reFlutter). reFlutter.

### nowsecure

- [fsmon](https://github.com/nowsecure/fsmon) Utilidad de monitoreo del sistema de archivos que se ejecuta en Linux, Android, iOS y OSX.
- [frida-trace](https://github.com/nowsecure/frida-trace) Rastrea APIs declarativamente a través de Frida.
- [frida-cycript](https://github.com/nowsecure/frida-cycript) Esta es una bifurcación de [Cycript] 1 en la que reemplazamos su tiempo de ejecución con uno nuevo llamado [Mjølner] 3 impulsado por [Frida] 4. Esto permite que frida-cycript se ejecute en todas las plataformas y arquitecturas mantenidas por [frida-core] 8.
- [frida-screenshot](https://github.com/nowsecure/frida-screenshot) Captura pantallas utilizando Frida.


### Frameworks

- [RMS-Runtime-Mobile-Security](https://github.com/m0bilesecurity/RMS-Runtime-Mobile-Security)
- [MobSf](https://github.com/MobSF/Mobile-Security-Framework-MobSF)
- [pirogue](https://pts-project.org/). Informática forense de dispositivos móviles e investigación digital.
- [Medusa](https://github.com/Ch0pin/medusa). Marco de instrumentación binaria basado en FRIDA


---

## Jailbreak

- [checkra1n]
- [palera1n]
- [AppSync](https://cydia.akemi.ai/?page/net.angelxwind.appsyncunified). AppSync es un tweak que parchea installd, permitiendo la instalación de paquetes IPA con firmas falsas.
- [Cydia Impactor](http://www.cydiaimpactor.com/). Esta herramienta fue creada originalmente para hacer jailbreak a iPhones, pero ha sido reescrita para firmar e instalar paquetes IPA en dispositivos iOS mediante sideloading.

---

## Recursos y Tutoriales

- [ios-frida-objection-cheat-sheet](https://www.virtuesecurity.com/kb/ios-frida-objection-pentesting-cheat-sheet/)
- [ios-Swift Anti-Jailbreak Bypass with Frida](https://syrion.me/blog/ios-swift-antijailbreak-bypass-frida/)
- [RE-iOS-Apps](https://github.com/ivRodriguezCA/RE-iOS-Apps)
- [iOS-Bypass-Jailbreak](https://philkeeble.com/ios/reverse-engineering/iOS-Bypass-Jailbreak/)
- [Post-on-iOS-RE](https://philkeeble.com/categories/#ios)
- [iOS-Reverse-Engineering](https://github.com/GhidraEnjoyr/iOS-Reverse-Engineering)

---

## Forense de iOS
- [ios_forensics_suite](https://github.com/piotrbania/ios_forensics_suite)

---

## CTF con apps de iOS

- [NCC-CON-2018](https://ch1kpee.com/2018/01/08/ncc-con-2018-ios-ctf-solutions/)
- [awesome-mobile-ctf](https://github.com/xtiankisutsa/awesome-mobile-CTF)
- [ios-ctf](https://www.ivrodriguez.com/mobile-ctf/)
- [Walkthrough of an iOS CTF](https://www.optiv.com/explore-optiv-insights/source-zero/walkthrough-ios-ctf)
- [H1702 CTF](http://redgetan.cc/h1_702-ctf-reversing-ios-android-arm-writeup/)
- [frida-ios-jailbreak-bypass](https://syrion.me/blog/ios-swift-antijailbreak-bypass-frida/)
- [bypass-jailbreak-detection-ios](https://blog.attify.com/bypass-jailbreak-detection-frida-ios-applications/)
