Zewnetrzne dane Rueda Caller
==========================

Ten katalog jest obok rueda-caller, nie wewnatrz kodu aplikacji.

music/tracks/                  - utwory MP3/WAV
music/configuration/<id>.json  - konfiguracja kazdego utworu
figures/figures.tsv            - tabela figur
figures/figure-phases.tsv      - fazy figur
figures/combination-timing-rules.tsv - reguly kombinacji
voices/default/<figureId>.m4a  - pierwszy zestaw glosow
voices/voice-02/               - kolejny zestaw glosow

audioPath w konfiguracji jest wzgledny do music, np. tracks/song.mp3.
Vite udostepnia ten katalog tylko do odczytu pod /content/.
music/catalog.json jest generowany z music/configuration/*.json.
Po recznej zmianie danych odswiez aplikacje; edycja i zapis przez UI
nie sa jeszcze wdrozone. Eksport pomiaru pobiera plik, nie nadpisuje go.

npm run build w rueda-caller kopiuje dane do dist/content, aby wynik
dzialal na zwyklym hostingu statycznym. Kod JS pobiera dane przez HTTP;
TSV i konfiguracje nie sa wbudowane w bundle aplikacji.
Po dodaniu/usunieciu konfiguracji na hostingu zbuduj ponownie katalog.
Pliki w dist sa publiczne; nie umieszczaj tutaj danych poufnych.
