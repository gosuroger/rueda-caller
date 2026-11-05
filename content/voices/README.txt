Nagrania wywolan figur
=====================

Kazdy glos ma osobny katalog:
  ../rueda-content/voices/default/       - pierwszy zestaw nagran
  ../rueda-content/voices/voice-02/      - przyklad drugiego zestawu

Katalog nowego glosu nazwij malymi literami ASCII, cyframi i myslnikami.
Kazdy katalog zawiera komplet wywolan jednej osoby. Te same nazwy plikow
w roznych katalogach odpowiadaja tym samym figurom.

Nazwa pliku: nazwa figury malymi literami, spacje zamienione na myslniki.
ID w ../rueda-content/figures/figures.tsv sa zgodne z nazwami figur w tym formacie.
Rozszerzenie zachowaj zgodne z rzeczywistym formatem: .m4a albo .wav.
Hiszpanskie akcenty pozostaja w name/shout, ale nie w ID i nazwach plikow.
Przyklady: Siéntala -> sientala.m4a, Vacílala -> vacilala.m4a.
Pozostale pliki nazwij wedlug aktualnej kolumny id w figures.tsv.
W nagraniu wypowiedz tekst z kolumny shout.

Plik                         Tekst do wypowiedzenia
---------------------------  ----------------------
mosquito.m4a                 Mosquito
mosquito-doble.m4a            Mosquito doble
mosquito-triple.m4a           Mosquito triple
dame.m4a                     Dame
dame-dos.m4a                 Dame dos
dame-dos-con-uno.m4a          Dame dos con uno
dame-dos-con-dos.m4a          Dame dos con dos
pisa.m4a                     Pisa
pisa-bum.m4a                 Pisa Bum
mosquito-loco.m4a             Mosquito loco
enchufla.m4a                 Enchufla
enchufla-doble.m4a            Enchufla doble
cadeneta.m4a                 Cadeneta
cadeneta-basta.m4a            Basta
cadeneta-dummy-1.m4a          Cadeneta dummy 1
enchufla-sientala.m4a         Enchufla sientala
sientala.m4a                 Sientala
giro.m4a                     Giro
olivia.m4a                   Olivia
olivia-doble.m4a             Olivia doble

M4A (zwykle AAC) jest odpowiedni, jesli przegladarka obsluguje jego kodek.
Alternatywa: WAV PCM 16-bit, mono, 44100 Hz lub 48000 Hz.
Jeden plik = jedno wywolanie, bez muzyki, bez ciszy przed wypowiedzia,
bez obcietego poczatku/konca slowa i bez przesterowania.
Wyrownaj glosnosc pomiedzy plikami i uzyj tego samego formatu dla zestawu.

Przyklady:
  ../rueda-content/voices/default/enchufla.m4a
  ../rueda-content/voices/voice-02/enchufla.m4a

Aplikacja odtwarza M4A z zestawu default jako zapowiedzi figur.
Nagrania potrzebne dla planu sa dekodowane przed Play.
Brak nagrania, blad pobierania lub dekodowania jest sygnalizowany w UI
i zastepowany beepem, bez przerywania muzyki.
Wybor zestawu w UI i odtwarzanie alternatywnych WAV nie sa jeszcze podpiete.
