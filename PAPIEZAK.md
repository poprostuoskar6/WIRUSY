Oto instrukcja uruchomienia projektu Papiezak na podstawie struktury plików:

```markdown
# Instrukcja uruchomienia Papiezak (C# WPF)

## Wymagania wstępne
- [.NET Framework 4.7.2](https://dotnet.microsoft.com/download/dotnet-framework/net472) lub nowszy
- Visual Studio 2019+ (lub samodzielny kompilator)
- System Windows (WPF nie jest w pełni kompatybilny z Linux)

## 1. Klonowanie repozytorium
```cmd
git clone https://github.com/xProsek720/Papiezak.git
cd Papiezak
```

## 2. Kompilacja projektu
Otwórz rozwiązanie w Visual Studio:
1. Otwórz `Papiezak.csproj`
2. Zainstaluj brakujące pakiety NuGet (jeśli wymagane)
3. Skompiluj rozwiązanie (Ctrl + Shift + B)

## Alternatywnie przez CLI (Windows):
```powershell
msbuild /p:Configuration=Release
```

## 3. Uruchomienie aplikacji
Po kompilacji znajdziesz plik wykonywalny w:
```
Papiezak\bin\Release\Papiezak.exe
```

## W przypadku problemów
### Brakujące zależności:
- Zainstaluj [Microsoft Visual C++ Redistributable](https://aka.ms/vs/16/release/vc_redist.x64.exe)
- Włącz .NET Framework 3.5/4.7 w funkcjach systemu Windows

### Błędy kompilacji:

nuget restore
msbuild /t:Clean /t:Rebuild

## Ważne uwagi
1. Projekt zawiera komponenty WPF - wymaga systemu Windows
2. Pliki w folderze Properties to konfiguracje assembly
3. Sprawdź czy masz aktualną wersję [Git](https://git-scm.com/)

## Bezpieczeństwo
Przed uruchomieniem sprawdź:
- Zawartość plików *.cs pod kątem niestandardowych funkcji
- Konfigurację w Settings.settings
- Zależności w Papiezak.csproj

⚠️ Aplikacja może wymagać uprawnień administracyjnych do niektórych operacji!
```

Dokładne kroki mogą się różnić w zależności od:
- Wersji systemu operacyjnego
- Konfiguracji środowiska developerskiego
- Celu poszczególnych komponentów (np. WatchDog.cs, bowserKiller.cs)

Zalecana ścieżka dla użytkowników Linux:
1. Użyj maszyny wirtualnej z Windows
2. Lub skonwertuj projekt na .NET Core/Mono
3. Dostosuj kod do kompatybilności z Linux
