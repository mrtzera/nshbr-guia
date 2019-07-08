Nesta parte iremos te informar o básico sobre termologias mais usadas na cena, o que você irá poder fazer após esse guia e também deixar alguns avisos importantes antes que você prossiga.

!!! important
    Está é uma seção com muitas informações para você agregar, mas se você é um completo noob na cena do Switch, é altamente recomendável que você leia tudo antes de prosseguir.

## **O que é Homebrew?**
Homebrew é um termo usado para descrever um software não autorizado pela Nintendo. Isto inclui aplicativos, jogos, emuladores e etc. Alguns exemplos de softwares que o Switch não suporta oficialmente poderia ser:

- Instalador de .nsp (jogos do Switch)
- Emulador de Nintendo DS
- Leitor de manga/HQ
- Reprodutor de media (video, musica e etc) 
  
## **O que é uma Custom Firmware?**
Custom Firmware (CFW) permite que as homebrew tenham mais acesso ao sistema do que os aplicativos "oficiais" de forma geral disponíveis na maioria dos sistemas, dando espaço para que desenvolvedores projetem softwares que não rodariam nativamente no Nintendo Switch.

!!! info
    Nesse momento, todos os Nintendo Switches vendidos antes de julho de 2018 podem rodar uma Custom Firmware através de uma falha bastante conhecida como **fusee-gelee**. 

!!! info
    Switches fabricados após essa data podem ser desbloqueados somente em determinadas firmwares, através de uma falha conhecida como **Deja-vu**. 

## **O que você irá conseguir fazer através desse guia?**
Esse guia irá te dar a habilidade de rodar uma Custom Firmware grátis em um Nintendo Switch em que a falha de desbloqueio já foi ou não corrigida. Podendo instalar todos os mais variados tipos de homebrews, aumentando absurdamente o leque de possibilidades que você pode fazer com seu querido Nintendo Switch.

## **Que falhas de desbloqueio são essas?**

### **fusee-gelee**
Essa foi a primeira falha descoberta pelos hackers (também chamada de ShofEL2 ou CVE-2018-6242) que funciona quando o switch esta em um modo chamado "recovery mode (RCM)". Podemos dizer que o fusee-gelee é uma falha "não persistente", que significa que você precisa de um outro dispositivel (por exemplo um PC ou um celular Android) para habilitar a CFW em cada reboot do console.

A falha permite um total constrole do sistema do console, isso se deve por conta da falha rodar antes mesmo do boot normal do switch, significando que tudo do sistema operacional oficial do Switch (chamado de Horizon ou HOS) pode ser alterado.

Caso você tenha interesse em uma leitura mais técnica sobre como essa falha funciona, leia esse [documento](https://www.exploit-db.com/docs/english/44532-nintendo-switchnvidia-vulnerability-disclosure-fus%C3%A9e-gel%C3%A9e.pdf "documento") (em inglês).

### **Deja-vu**
Outra falha que foi descoberta é chamada de Deja-vu, a falha se aproveita de uma brecha no warmboot firmware (um tipo de código que roda quando você coloca o switch no modo sleep e depois o reativa). Essa falha também permite um controle total do sistema como no fusee-gelee, Deja-vu é uma falha baseada somente em software, sendo ativada pelo browser do Switch, e deve ser ativada toda vez que você reinicia o console e volta para a firmware original (Horizon).

Possível somente para Switchs com firmware: 1.0.0 / 2.0.0 - 3.0.0 / 4.0.1 - 4.1.0

Especula-se que ela pode ser aplicada até o firmware 7.0.1, e que só foi corrigida no firmware 8.0.0, apesar de nada ter sido confirmado pelos hackers da cena, é possível que no futuro teremos dísponivel também até essa firmware. 

A forma de aplicação dessa falha são chamadas de Nereba para a firmware 1.0.0 e Caffeine para as firmwares 2.0.0 / 3.0.0 / 4.0.1 e 4.1.0.

## **Considerações**
Para os Switchs em que a falha não foi corrigida, iremos ensinar a você desbloquear usando um custom bootloader (um software que faz com que o Switch dê boot em um outro sistema ao invés do Horizon) chamado Hekate. 

Para aqueles que possuim em Switch que já foi corrigida a falha, os chamados "Switches patcheados" ou "Switches não desbloqueáveis", iremos também ter uma sessão nesse guia, em que o meio de desbloqueio é diferente do outro.

A CFW utilizada será o Atmosphere, uma custom firmware totalmente grátis e com funcionalidades muito interessantes.

!!! warning
    É importante saber que aparentemente a Nintendo adotou uma tolerância quase zero em relação a banimento de consoles, é possível sim que você possa ser banido por desbloquear seu Switch, alguns homebrews, acessso a internet pelo CFW, jogos em formato .nsp são alguns fatores que podem levar ao banimento mais fácilmente. Alguns métodos e dicas serão abordados nesse guia para que você possa diminuir essa chance.

!!! danger
    Existe também mesmo que remota, uma chance de seu console brickar (parar de funcionar totalmente), as chances são mínimas, mas mesmo assim iremos ensinar a fazer o importantíssimo  backup da NAND (todo o software do seu switch, sistema operacional, informações salvas, save de games e etc) para que você possa recuperá-lo caso você dê um azar desse.

!!! warning
    Outra coisa que você deve ficar atento é nas homebrews que você instala no seu Switch, como todo sistema possúi algum tipo de vírus, no Switch também não seria diferente, colocando uma homebrew ou até mesmo um jogo (.nsp ou .xci) de uma fonte não confíavel, é possível que ele posso conter um código de brick do seu console