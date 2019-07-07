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

## **O que você irá conseguir fazer através desse guia?**
Esse guia irá te dar a habilidade de rodar uma Custom Firmware de escolha em um Nintendo Switch não modificado.

Iremos detalhar de como usar através de duas falhas (com diferentes tipos de implmentação dependendo da firmware em que você está)

### **fusee-gelee**
Essa foi a primeira falha descoberta pelos hackers (também chamada de ShofEL2 ou CVE-2018-6242) que funciona quando o switch esta em um modo chamado "recovery mode (RCM)". Podemos dizer que o fusee-gelee é uma falha "não persistente", que significa que você precisa de um outro dispositivel (por exemplo um PC ou um celular Android) para habilitar a CFW em cada reboot do console.

A falha permite um total constrole do sistema do console, isso se deve por conta da falha rodar antes mesmo do boot normal do switch, significando que tudo do sistema operacional oficial do Switch (chamado de Horizon ou HOS) pode ser alterado.

Caso você tenha interesse em uma leitura mais técnica sobre como essa falha funciona, leia esse [documento](https://www.exploit-db.com/docs/english/44532-nintendo-switchnvidia-vulnerability-disclosure-fus%C3%A9e-gel%C3%A9e.pdf "documento") (em inglês).

### **Deja-vu**
Outra falha que foi descoberta é chamada de deja-vu, a falha se aproveita de uma brecha no warmboot firmware (um tipo de código que roda quando você coloca o switch no modo sleep e depois o reativa). Essa falha também permite um controle total do sistema como no fusee-gelee, deja-vu é uma falha baseada somente em software, sendo ativada pelo browser do Switch, e deve ser ativada toda vez que você reinicia o console e volta para a firmware original (Horizon).

Infelizmente essa falha está disponível somente para Switches com firmware: 1.0.0 / 3.0.0 / 4.0.1 e 4.1.0, Especula-se que essa falha pode ser aplicada até o firmware 7.0.1, e que só foi corrigida no firmware 8.0.0, é possível que no futuro teremos dísponivel também na 7.0.1. A forma de aplicação dessa falha são chamadas de Nereba para firmware 1.0.0 e Caffeine para as firmwares 2.0.0 / 3.0.0 / 4.0.1 e 4.1.0.

### **Considerações**
Nesse guia iremos ensinar a você desbloquiar usando um custom bootloader (um software que faz com que o Switch dê boot em um outro sistema ao invés do Horizon) chamado Hekate. 

A CFW utilizada será o Atmosphere, uma custom firmware totalmente grátis e com funcionalidades muito interessantes.
