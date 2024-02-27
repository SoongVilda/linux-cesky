# Instalace a odinstalace programů
Podobně jako na mobilu s Androidem nebo iOS, terminologie je jiná, ale princip je stejný.

## Klíčové aspekty
- Programy a aplikace (software) mají centrální zdroj - repozitáře, pomyslný *Obchod s aplikacemi*.
- Většinou se nic nestahuje z webových stránek. To je běžné hlavně u Windows.

## Správce balíčků
Správce balíčků v Linuxu instaluje programy jako balíky - bloky, které lze přidávat a odebírat.

Na Androidu a iOSu správce balíčků uživatel nevidí, ale pod kapotou **Google Play** a **App Store** fungují podobně. 

## Co je balík?
Balík je zabalený program (software), který potřebuje další balíky, tzv. závislosti. Balíky a závislosti se ukládají v repozitáři - *Obchodě s aplikacemi*.

### Co je závislost?
Závislost je balík poskytující dalším balíkům nutnou funkci, bez které nemohou fungovat.  
***Poznámka:** O závislosti se uživatel zpravidla nemusí starat. To dělá správce balíčků.*

### Vizuální ukázka
```
balík
    | 
    --balík 1 (závislost 1)
    --balík 2 (závislost 2)
    --balík 3 (závislost 3)
    --balík 4 (závislost 4)
```

## Základy Správce baličků
Linux distribuce používají různé správce balíčků, ale každý dělá to stejné, některé to dělají jinak, umí více nebo méně. O rozdílech až později.

## Instalace balíčků (programů)
Řekněme, že chceme nainstalovat gimp. Princip je stejný, ale konrkétní provedení bude různé dle Linux distribuce. Níže je uvedený seznam nejvíc používaných příkazů dle linux distribucí a správců balíčků.

***Tip:** Místo `gimp` lze napsat jakýkoliv jiný balík dostupný v repozitářích.*

***Poznámka:** Některé příkazy obsahují `sudo`, to umožní spustit příkaz s právy root uživatele **(admid práva ve Windows)**, bez nich není dovoleno provádět v systému změny.*

### Debian, Ubuntu, Pop!_OS, Kubuntu
---
#### Nainstaluje GIMP
```
sudo apt install gimp
```

#### Odinstaluje GIMP
```
sudo apt remove gimp
```

#### Odinstaluje GIMP a nepotřebné závislosti. 
```
sudo apt autoremove gimp
```
***Tip:** Odinstalace nepotřebných závislosti je optimální, protože nezůstane v systému nepotřebný nepořádek. To je častý problém Windows.*

#### Vyhledat balík
```
apt search gimp
```
***Tip:** Vyhledat dle `gimp` v repozitáři, najde i balíky souvesjící s `gimp`, nejen `gimp` samotný.*

### Fedora
---
#### Nainstaluje GIMP
```
sudo dnf install gimp
```

#### Odinstaluje GIMP
```
sudo dnf remove gimp
```

#### Vyhledat balík
```
dnf search gimp
```
***Tip:** Vyhledat dle `gimp` v repozitáři, najde i balíky souvesjící s `gimp`, nejen `gimp` samotný.*

### ArchLinux, CachyOS, Manjaro, Garuda atd.
---
#### Nainstaluje GIMP
```
sudo pacman -S gimp
```

#### Odinstaluje GIMP
```
sudo pacman -R gimp
```

#### Odinstaluje GIMP a nepotřebné závislosti.
```
sudo pacman -Rs gimp
```
***Tip:** Odinstalace nepotřebných závislosti je optimální, protože nezůstane v systému nepotřebný nepořádek. To je častý problém Windows.*

#### Vyhledat balík
```
pacman -Ss gimp
```
***Tip:** Vyhledat dle `gimp` v repozitáři, najde i balíky souvesjící s `gimp`, nejen `gimp` samotný.*

### OpenSUSE
---
#### Nainstaluje GIMP
```
sudo zypper install gimp
```

#### Odinstaluje GIMP
```
sudo zypper remove gimp
```

#### Odinstaluje GIMP a nepotřebné závislosti.
```
sudo zypper remove --clean-deps gimp
```
***Tip:** Odinstalace nepotřebných závislosti je optimální, protože nezůstane v systému nepotřebný nepořádek. To je častý problém Windows.*

#### Vyhledat balík
```
zypper search gimp
```
***Tip:** Vyhledat dle `gimp` v repozitáři, najde i balíky souvesjící s `gimp`, nejen `gimp` samotný.*
