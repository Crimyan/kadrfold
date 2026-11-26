# Kadrfold

**Prosty i szybki edytor wideo na Windows, z auto-montażem, napisami i korekcją koloru.**

> **Wczesna wersja (beta): v0.1.1.** W becie Kadrfold jest darmowy. Mogą trafić się niedoróbki, więc rób kopie ważnych projektów i nagrań.

**[Pobierz Kadrfold 0.1.1 dla Windows](https://github.com/Crimyan/kadrfold/releases/download/v0.1.1-beta/Kadrfold_0.1.1_x64-setup.exe)**

[English](README.md)

## Co potrafi

**Montaż**

- Oś czasu ze ścieżkami obrazu i dźwięku, przycinanie, cięcie, przeciąganie plików z Eksploratora.
- Klatki kluczowe położenia, skali, obrotu i krycia.
- Przejścia między klipami.
- Korekcja koloru i warstwy korekcyjne, które zmieniają wszystko pod sobą.
- Cofanie i ponawianie każdej zmiany, autozapis i odzyskiwanie projektu po awarii.

**Auto-montaż**

- Wycina ciszę i wtrącenia („yyy”, „eee”). Najpierw widzisz proponowane cięcia i je zatwierdzasz, a jedno Ctrl+Z przywraca wszystko.
- Ścisza muzykę pod mową.

**Napisy**

- Napisy z rozpoznawania mowy (Whisper) liczone na Twoim komputerze. Nic nie jest wysyłane do internetu.
- Tłumaczenie napisów, też lokalnie (modele Gemma 4 przez llama.cpp albo Twoja Ollama).
- Style napisów, animacja słowo po słowie, napisy wtopione w obraz albo zapisane jako SRT.

**Eksport**

- MP4 kodowany na karcie graficznej (NVIDIA NVENC; koder Intela i AMD też, jeśli jest).
- Przeniesienie montażu do Premiere Pro (XML) i DaVinci Resolve (FCPXML).

## Instalacja

1. Pobierz **[Kadrfold_0.1.1_x64-setup.exe](https://github.com/Crimyan/kadrfold/releases/download/v0.1.1-beta/Kadrfold_0.1.1_x64-setup.exe)**. Wszystkie wersje: [Releases](../../releases).
2. Uruchom. Instaluje się tylko dla Twojego konta (bez uprawnień administratora) w `%LOCALAPPDATA%\Kadrfold` i dodaje skrót w menu Start. Instalator pyta o język (English albo Polski).
3. Windows SmartScreen może ostrzec o nieznanym wydawcy (beta nie jest podpisana): wybierz *Więcej informacji → Uruchom mimo to*.

**Wymagania:** Windows 10 lub 11 (64-bit), karta graficzna ze sterownikiem Vulkan (zalecana karta NVIDIA). WebView2 instaluje się sam, jeśli go brakuje.

Odinstalowanie: *Ustawienia → Aplikacje* w Windows.

## Modele i Twoje dane

Instalator zawiera program i FFmpeg. Modeli rozpoznawania mowy i tłumaczenia w nim **nie ma**: Kadrfold pobiera je dopiero przy pierwszym użyciu napisów albo tłumaczenia i przed pobraniem pokazuje ich rozmiar.

Miniatury, fale dźwięku, autozapisy i pobrane modele leżą w folderze danych, domyślnie `%LOCALAPPDATA%\app.kadrfold.desktop`. Modele potrafią zająć kilka gigabajtów, więc w *Pomoc → Folder danych i modeli* możesz wybrać inny folder albo dysk. Nagrania i projekty zostają tam, gdzie je trzymasz.

## Aktualizacje

Kadrfold chwilę po starcie i potem co kilka godzin sprawdza na tej stronie, czy jest nowa wersja. Gdy jest, na pasku tytułu pojawia się przycisk **↑ Aktualizacja**: instalujesz ją jednym kliknięciem, po zapisaniu projektu. Z GitHuba pobierany jest tylko plik z numerem wersji, nic o Twoich projektach ani plikach nie jest wysyłane. Automatyczne sprawdzanie wyłączysz w *Pomoc → Sprawdź aktualizacje*.

## Stan

Beta, darmowa, kod zamknięty. Znalazłeś błąd albo masz pomysł? Załóż [zgłoszenie](../../issues): zrzut ekranu i kroki do powtórzenia bardzo pomagają.

## Licencja

W becie Kadrfold można pobierać i używać za darmo. Kod źródłowy nie jest publiczny. Zobacz [LICENSE.txt](LICENSE.txt).
© 2026 Crimyan. Wszelkie prawa zastrzeżone.

Kadrfold korzysta z komponentów firm trzecich na ich własnych licencjach, m.in. z FFmpeg na licencji LGPL (bez części GPL). Pełna lista z tekstami licencji jest w [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt), w folderze programu po instalacji i w *Pomoc → O programie i licencje*.
