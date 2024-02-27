# Základní příkazy
Využití terminálu vyžaduje alespoň základní znalost příkazů.
- **Výhoda:** Naučíte se to jednou a máte vystaráno do konce života. Většina základních příkazů má přes 50 let a jsou stále stejné, protože fungují a není důvod je měnit. Ovšem při vydání nových verzí Windows se znovu a znovu je třeba učit nové věci, protože Microsoft se rozhodl pro změny, ačkoliv to mnohdy nedává smysl.
- **Nevýhoda:** Je potřeba trochu trpělivosti, abyste se naučili něco nového.

## Příkazy
Zde je několik základních příkazů, které jsou užitečné pro každého, kdo začíná s Linuxem:

1. **`ls`** - Zobrazit soubory a složky
   - **Příklad:** `ls` zobrazí seznam souborů a složek ve vašem aktuálním adresáři.
   - **Varianty:** `ls -l` pro zobrazení podrobných informací, `ls -a` pro zobrazení skrytých souborů.

2. **`cd`** - Změnit adresář
   - **Příklad:** `cd Documents` změní aktuální adresář na adresář Documents.
   - **Poznámka:** `cd ..` vás vrátí do nadřazeného adresáře.

3. **`pwd`** - Zobrazit aktuální cestu adresáře
   - **Příklad:** `pwd` zobrazí cestu aktuálního adresáře, ve kterém se nacházíte.

4. **`mkdir`** - Vytvořit nový adresář
   - **Příklad:** `mkdir NovyAdresar` vytvoří nový adresář s názvem NovyAdresar.

5. **`touch`** - Vytvořit nový soubor
   - **Příklad:** `touch soubor.txt` vytvoří nový prázdný soubor s názvem soubor.txt.

6. **`rm`** - Smazat soubory nebo adresáře
   - **Příklad:** `rm soubor.txt` smaže soubor s názvem soubor.txt.
   - **Varování:** `rm -r Adresar` smaže adresář Adresar a vše, co obsahuje!

7. **`cp`** - Kopírovat soubory nebo adresáře
   - **Příklad:** `cp soubor1.txt soubor2.txt` zkopíruje soubor1.txt do soubor2.txt.

8. **`mv`** - Přesunout nebo přejmenovat soubory nebo adresáře
   - **Příklad:** `mv soubor1.txt NovySoubor.txt` přejmenuje soubor1.txt na NovySoubor.txt.

9. **`cat`** - Zobrazit obsah souboru
   - **Příklad:** `cat soubor.txt` zobrazí obsah souboru soubor.txt na obrazovce.

10. **`man`** - Zobrazit manuálovou stránku pro příkazy
    - **Příklad:** `man ls` zobrazí manuálovou stránku pro příkaz ls.

Tato příručka obsahuje základy, které pomohou novým uživatelům Linuxu pochopit a používat základní příkazy. Je vždy dobré zdůraznit, že při práci s příkazy jako `rm`, které mohou mazat soubory, je třeba být opatrný.

## Použití základních příkazů
Typická situace: neznámý počítač, kde je vidět otevřené okno terminálu. Co teď?

### Rozpoznání Linux distribuce
1. **Otázka:** Co to je za Linux? S čím mám tu čest?
2. **Získání odpovědi:** Zadáním příkazu `cat /etc/os-release` do terminálu a stisknutím klávesy enter.
3. **Vyhodnocení odpovědi:** Nejužitečnější části výstupu v terminálu: `NAME="CachyOS Linux"` a `PRETTY_NAME="CachyOS"`.
4. **Odpověď:** Na aktuálním počítači běží Linux distribuce jménem CachyOS.
```
❯ cat /etc/os-release
NAME="CachyOS Linux"
PRETTY_NAME="CachyOS"
ID=cachyos
ID_LIKE=arch
BUILD_ID=rolling
ANSI_COLOR="38;2;23;147;209"
HOME_URL="https://cachyos.org/"
DOCUMENTATION_URL="https://wiki.cachyos.org/"
SUPPORT_URL="https://forum.cachyos.org/"
BUG_REPORT_URL="https://github.com/cachyos"
PRIVACY_POLICY_URL="https://terms.archlinux.org/docs/privacy-policy/"
LOGO=cachyos
```

### Rozpoznání umístění
1. **Otázka:** Co to je za adresář (složku)? Kde to jsem?
2. **Získání odpovědi:** Zadáním příkazu `pwd` do terminálu a stisknutím klávesy enter.
3. **Odpověď:** Terminál je otevřen v umístění `/home/vilda`.
```
❯ pwd
/home/vilda
```

### Obsah adresáře
1. **Otázka:** Co je v adresáři (složce) za data?
2. **Získání odpovědi:** Zadáním příkazu `ls` do terminálu a stisknutím klávesy enter.
3. **Odpověď:** Adresář obsahuje následující soubory:
```
❯ ls
drwxr-xr-x    - vilda 26 úno 23:13  Dokumenty
drwxr-xr-x    - vilda 11 zář  2023  dxvk
drwxr-xr-x    - vilda 24 úno 01:05  Games
drwxr-xr-x    - vilda 19 úno 19:43  go
drwxr-xr-x    - vilda 24 čec  2023  GPU
drwxr-xr-x    - vilda 24 čec  2023  Hudba
drwxr-xr-x    - vilda 30 led 19:25  Obrázky
drwxr-xr-x    - vilda 27 lis  2023  Plocha
drwxr-xr-x    - vilda 25 úno 23:16  Stažené
drwxr-xr-x    - vilda 24 čec  2023  Veřejné
drwxr-xr-x    - vilda 25 led 17:09  Videa
drwxr-xr-x    - vilda 24 čec  2023  Šablony
```
