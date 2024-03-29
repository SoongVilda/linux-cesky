# Úvod do hraní na Linuxu
Hraní her na Linuxu je sice podobné jako na Windows, ale existují zde odlišnosti, níže následuje rozpis všech detailů.

# Nástroj pro hraní na Linuxu
Pro hraní her existuje celá řada nástrojů, které jsou nutností nebo aspoň velmi nápomocné.

## Základní nástroje
- [Wine](https://www.winehq.org/) - Původně akronym pro "Wine Is Not an Emulator", což znamená "Wine není emulátor") je kompatibilní vrstva umožňující spouštění aplikací Windows na několika operačních systémech kompatibilních s POSIX, jako jsou Linux, macOS a BSD.
- [Proton](https://github.com/ValveSoftware/Proton) - Nástroj pro použití se Steam klientem, který umožňuje spouštět hry, které jsou exkluzivní pro Windows, na operačním systému Linux. K tomu využívá Wine.
- [DXVK](https://github.com/doitsujin/dxvk) - Překladová vrstva založená na Vulkanu pro Direct3D 9/10/11, která umožňuje spouštění 3D aplikací na Linuxu s využitím Wine.
- [vkd3d-proton](https://github.com/HansKristian-Work/vkd3d-proton) - odnož VKD3D, s cílem implementovat plnou API Direct3D 12 na základě Vulkanu. Tento projekt slouží jako vývojové úsilí pro podporu Direct3D 12 ve Protonu.

## Další nástroje
Tyto nástroje jsou zvláště nápomocné pro zpřístupňění spouštěčů, jako **Ubisoft connect**, **Battle.net**, **GOG Galaxy** a další.  
***Zajímavost:** Steam jako jediný funguje nativně na Linuxu a lze ho najít v repozitářích snad na každé Linux distribuci.*
- [Lutris](https://lutris.net/)
- [Bottles](https://usebottles.com/)
- [Heroic Games Launcher](https://heroicgameslauncher.com/)

## Výhody
---
Výhody hraní her na Linuxu a vysvětlení.

### Kompatibilita
- Zpětná kompatibilita her na nejnovějších Windows 11 se stále zhoršuje, právě kompatibilita je na Linuxu se staršímí hrami značně lepší.
- Chování **Základních nástrojů**, umožňuje překladem zachovat kompatibilitu starším hrám, ale i novějším titlům.

### Výkon a stabilita FPS
- Linux pracuje s komponenty počítače (hardware) efektivněji, méně ho zatěžuje, to zajišťuje vyšší výkon celého počítače, nejen pro hry.
- DXVK a VKD3D umožňují lepší, efektvinější paralelizaci, protože Vulkan je na rozdíl od DirectX psaný pro lepší využití více jader procesoru.
- Vulkan má celou řadu kroků, jak zvyšuje výkon. Například: Pre-cached shaders - přednačtení shaderu, shadery se jen načítají, nespotřebují výkon grafické karty.

### Odlišné ovladače pro hardware
- AMD grafické karty používají na Linuxu značně odlišné ovladače. Obsahují více oprav, optimalizaci, dokonce celé implementace funkcí, které v ovldačích pro Windows nejsou dostupné.

## Nevýhody
---
Nevýhody hraní her na Linuxu a vysvětlení.

### Kompatibilita
Některé hry naopak nejsou kompatibilní s Linuxem, z pravidla ty co čerstvě výjdou.
- **Anti-cheat** - hry s anti-cheatem většinou nefungují, aktuálně funguje velmi málo her.
