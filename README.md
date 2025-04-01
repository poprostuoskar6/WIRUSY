## ⚠️ WAŻNE INSTRUKCJE ⚠️

# BEZPIECZNE POBIERANIE Z MEGA
## Z RACJI ŻE TE PLIKI SĄ DOŚĆ SPORE TO MACIE TUTAJ [MEGA](https://mega.nz/folder/MM0zxbaI#ogAK3udFHKs7Wjn5XxFCng)

## WERYFIKACJA BEZPIECZEŃSTWA
Przed pobraniem **ZAWSZE** sprawdź pliki:
🔗 [VIRUSTOTAL LINK](https://www.virustotal.com/gui/url/b342d1db16708f2d3c68b5bfddb23ed48306610e9c56956110a4edaf779d21b0?nocache=1)

## METODA 1: POBIERANIE RĘCZNE (NAJPROSTSZE)
1. Kliknij w link: [MEGA](https://mega.nz/folder/MM0zxbaI#ogAK3udFHKs7Wjn5XxFCng)
2. Wybierz "Download as ZIP"
3. Poczekaj na przygotowanie archiwum
4. Zapisz plik na dysku

## METODA 2: POBIERANIE PRZEZ TERMINAL
### 1. Instalacja narzędzia
```bash
sudo apt update && sudo apt install megatools -y
```

### 2. Komenda do pobrania
```bash
megadl 'https://mega.nz/folder/MM0zxbaI#ogAK3udFHKs7Wjn5XxFCng' --path ./pobrane_dane
```

### Co się stanie?
- Utworzy folder `pobrane_dane` w bieżącej lokalizacji
- Ściągnie wszystkie pliki z Twojego folderu MEGA
- Zachowa strukturę katalogów

## GDZIE SĄ PLIKI?
| Metoda | Lokalizacja plików |
|--------|---------------------|
| Ręczna | Folder "Downloads" |
| Terminal | `./pobrane_dane` w aktualnym katalogu |

## ROZWIĄZYWANIE PROBLEMÓW
### Najczęstsze błędy:
1. **Błąd SSL**:
   ```bash
   sudo apt install --reinstall ca-certificates
   ```
   
2. **Brak uprawnień**:
   ```bash
   sudo adduser $USER fuse
   ```

3. **Nieprawidłowy link**:
   - Sprawdź czy link zawiera: `folder/MM0zxbaI#ogAK3udFHKs7Wjn5XxFCng`
   - Używaj dokładnej składni z cudzysłowiami: `'https://...'`

## BEZPIECZEŃSTWO
- Kali Linux działa jako root - rozważ użycie zwykłego użytkownika
- Zawsze sprawdzaj pliki na VirusTotal przed uruchomieniem
- Pobieraj tylko z zaufanych źródeł
