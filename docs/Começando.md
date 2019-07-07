## **Antes de começar**

Nesta parte iremos te informar o básico sobre termologias mais usadas na cena, o que você irá poder fazer após esse guia e também deixar alguns avisos importantes antes que você prossiga.

!!! important
    Está é uma seção com muitas informações para você agregar, mas se você é um completo noob na cena do Switch, é altamente recomendável que você leia tudo antes de prosseguir.

## **O que é Homebrew?**
Homebrew é um termo usado para descrever um software não autorizado pela Nintendo. Isto inclui custom firmware (CFW), aplicativos, jogos, emuladores e etc.  
  
## **O que é uma Custom Firmware?**
Custom Firmware (CFW) permite que as homebrew tenham mais acesso ao sistema do que os aplicativos "oficiais" de forma geral disponíveis na maioria dos sistemas.

Nesse momento, todos os Nintendo Switches vendidos antes de julho de 2018 podem rodar uma Custom Firmware. Switches fabricados após essa data podem ser desbloqueados somente se eles tirevem na Firmware (FW) 4.1.0. Fique tranquilo que esse guia servirá pra você também que tem um switch nessa condição.

Uma forma fácil de você verificar se seu Nintendo Switch é ou desbloqueável independente da versão do seu Firmware, é só acessar esse [site](https://damota.me/ssnc/checker/ "site") e digitar o "serial number" do seu Switch.

## **O que irei conseguir fazer através desse guia?**
Esse guia irá te dar a habilidade de rodar uma Custom Firmware de escolha em um Nintendo Switch não modificado.

Iremos detalhar de como usar através de duas falhas (com diferentes tipos de implmentação dependendo da firmware em que você está)

### **fusee-gelee**
Essa foi a primeira falha descoberta pelos hackers (também chamada de ShofEL2 ou CVE-2018-6242) que funciona quando o switch esta em um modo chamado "recovery mode (RCM)". Podemos dizer que o fusee-gelee é uma falha "não persistente", que significa que você precisa de um outro dispositivel (por exemplo um PC ou um celular Android) para habilitar a CFW em cada reboot do console.

A falha permite um total constrole do sistema do console, isso se deve por conta da falha rodar antes mesmo do boot normal do switch, significando que tudo do sistema operacional oficial do Switch (chamado de Horizon ou HOS) pode ser alterado.

Caso você tenha interesse em uma leitura mais técnica sobre como essa falha funciona, leia esse [documento](https://www.exploit-db.com/docs/english/44532-nintendo-switchnvidia-vulnerability-disclosure-fus%C3%A9e-gel%C3%A9e.pdf "documento") (em inglês).

### **Deja-vu**
The secondary exploit group is called deja-vu, which takes advantage of an oversight in the Nintendo Switch’s warmboot firmware (the code that runs when you put your Switch to sleep and wake it up). This exploit also allows for a full system takeover, as we can reboot the system into a state with the same posibilities that fusee-gelee provides. Deja-vu is a browser-based, software only exploit. You must launch the exploit through the browser every time you reboot your system into stock firmware.

Deja-vu currently only has implementations available from firmwares 1.0.0 - 3.0.0 and 4.0.1 - 4.1.0, however the exploit theoretically works up to firmware 7.0.1 (the exploit was patched in firmware 8.0.0) and support for these higher firmwares should be added in the future. The current deja-vu implementations are Nereba for firmware 1.0.0, and Caffeine for firmwares 2.0.0-3.0.0 and 4.0.1 - 4.1.0.

### **Custom Firmware**
This guide will focus on using a configuration of the Hekate custom bootloader, as well as the Atmosphere custom firmware, both provided by Team AtlasNX’s Kosmos. You can also install ReiNX along the way if you wish to use that instead, however this guide will assume you are using Hekate and Atmosphere, and will not walk you through using ReiNX.

Atmosphere provides most things you might expect in a custom firmware, including homebrew, cheats, game mods, emuNAND (referred to as emuMMC on Switch), and more.