.. _Device Manager:

Menedżer Urządzeń
======================================

Menedżer Urządzeń CharaChorder to kompleksowe narzędzie dla użytkowników urządzeń z
systemem CCOS. Oferuje wysokiej jakości grafikę, animacje i prosty interfejs użytkownika.
W Menedżerze Urządzeń możesz zmieniać :ref:`układ<Device Manager:Layout>`, zarządzać swoją
:ref:`biblioteką akordów<Device Manager:Library>`, oraz dostosowywać
:ref:`ustawienia<Device Manager:Device>` swojego urządzenia.

W tej sekcji omówimy Menedżer Urządzeń i sposoby nawigacji w nim, abyś mógł skonfigurować
swoje urządzenie według własnych preferencji. Najpierw opiszemy stronę internetową i
przyciski na niej, potem przejdziemy przez główne sekcje Menedżera Urządzeń i ich
użycie, a na końcu wspomnimy o dodatkowych funkcjach i narzędziach.

Możesz skorzystać z poniższych odnośników, aby przejść do interesującej Cię sekcji, lub
po prostu przewinąć na początek.

.. contents:: Spis treści tej strony
   :local:

.. _Device Manager:Connecting to the Device Manager:

Łączenie z Menedżerem Urządzeń
*********************************

Możesz wykonać poniższe kroki, aby połączyć się z Menedżerem Urządzeń po raz pierwszy.

.. Note::
    Jeśli wcześniej wybrałeś :ref:`Auto-connect<Autoreconnect>` w tej samej przeglądarce dla
    tego samego urządzenia, być może nie będziesz musiał powtarzać tych kroków za każdym
    razem przy wchodzeniu na stronę menedżera.

1. W przeglądarce opartej na Chromium, takiej jak Chrome lub Edge, przejdź na stronę
   `CharaChorder Device Manager <https://charachorder.io>`__.
2. Kliknij „Connect” na dole ekranu, na środku.
3. Gdy pojawi się okno z napisem „charachorder.io wants to connect to a serial port”,
   wybierz swoje urządzenie CharaChorder, a następnie kliknij przycisk „Connect”.


.. image:: /assets/images/ManagerSELECTDEVICE.png
  :width: 400
  :alt: Obraz przedstawiający okno dialogowe z prośbą o połączenie przez port szeregowy

Jeżeli wykonasz powyższe kroki poprawnie, zobaczysz nazwę podłączonego urządzenia na dolnym
pasku tam, gdzie wcześniej widniał napis „Connect”.

.. _Device Manager:serialportaccess:

Dostęp do portu szeregowego w systemie Linux
--------------------------

.. warning::
    Dla użytkowników **Linuxa**: dostęp do portu szeregowego często jest ograniczony do
    określonych grup użytkowników ze względów bezpieczeństwa.
    Aby umożliwić dostęp do portu szeregowego w przeglądarce (takiej jak Chromium),
    musisz dodać swojego użytkownika do odpowiedniej grupy w zależności od dystrybucji
    Linuksa. Wykonaj poniższe kroki, aby przyznać dostęp.

Dla Ubuntu, Debian, Fedora, Linux Mint, openSUSE, CentOS, Elementary OS, Zorin OS:

.. code-block:: bash

    sudo usermod -aG dialout $USER

Dla Arch Linux, Manjaro:

.. code-block:: bash

    sudo usermod -aG uucp $USER

Zastąp ``$USER`` swoją nazwą użytkownika lub pozostaw ``$USER``, aby automatycznie
odwołać się do bieżącego użytkownika.
Wyloguj się i zaloguj ponownie, aby zmiany zaczęły obowiązywać.

Jeśli powyższe polecenia nie działają, sprawdź właściciela grupowego urządzenia
szeregowego (np. ``/dev/ttyUSB0``) za pomocą:

.. code-block:: bash

    ls -l /dev/ttyUSB0

To polecenie wyświetli grupę urządzenia. Zamień ``/dev/ttyUSB0`` na odpowiedni plik urządzenia w twoim systemie.
Po zidentyfikowaniu grupy (np. ``dialout``, ``uucp`` lub innej), dodaj swojego użytkownika do tej grupy, używając:

.. code-block:: bash

    sudo usermod -aG <group_name> $USER

Zastąp ``<group_name>`` nazwą grupy wyświetloną w poprzednim kroku.
Wyloguj się i zaloguj ponownie, aby zastosować zmiany.
Twój użytkownik uzyska teraz niezbędne uprawnienia do dostępu do portu szeregowego.

.. _Device Manager Website:

Strona internetowa Device Managera
************************

Device Manager posiada menu nawigacyjne po lewej stronie ekranu.
Niezależnie jednak od tego, na której stronie się znajdujesz,
istnieje kilka przydatnych przycisków, które warto znać.


Połącz / Nazwa urządzenia
---------------------

Na dole, na środku ekranu, znajduje się miejsce, w którym możesz połączyć się
ze swoim urządzeniem i zobaczyć, z którym urządzeniem jesteś aktualnie
połączony, a także inne informacje, takie jak wersja strony i wersja CCOS
twojego urządzenia.

Cofnij i ponów
---------------

.. image:: /assets/images/ManagerUndoRedo.png
  :width: 200
  :alt: Strzałki Cofnij i Ponów

W lewym górnym rogu znajdują się wygodne przyciski cofania i ponawiania,
które działają dokładnie tak, jak sugerują ich nazwy. Podczas wprowadzania
zmian w układzie, akordach lub innych ustawieniach możesz cofać je
pojedynczo, aż do pierwszej wprowadzonej zmiany podczas tej sesji.
Po cofnięciu możesz także ponawiać zmiany, które wcześniej zostały cofnięte.

.. _Device Manager:Color Scheme:

Schemat kolorów
--------------

W prawym dolnym rogu Device Managera zobaczysz kółko o jednolitym kolorze.
Po najechaniu na nie kursorem pojawi się etykieta "color scheme" (schemat kolorów).
Klikając to kółko, możesz zmienić schemat kolorów Device Managera.
W menu schematu kolorów możesz wybrać preferowany kolor przy pomocy palety
kolorów, systemu RGB lub poprzez ikonę pipety, aby wybrać kolor z ekranu.

.. image:: /assets/images/ManagerColorScheme.png
  :width: 300
  :alt: Menu schematu kolorów

Tryb jasny i ciemny
--------------------

Również w prawym dolnym rogu znajdziesz ikonę słońca lub księżyca, za pomocą
której możesz przełączać się między trybem jasnym i ciemnym. Przełącznik ten
może być pomocny dla osób, które preferują jaśniejszy ekran w celu lepszej
widoczności lub ciemniejszy, aby zmniejszyć zmęczenie oczu.

.. _Device Manager:Save Button:

Przycisk zapisu
-------------

.. image:: /assets/images/ManagerSaveButton.png
  :width: 200
  :alt: Przycisk zapisu

Jeżeli wprowadzisz zmiany w :ref:`bibliotece<Device Manager:Library>`,
:ref:`edytorze układu<Device Manager:Layout>` lub
:ref:`menu ustawień<Device Manager:Settings Menu>`, na górze po lewej
stronie pojawi się kolorowy przycisk "save" (zapisz).

.. Note::
    Zmiany nie zostaną zastosowane dopóki nie klikniesz przycisku zapisu.


.. _Device Manager:Device:

Urządzenie
***************

Zakładka *Device* to miejsce, w którym możesz skonfigurować większość
ustawień swojego :ref:`podłączonego<Device Manager:Connecting to the Device Manager>`
urządzenia CCOS i tworzyć kopie zapasowe.
Poniżej znajdziesz różne ustawienia, które możesz zmieniać.
Bardziej szczegółowe wyjaśnienia znajdziesz w sekcji
:doc:`GTM<GenerativeTextMenu>`.


.. _Backup Section:

Sekcja kopii zapasowych
----------------

.. image:: /assets/images/ManagerHistoryMenu.png
  :width: 400
  :alt: Menu kopii zapasowych

Menu *Backup* zawiera Twoje kopie zapasowe, a także umożliwia
przywracanie urządzenia z pliku kopii zapasowej. Istnieje
kilka rodzajów kopii zapasowych, które możesz
utworzyć – omówimy je w sekcji
:ref:`backups<Device Manager:Backups>`.

Jeśli włączysz opcję "Auto-backup", strona zapisze kopię zapasową
w Twojej przeglądarce. Kopia ta przechowywana jest lokalnie na
Twoim komputerze, więc tylko TY masz do niej dostęp.

W Device Managerze możesz tworzyć kopie zapasowe swoich akordów,
układu oraz ustawień. Poniżej przedstawiamy kroki jak utworzyć
i przywrócić kopie zapasowe dla Twojego urządzenia :doc:`CCOS<CCOS>`.


.. _Device Manager:Creating a Backup:

Tworzenie kopii zapasowej
~~~~~~~~~~~~~~~~~~

.. Note::
    Aby wykonać poniższe kroki, musisz być już
    :ref:`połączony<Device Manager:Connecting to the Device Manager>`
    z Device Managerem.

1. Otwórz zakładkę *Device* i znajdź menu "Backup" w lewym górnym rogu.

2. Wybierz "individual backup", aby pobrać kopię zapasową na komputer,
   albo "download everything", aby pobrać pojedynczy plik zawierający
   wszystkie trzy części. Pliki zostaną zapisane w formacie *.json*.

    .. note::
        Możesz wykonać osobne kopie zapasowe akordów, układu lub ustawień.
        Opcja "download everything" pobierze wszystkie trzy naraz w jednym pliku.

3. W razie potrzeby wybierz lokalizację zapisu na komputerze i nadaj plikowi dowolną nazwę.

Gratulacje! Kopia zapasowa została utworzona.


.. _Restoring from a Backup:

Przywracanie z kopii zapasowej
~~~~~~~~~~~~~~~~~~~~~~~~~

Dodatkowo możesz przywracać akordy, układ i ustawienia w Device Managerze. Wykonaj następujące kroki:

.. Note::
    Aby wykonać te kroki, musisz być już
    :ref:`połączony<Device Manager:Connecting to the Device Manager>` z Device Managerem.

1. Otwórz zakładkę *Device* i znajdź menu "Backup" w lewym górnym rogu.

2. Kliknij "Restore".

3. Wybierz plik, z którego chcesz przywrócić dane. Plik powinien być w formacie *.json*.

    .. note::
        Pliki do przywracania tworzone są wcześniej poprzez
        :ref:`tworzenie kopii zapasowej<Device Manager:Creating a Backup>`.

4. Jeśli wystąpią zmiany, na górze po lewej stronie pojawi się
:ref:`przycisk zapisu<Device Manager:Save Button>`. Sprawdź
zmiany w odpowiedniej zakładce: akordy w
:ref:`bibliotece<Device Manager:Chord Manager>`, układ w
:ref:`układzie<Device Manager:Layout>`, a ustawienia w
:ref:`ustawieniach<Device Manager:Settings Menu>`.

    .. note::
        Przywracanie nie kasuje danych z urządzenia. W przypadku konfliktów
        (np. zmiana ustawienia, inny klawisz w układzie czy inny
        :ref:`output<Chords:Chord Output>` akordu), dane zostaną nadpisane.
        Ustawienia i układ zawsze nadpisują całość.

5. Po sprawdzeniu zmian kliknij :ref:`save<Device Manager:Save Button>`, aby je zatwierdzić.


.. _Device Section:

Sekcja urządzenia
----------------

.. _Autoreconnect:

Tutaj znajdziesz przydatny przełącznik "Auto-connect". Po jego włączeniu
Device Manager automatycznie połączy się z Twoim urządzeniem poprzez
:doc:`połączenie szeregowe<SerialAPI>` za każdym razem, gdy otworzysz
stronę. Podczas połączenia automatycznie odczyta również Twoje akordy,
aby wykryć ewentualne zmiany od ostatniego połączenia. Dzięki temu
nie musisz już ręcznie łączyć się z Device Managerem za każdym razem!

W tej sekcji możesz także włączyć lub wyłączyć komunikaty
:ref:`powitalne<GenerativeTextMenu:Startup>` oraz
:ref:`informacje w czasie rzeczywistym<GenerativeTextMenu:Realtime Feedback>`.
Dodatkowo możesz wyczyścić niektóre dane urządzenia: akordy, układ,
a nawet przywrócić ustawienia fabryczne.

.. image:: /assets/images/ManagerSettingsDevice.png
  :width: 1200
  :alt: Okno ustawień urządzenia

.. _Spurring:

Akordowanie natychmiastowe
----------

.. dropdown:: Czym jest Akordowanie natychmiastowe?

    *Akordowanie natychmiastowe* to tryb „tylko akordowy”, w którym urządzenie wysyła
    :ref:`akordy<Chords:What are Chords>` już w momencie wciśnięcia przycisku,
    a nie dopiero po wciśnięciu i zwolnieniu.
    W trybie *Akordowania natychmiastowego* możesz wciskać klawisze
    :ref:`akordu<Chords:What are Chords>` pojedynczo, z dłuższymi
    odstępami czasowymi, co ułatwia naukę akordowania bez presji dokładnego
    :ref:`timingu<GenerativeTextMenu:Press Tolerance>`.

    Akordowanie natychmiastowe umożliwia również przechodzenie z jednego
    :ref:`akordu<Chords:What are Chords>` do drugiego bez konieczności
    całkowitego zwalniania wszystkich klawiszy.
    Dla zaawansowanych użytkowników może to znacznie zwiększyć szybkość pisania,
    kosztem utraty możliwości klasycznego wprowadzania znaków.

.. image:: /assets/images/ManagerSettingsSpurring.png
  :width: 1200
  :alt: Okno ustawień Akordowania natychmiastowego

W tym oknie możesz włączyć lub wyłączyć tryb *Akordowanie natychmiastowe*, a także ustawić czas
bezczynności za pomocą :ref:`limitu czasu akordowania natychmiastowego<GenerativeTextMenu:Spurring Timeout>`.

Arpeggiacja
-------------
.. dropdown:: Czym są Arpeggiacje?

    *Arpeggiacje* to akcje czasowe, które modyfikują
    :ref:`akord<Chords:What are Chords>` po jego wykonaniu. Typowym przykładem
    jest użycie :ref:`modyfikatorów akordów<Device Manager:Chord Modifiers>`
    tuż po wykonaniu akordu. Możesz przeczytać tą sekcję aby dowiedzieć się
    jak działają modyfikatory akordów.

    Przykładowo: po zaakordowaniu słowa *run*, możesz w czasie trwania
    :ref:`limitu czasu arpeggiacji<GenerativeTextMenu:Arpeggiate Timeout>`
    wcisnąć :ref:`modyfikator czasu przeszłego<Device Manager:Past tense>`, aby zamienić je na *ran*.

.. image:: /assets/images/ManagerSettingsArpeggiates.png
  :width: 1200
  :alt: Okno ustawień Arpeggiacji

W tym oknie możesz włączyć lub wyłączyć Arpeggiacje oraz dostosować czas
za pomocą :ref:`Limit czasu arpeggiacji<GenerativeTextMenu:Arpeggiate Timeout>`.

.. _Device Manager:Chord Modifiers:

Modyfikatory akordów
-----------------

.. dropdown:: Czym są modyfikatory akordów?

    Modyfikatory akordów to akcje, które zmieniają akord w momencie
    :ref:`akordowania<Chords:What are Chords>` — mogą być wykonywane
    razem z :ref:`wejściem akordu<Chords:Chord Input>` lub bezpośrednio
    po nim (arpeggiacyjnie), o ile włączone są
    :ref:`arpeggiates<GenerativeTextMenu:Arpeggiate>`.

    Na luty 2024 obsługa modyfikatorów akordów dostępna jest wyłącznie
    na urządzeniach CharaChorder One i CharaChorder Lite oraz tylko w
    języku angielskim.

    .. note::
        Modyfikatory akordów nie są tym samym co modyfikatory klawiaturowe
        (``CTRL``, ``ALT``, ``FN``), które działają na zwykłych klawiszach.
        Modyfikatory akordów działają na akordach.

.. image:: /assets/images/ManagerSettingsModifiers.png
  :width: 1200
  :alt: Okno ustawień modyfikatorów akordów

W tym oknie znajdziesz krótkie wyjaśnienie modyfikatorów oraz sposób, za pomocą którego możesz się do nich dostać.

Kapitalizacja
~~~~~~~~~~~~~~~

Modyfikator kapitalizacji modyfikuje dowolny akord tak, aby pierwsza litera w
:ref:`wyniku<Chords:Chord Output>` była zapisana wielką literą.
Ten :ref:`modyfikator<Device Manager:Chord Modifiers>` można wykonać
jednocześnie z :ref:`akordem<Chords:What are Chords>` lub
:ref:`arpeggiate<GenerativeTextMenu:Arpeggiate>`.

Modyfikator kapitalizacji przypisany jest do klawisza ``SHIFT``.
W :ref:`edytorze układu<Device Manager:Layout>` klawisz ten nosi
nazwę „Shift Keyboard Modifier (Left)” lub
„Shift Keyboard Modifier (Right)”.

.. note::
    Jeśli masz aktywny ``CAPS LOCK``, wszystkie litery w akordzie zostaną
    zapisane wielkimi literami, z wyjątkiem pierwszej litery podczas
    używania tego modyfikatora.

Czas teraźniejszy
~~~~~~~~~~~~~~

Modyfikator czasu teraźniejszego modyfikuje obsługiwane akordy tak, aby
przekształcić je w warianty czasu teraźniejszego. Słowo „run” zmieni
się na „running”, a „work” na „working”. Ten
:ref:`modyfikator<Device Manager:Chord Modifiers>` można wykonać
jednocześnie z :ref:`akordem<Chords:What are Chords>` lub
:ref:`arpeggiate<GenerativeTextMenu:Arpeggiate>`.

Lokalizacja modyfikatora zależy od urządzenia. Na CharaChorder One
modyfikator ten jest przypisany do klawisza
„AMBIDEXTROUS THROWOVER (LEFT)”. Na CharaChorder Lite — do
klawisza „NUMERIC LAYER (LEFT)”.

Liczba mnoga
~~~~~~~~~~~

Modyfikator liczby mnogiej sprawia, że obsługiwane akordy przyjmują formę mnogą.
Dodaje „s” lub „es” na końcu obsługiwanych akordów. Przykładowo: „Box” zmieni
się na „boxes”, a „dog” na „dogs”.
Ten :ref:`modyfikator<Device Manager:Chord Modifiers>` można wykonać jednocześnie z
:ref:`akordem<Chords:What are Chords>` lub
:ref:`arpeggiate<GenerativeTextMenu:Arpeggiate>`.

Lokalizacja modyfikatora zależy od urządzenia. Na CharaChorder One przypisany jest
do klawisza „AMBIDEXTROUS THROWOVER (RIGHT)”. Na CharaChorder Lite — do klawisza
„RIGHT SPACEBAR” (nie mylić z klawiszem „SPACE”).

.. _Device Manager:Past tense:

Czas przeszły
~~~~~~~~~~~

Modyfikator czasu przeszłego modyfikuje obsługiwane akordy tak, aby przekształcić
je w warianty czasu przeszłego. Słowo „run” zmieni się na „ran”, a „work” na
„worked”. Ten :ref:`modyfikator<Device Manager:Chord Modifiers>` można wykonać
jednocześnie z :ref:`akordem<Chords:What are Chords>` lub
:ref:`arpeggiate<GenerativeTextMenu:Arpeggiate>`.

Lokalizacja modyfikatora zależy od urządzenia. Na CharaChorder One przypisany
jest do klawisza „NUMERIC LAYER (LEFT)”. Na CharaChorder Lite — do klawisza
„SPACE” (nie mylić z klawiszem „RIGHT SPACEBAR”).

Stopień wyższy
~~~~~~~~~~~~~

Modyfikator stopnia wyższego modyfikuje obsługiwane akordy tak, aby
przekształcić je w formę porównawczą. „Big” staje się „bigger”, a
„small” zmienia się na „smaller”.
Ten :ref:`modyfikator<Device Manager:Chord Modifiers>` można wykonać
jednocześnie z :ref:`akordem<Chords:What are Chords>` lub
:ref:`arpeggiate<GenerativeTextMenu:Arpeggiate>`.

Modyfikator ten przypisany jest do klawisza „NUMERIC LAYER (RIGHT)”
zarówno na CharaChorder One, jak i na CharaChorder Lite.

Wprowadzanie znaków
----------------

.. dropdown:: Czym jest wprowadzanie znaków?

    Wprowadzanie znaków, znane w społeczności CharaChorder jako „chentry”,
    oznacza pisanie pojedynczych znaków jeden po drugim.

.. image:: /assets/images/ManagerSettingsChentry.png
  :width: 1200
  :alt: Pole ustawień wprowadzania znaków

W tym polu możesz zmieniać ustawienia związane z używaniem urządzenia do wprowadzania pojedynczych znaków.

.. dropdown:: Zamiana mapowania klawiszy 0 i 1

    To ustawienie zamienia funkcje dwóch klawiszy w lewym dolnym rogu CharaChorder Lite.

    Tradycyjne klawiatury QWERTY mają klawisz ``CTRL`` w lewym dolnym rogu, a klawisz
    ``GUI`` (klawisz Command na Macu, klawisz Windows na Windows, klawisz Super na
    Linuksie itd.) po prawej stronie od ``CTRL``. W CharaChorder Lite te dwa klawisze
    są domyślnie zamienione, co dla niektórych użytkowników bywa nieintuicyjne i
    trudne do przyzwyczajenia. Nowe urządzenie CharaChorder Lite ma klawisz ``GUI``
    w lewym dolnym rogu, a ``CTRL`` po jego prawej stronie.

    Dzięki temu ustawieniu możesz na poziomie CCOS zamienić te klawisze miejscami, aby
    ``CTRL`` był w lewym dolnym rogu.

.. dropdown:: Wprowadzanie znaków (chentry)

    To ustawienie jest przełącznikiem, który dezaktywuje funkcje akordowania na
    urządzeniach CCOS. Domyślnie jest wyłączone, ale można je włączyć, jeśli
    nie chcemy używać akordów. Ustawienie to bywa przydatne np. podczas grania
    w gry, gdy nie chcemy przypadkowo aktywować akordów.

    Jeśli Twoje urządzenie CCOS nagle utraci zdolność akordowania, warto sprawdzić,
    czy to ustawienie nie jest aktywne.

.. dropdown:: Częstotliwość skanowania klawiszy

    Częstotliwość skanowania, czasem nazywana „czasem skanowania klawisza”,
    odnosi się do częstotliwości sprawdzania przez urządzenie stanu klawiszy.
    Dla odniesienia: 5 ms odpowiada 200 Hz, co oznacza, że :doc:`CCOS<CCOS>`
    sprawdza pozycję klawiszy co 5 milisekund, czyli 200 razy na sekundę.
    Niższe wartości zazwyczaj są lepsze, ponieważ zwiększają responsywność
    CCOS, chociaż przy niskich wartościach różnice są zwykle niewielkie.
    W GTM to ustawienie można regulować w milisekundach (ms).

.. dropdown:: Odbijanie przy wciśnięciu klawisza

    Ustawienie debounce press określa przedział czasowy (w milisekundach),
    w którym :doc:`CCOS<CCOS>` odfiltrowuje podwójne aktywacje klawisza
    przy zdarzeniu wciśnięcia. Innymi słowy, wszystkie powtórne aktywacje
    w tym przedziale będą liczone jako jedno naciśnięcie.

    Należy dostosować to ustawienie, jeśli pojawiają się niechciane,
    powtarzające się znaki podczas pisania. Zwiększenie tej wartości
    zmniejszy prawdopodobieństwo wystąpienia takich błędów, ponieważ
    :doc:`CCOS<CCOS>` będzie czekać dłużej zanim wprowadzi kolejny znak przypisany
    do tego samego kierunku przełącznika. Jednak zbyt wysokie ustawienie
    może spowodować problemy z rozpoznawaniem zamierzonych podwójnych
    naciśnięć, dlatego zaleca się testowanie różnych wartości w
    niewielkich krokach. Ustawienie to powinno być używane w połączeniu
    z ustawieniem debounce release.

.. dropdown:: Odbijanie przy puszczeniu klawisza

    Ustawienie "Odbijanie przy puszczeniu klawisza" określa przedział
    czasowy (w milisekundach), w którym :doc:`CCOS<CCOS>` odfiltrowuje
    podwójne aktywacje klawisza przy zdarzeniu puszczenia. Innymi
    słowy, wszystkie powtórne aktywacje w tym przedziale będą liczone
    jako jedno puszczenie.

    Należy dostosować to ustawienie, jeśli pojawiają się niechciane,
    powtarzające się znaki podczas pisania. Zwiększenie tej wartości
    zmniejszy prawdopodobieństwo wystąpienia takich błędów, ponieważ
    CCOS będzie czekać dłużej zanim wprowadzi kolejny znak przypisany
    do tego samego kierunku przełącznika. Jednak zbyt wysokie
    ustawienie może spowodować problemy z rozpoznawaniem zamierzonych
    podwójnych naciśnięć, dlatego zaleca się testowanie różnych wartości
    w niewielkich krokach. Ustawienie to powinno być używane w połączeniu
    z ustawieniem debounce press.

.. dropdown:: Opóźnienie wprowadzania znaków

    To ustawienie dodaje niewielkie opóźnienie do wprowadzania znaków.
    Mierzone jest w mikrosekundach (μs) i domyślnie ma bardzo małą wartość.

    Należy zwiększyć tę wartość, jeśli komputer nie przyjmuje wszystkich
    znaków wysyłanych przez urządzenie, np. podczas używania
    :doc:`GTM<GenerativeTextMenu>`. W przypadku tego problemu
    :doc:`GTM<GenerativeTextMenu>` może wyglądać dziwnie, z
    brakującymi fragmentami lub znakami.

    Jeśli masz szybszy komputer, możesz obniżyć to ustawienie, aby
    akordowanie i :doc:`GTM<GenerativeTextMenu>` były szybsze i
    bardziej responsywne.

Mysz
-------

.. dropdown:: Mysz ???

    :doc:`CCOS<CCOS>` posiada funkcję myszy. Oznacza to, że Twój CharaChorder
    lub klawiatura z systemem CCOS może kontrolować mysz Twojego komputera.
    Te ustawienia wpływają na sposób działania myszy w CharaChorder.

.. image:: /assets/images/ManagerSettingsMouse.png
  :width: 1200
  :alt: Pole ustawień Myszy

W tym polu możesz dostosować ustawienia związane z funkcjami myszy w :doc:`CCOS<CCOS>`.

.. dropdown:: Prędkość myszy

    :doc:`CCOS<CCOS>` ma dwie prędkości myszy: szybka (fast speed) i wolna (slow speed).
    Wolna prędkość jest aktywowana, gdy używasz tylko jednego klawisza myszy w jednym
    kierunku (w przeciwieństwie do używania dwóch klawiszy w tym samym kierunku).
    Szybka prędkość jest aktywowana, gdy używasz dwóch klawiszy myszy w jednym
    kierunku (zamiast tylko jednego).

    Możesz przeczytać dokładniejsze wyjaśnienie prędkości myszy w sekcji
    :ref:`GTM<GenerativeTextMenu:Slow Speed>`.

.. dropdown:: Prędkość przewijania

    Prędkość przewijania odnosi się do szybkości, z jaką :doc:`CCOS<CCOS>` przewija ekran.

    Więcej szczegółów o prędkości przewijania znajdziesz w sekcji
    :ref:`GTM<GenerativeTextMenu:Scroll Speed>`.

.. dropdown:: Aktywna mysz

    Tryb aktywny przesuwa kursor myszy o jeden piksel mniej więcej raz na minutę
    (czas nie jest dokładnie określony). To ustawienie może być używane, aby
    zapobiec przechodzeniu komputera w tryb uśpienia. Warto wyłączyć to ustawienie,
    jeśli zauważysz, że aplikacje na pulpicie blokują powiadomienia mobilne
    (na przykład w Discord lub Microsoft Teams).

.. dropdown:: Częstotliwość odpytywania


    Częstotliwość odpytywania (poll rate) określa, jak często dane z funkcji myszy
    CharaChorder są przesyłane do podłączonego urządzenia. Innymi słowy — jak
    często aktualizowana jest pozycja kursora na komputerze.

    Szczegółowe wyjaśnienie znajdziesz w sekcji :ref:`GTM<GenerativeTextMenu:Poll Rate>`.

Akordowanie
-----------

.. dropdown:: Czym jest Akordowanie?

    Akordowanie to piękna funkcja pozwalająca na naciśnięcie wielu klawiszy
    jednocześnie, aby uzyskać zdefiniowany wcześniej wynik, czy to pojedyncze
    słowo, całe zdanie, czy ważny adres.

    Akord to typ akcji wejścia/wyjścia na klawiaturze: naciskasz dwa lub więcej
    klawiszy jednocześnie i zwalniasz je jednocześnie, po czym wcześniej
    zdefiniowany wynik zastępuje naciśnięte klawisze.

    Dzięki akordowaniu możemy wpisywać całe słowa naraz, zamiast pojedynczych liter.
    Możliwe jest nawet tworzenie akordów dla całych fraz i zdań.

.. image:: /assets/images/ManagerSettingsChording.png
  :width: 1200
  :alt: Pole ustawień Akordowania

W tym polu możesz dostosować ustawienia związane z możliwościami
:doc:`CCOS<CCOS>` dotyczącymi :doc:`akordowania<Chords>`, a także
całkowicie wyłączyć :doc:`akordowanie<Chords>`, jeśli tak zdecydujesz.

.. dropdown:: Limit czasowy auto-usuwania

    To ustawienie zmienia czas, w którym CCOS liczy czas na zastąpienie
    znaków poprzedzających akord.

    Urządzenia CCOS posiadają licznik czasu, który uruchamia się po każdym
    wprowadzeniu znaku w trybie tradycyjnego wpisywania znaków (chentry,
    czyli wpisywanie litera po literze). Ten licznik decyduje, czy kolejny
    wykonany akord usunie poprzedzające znaki.

    Funkcja ta pozwala użytkownikom na poprawienie błędnie wykonanych akordów
    poprzez szybkie ponowne ich wykonanie, bez konieczności ręcznego usuwania
    błędnych znaków. Po upływie limitu czasu, system automatycznie usuwa
    wszystkie poprzedzające znaki (do ostatniego znaku łamiącego) i zastępuje
    je oczekiwanym akordem.

.. dropdown:: Tolerancja naciśnięcia

    Tolerancja naciśnięcia określa okno czasowe, w którym może zostać wykonany
    akord, mierzone w milisekundach (ms). Licznik ten uruchamia się przy
    pierwszym naciśnięciu pierwszego klawisza w akordzie i kończy się po
    naciśnięciu ostatniego klawisza, lub gdy limit czasu zostanie
    przekroczony — w zależności od tego, co nastąpi wcześniej.
    Dokładniejsze wyjaśnienie znajdziesz w sekcji
    :ref:`GTM<GenerativeTextMenu:Press Tolerance>`.

.. dropdown:: Tolerancja zwolnienia

    Tolerancja zwolnienia określa okno czasowe, w którym może zostać wykonany
    akord, mierzone w milisekundach (ms). Licznik ten uruchamia się przy
    pierwszym zwolnieniu dowolnego klawisza w akordzie i kończy po pełnym
    wykonaniu akordu lub po upływie limitu czasu — w zależności co nastąpi
    wcześniej. Dokładniejsze wyjaśnienie znajdziesz w sekcji
    :ref:`GTM<GenerativeTextMenu:Release Tolerance>`.

.. dropdown:: Akordowanie złożone

    Ta opcja pozwala na włączenie lub wyłączenie :ref:`akordów złożonych<Chords:Compound Chords>`.

RGB
------

Ustawienia RGB mają zastosowanie TYLKO dla CharaChorder Lite (stan na luty 2024).

Te ustawienia pozwalają dostosować kolor i jasność twojego CharaChorder Lite.

.. image:: /assets/images/ManagerSettingsRGB.png
  :width: 1200
  :alt: Pole ustawień RGB

.. _Device Manager:Library:

Biblioteka
***************

.. image:: /assets/images/ChordManager.png
  :width: 1200
  :alt: Obraz przedstawiający Bibliotekę

Biblioteka to potężne narzędzie, które pozwala na dodawanie, usuwanie
i edytowanie akordów zapisanych w twojej bibliotece akordów. Jest łatwa
w obsłudze i szybko się ładuje. Poniżej omówimy jak z niej korzystać.

Kiedy :ref:`połączysz<Device Manager:Connecting to the Device Manager>`
swoje urządzenie z menedżerem urządzenia, strona zacznie odczytywać
akordy z twojego urządzenia. Może to zająć kilka sekund — a nawet
ponad minutę w przypadku bardzo dużych bibliotek — podczas pierwszego
ładowania. Jeżeli masz włączoną opcję :ref:`auto-połączenia<Autoreconnect>`,
czas ładowania będzie znacznie krótszy.

Wyświetlane akordy są posortowane alfabetycznie według listy
:ref:`wyjść akordów<Chords:Chord Output>`. Liczba wyświetlanych akordów
zależy od rozmiaru ekranu i ustawień powiększenia przeglądarki.
Nad listą akordów znajduje się pasek wyszukiwania, który pokazuje liczbę
akordów na twoim urządzeniu CCOS, dopóki nic nie wpiszesz.

.. _search bar:

Możesz przeszukiwać akordy według :ref:`wyjść akordów<Chords:Chord Output>`
(słów pojawiających się po wykonaniu akordu). Pasek wyszukiwania nie
rozróżnia wielkości liter, możesz wpisywać litery małe lub wielkie
niezależnie od zapisu akordu. Wyszukiwanie jest również intuicyjne — możesz
wyszukiwać fragmenty słów lub fraz.

Po prawej stronie paska wyszukiwania znajdują się dwie liczby oddzielone
ukośnikiem (``/``). Liczby te wskazują numer aktualnej strony oraz łączną
liczbę stron, na które podzielona jest twoja biblioteka akordów.
Używając nawiasów kątowych znajdujących się po prawej stronie tych
liczb możesz przełączać się między stronami biblioteki, która jest
posortowana alfabetycznie.

Pod przyciskami przewijania stron zobaczysz wysokie pole tekstowe z napisem
"Try typing here". Możesz użyć tego pola do testowania nowych akordów
podczas ich edycji w menedżerze.

Pod polem tekstowym, jeśli twoje urządzenie to obsługuje, znajdziesz
kilka skrótów pozwalających na:

- wyczyszczenie biblioteki akordów,
- przywrócenie domyślnych akordów startowych,
- dodanie funkcjonalnych akordów użytkowych,
- pobranie pliku tekstowego ze wszystkimi wyjściami akordów oddzielonymi znakiem
  pionowej kreski (|), do użycia w narzędziach treningowych.

Na samym dole strony, jeżeli najedziesz kursorem na nazwę urządzenia, zauważysz,
że możesz przytrzymać klawisz **Shift** i kliknąć na nią, aby wykonać operację
"Sync". Powoduje to ponowne odczytanie biblioteki akordów z twojego urządzenia
przez menedżer urządzenia. Proces ten może zająć kilka sekund.

Tworzenie akordu
-----------------

Możesz wykonać poniższe kroki, aby utworzyć nowy akord w menedżerze urządzenia.

.. Note::
    Aby wykonać te kroki, musisz już mieć swoje urządzenie
    :ref:`połączone<Device Manager:Connecting to the Device Manager>`
    z menedżerem urządzenia.

1. Znajdź napis "New chord" (Nowy akord) pod :ref:`paskiem wyszukiwania<search bar>` i kliknij go.

2. Gdy pojawi się napis "Hold chord" (Przytrzymaj akord), naciśnij i przytrzymaj wszystkie klawisze,
   które chcesz wykorzystać jako swoje :ref:`wejście akordu<Chords:Chord Input>`.
   Po naciśnięciu wszystkich klawiszy zwolnij je.

   Teraz zobaczysz :ref:`wejście akordu<Chords:Chord Input>` w lewej kolumnie,
   przedstawione jako litery w indywidualnych polach. Te litery będą podświetlone
   kolorem (zamiast czarnego lub białego). Kolor zależy od wybranego
   :ref:`schematu kolorów<Device Manager:Color Scheme>`.
   Zauważysz również pojedynczą, unoszącą się kropkę w tym samym kolorze po
   prawej stronie pól z literami.

    .. Note::
        Możesz dodać dowolną liczbę akordów jednocześnie, nie definiując od razu
        :ref:`wyjścia akordu<Chords:Chord Output>`.

    .. Warning::
        Jeżeli klikniesz :ref:`zapisz<Device Manager:Save Button>` zanim zdefiniujesz
        :ref:`wyjście akordu<Chords:Chord Output>` zgodnie z :ref:`krokiem trzecim<Step 3>`,
        wszystkie utworzone akordy zostaną zapisane bez wyjścia, co może prowadzić do
        nieprawidłowego działania urządzenia.

.. _Step 3:

3. Kliknij w pole tekstowe po prawej stronie :ref:`wejścia akordu<Chords:Chord Input>`
utworzonego w poprzednim kroku i wpisz swoje docelowe
:ref:`wyjście akordu<Chords:Chord Output>`.

    .. dropdown:: Używanie kodów akcji

        Podczas wpisywania :ref:`wyjścia akordu<Chords:Chord Output>`, zauważysz,
        że nad kursorem pojawia się bańka z symbolem ``+``.
        Kliknij ją, aby otworzyć :ref:`menu kodów akcji<Device Manager:Using Action Codes>`,
        w którym możesz wyszukiwać konkretne kody akcji lub przeglądać dostępne kody do
        przypisania do :ref:`wyjścia akordu<Chords:Chord Output>`. Więcej o kodach akcji
        przeczytasz w sekcji :ref:`kody akcji<Device Manager:Using Action Codes>`.

    Podczas wpisywania tekst zmieni kolor na zgodny z wybranym
    :ref:`schematem kolorów<Device Manager:Color Scheme>`, a na końcu tekstu
    pojawi się unosząca się kropka.

4. Gdy będziesz zadowolony z :ref:`wyjścia<Chords:Chord Output>`, możesz przejść do edycji
kolejnego akordu lub kliknąć :ref:`zapisz<Device Manager:Save Button>`.

Usuwanie akordu
-----------------
Możesz wykonać poniższe kroki, aby usunąć akord w menedżerze urządzenia.

.. Note::
    Aby wykonać te kroki, musisz już mieć swoje urządzenie
    :ref:`połączone<Device Manager:Connecting to the Device Manager>` z menedżerem urządzenia.

1. Znajdź akord, który chcesz usunąć.

2. Gdy najedziesz kursorem na wybrany akord, zobaczysz małą ikonę kosza znajdującą się w
   linii z tym akordem. Kliknij ikonę kosza, aby oznaczyć akord do usunięcia.

    Po kliknięciu ikony kosza litery w lewej kolumnie zostaną przekreślone i zmienią kolor na czerwony.
    Możesz cofnąć oznaczenie akordu do usunięcia, klikając strzałkę „cofnij” obok ikony kosza.
    Litery powrócą wtedy do pierwotnego koloru i linia przekreślenia zniknie.

    .. tip::
        Możesz oznaczyć wiele akordów do usunięcia jednocześnie.
        Przechodzenie między stronami w bibliotece akordów nie anuluje oznaczeń.

3. Po oznaczeniu wszystkich akordów do usunięcia i gotowości do ich usunięcia, kliknij
   :ref:`przycisk zapisz<Device Manager:Save Button>`.

    Po kliknięciu „zapisz” oznaczone mapy akordów znikną z listy.

Edycja akordu
-----------------
Możesz wykonać poniższe kroki, aby edytować istniejący akord w menedżerze urządzenia.

.. Note::
    Aby wykonać te kroki, musisz już mieć swoje urządzenie
    :ref:`połączone<Device Manager:Connecting to the Device Manager>` z menedżerem urządzenia.

1. Znajdź akord, który chcesz edytować.

2. Kliknij pole tekstowe w prawej kolumnie, w którym wyświetla się
   :ref:`wyjście akordu<Chords:Chord Output>`.

3. Edytuj :ref:`wyjście akordu<Chords:Chord Output>` według własnych potrzeb.
   Podczas wpisywania tekst zmieni kolor, aby dopasować się do Twojego
   :ref:`schematu kolorów<Device Manager:Color Scheme>`, a na końcu
   tekstu pojawi się pływająca kropka.

    .. dropdown:: Korzystanie z kodów akcji

        Podczas wpisywania :ref:`wyjścia akordu<Chords:Chord Output>`, zauważysz,
        że nad kursorem pojawia się bąbel z ``+``. Możesz kliknąć ten przycisk,
        aby otworzyć :ref:`menu kodów akcji<Device Manager:Action Code Menu>`,
        w którym możesz wyszukiwać konkretne kody akcji lub przeglądać dostępne
        kody akcji do przypisania jako :ref:`wyjście akordu<Chords:Chord Output>`.
        Przeczytaj sekcję :ref:`kody akcji<Device Manager:Using Action Codes>`,
        aby uzyskać więcej informacji o różnych rodzajach kodów akcji.

    .. Tip::
        Możesz edytować wiele akordów przed :ref:`zapisaniem<Device Manager:Save Button>`
        zmian. Przechodzenie między stronami biblioteki akordów nie anuluje zmian
        wprowadzonych w istniejących akordach.

4. Po zakończeniu edycji kliknij :ref:`przycisk zapisz<Device Manager:Save Button>`, aby zapisać zmiany.

    Po kliknięciu :ref:`zapisz<Device Manager:Save Button>`, zmodyfikowane akordy
    zmienią kolor na taki sam jak reszta listy, a pływająca kropka zniknie.

Przycisk udostępniania
-------------

Obok każdego akordu zobaczysz ikonę udostępniania. Możesz udostępnić pojedyncze
mapowania akordów innym, naciskając ten przycisk. Gdy to zrobisz, adres URL
zostanie skopiowany do schowka Twojego komputera. Możesz go następnie udostępnić
innym, którzy dzięki temu będą mogli dodać dokładnie to samo mapowanie akordu do
swojego CharaChorder za pośrednictwem Menedżera Urządzenia.

Po kliknięciu odnośnika mapowania akordu zostaniesz przeniesiony do zakładki
Biblioteka, gdzie zobaczysz nowe mapowanie akordu gotowe do
:ref:`zapisania<Device Manager:Save Button>`.

.. _Device Manager:Layout:

Układ
**************

Menedżer Urządzenia posiada bardzo intuicyjny edytor warstw. Jest to trzecia opcja
w głównym pasku nawigacyjnym po lewej stronie strony. Po przejściu do tej zakładki
zobaczysz diagram swojego urządzenia, z każdą klawiszem wypełnionym odpowiednim
:ref:`kodem akcji<Device Manager:Using Action Codes>`.

.. _Device Manager:Layer Selector:

Selektor warstw
----------------

.. dropdown:: Wyjaśnienie warstw na urządzeniach CCOS

    Na dzień luty 2024 roku urządzenia :doc:`CCOS<CCOS>` posiadają trzy (3) warstwy,
    które możesz wykorzystać: warstwę podstawową, zwaną warstwą A1 (Alfa), warstwę
    drugorzędną, nazywaną A2 (Numeryczna), oraz warstwę trzeciorzędną, zwaną A3 (Funkcyjna).

    Aby uzyskać dostęp do warstw, należy nacisnąć i przytrzymać przycisk „dostępu do warstwy”.
    MUSISZ przytrzymać przycisk, aby użyć klawiszy przypisanych do innych warstw niż warstwa
    alfa. Warstwa alfa jest aktywna domyślnie.

    .. note::
        W tej sekcji odwołujemy się wyłącznie do domyślnych układów na urządzeniach CCOS.
        Jeżeli zmodyfikowałeś swój układ, poniższy opis może nie być dokładny dla Twojego
        urządzenia. Jeśli zakupiłeś urządzenie od CharaChorder, poniższe informacje są prawidłowe.

    **Warstwa A1**

    Warstwa A1, znana również jako warstwa alfa, jest główną warstwą aktywną domyślnie.
    Twoje urządzenie zawsze uruchamia się w warstwie A1.

    **Warstwa A2**

    Warstwa A2, czasami nazywana warstwą numeryczną, jest dostępna po naciśnięciu
    przycisku dostępu do warstwy :doc:`A2<CharaChorder Keys>`. W Menedżerze
    Urządzenia ten przycisk nosi nazwę „Numeric Layer (Left)” oraz
    „Numeric Layer (Right)”, osobno dla każdej ręki.

    Warstwa A2 jest dostępna przez naciśnięcie i przytrzymanie jednego z przycisków
    dostępu do warstwy. Każdy klawisz przypisany do warstwy A2 może zostać użyty
    tylko wtedy, gdy wciśnięty jest równocześnie przycisk dostępu do warstwy A2
    wraz z docelowym klawiszem. Nie musisz :doc:`akordować<Chords>` tych klawiszy
    razem; wymagane jest jedynie, by przycisk dostępu do warstwy A2 był wciśnięty
    w momencie naciskania klawisza docelowego.

    **Warstwa A3**

    Warstwa A3, czasami nazywana „warstwą funkcyjną”, jest dostępna po naciśnięciu
    przycisku dostępu do warstwy :ref:`A3<CharaChorder Keys>`. W Menedżerze
    Urządzenia ten przycisk jest przypisany jako „Function Layer (Left)” oraz
    „Function Layer (Right)”.

    Po przypisaniu przycisków dostępu do warstwy A3, dostęp do tej warstwy uzyskujemy
    przez naciśnięcie i przytrzymanie dowolnego z tych dwóch przycisków. Nie musisz
    przytrzymywać ich obu, by uzyskać dostęp do warstwy A3. Każdy klawisz przypisany
    do warstwy A3 może być aktywowany przez wciśnięcie i przytrzymanie przycisku
    dostępu do warstwy A3 razem z docelowym klawiszem. Nie musisz
    :doc:`akordować<Chords>` tych klawiszy razem; wymagane jest jedynie, by przycisk
    dostępu do warstwy A3 był wciśnięty w momencie naciskania klawisza docelowego.

.. Note::
    Poniższa sekcja zakłada, że Twoje urządzenie jest już
    :ref:`połączone<Device Manager:Connecting to the Device Manager>` z Menedżerem Urządzenia.

.. image:: /assets/images/ManagerLayoutSelector.png
  :width: 300
  :alt: Obraz selektora warstw

Nad diagramem urządzenia zobaczysz okrąg z literami „ABC” w środku.
Okrąg, wraz ze „skrzydłami” po lewej („123”) i prawej stronie („fx”),
tworzy selektor warstw. Możesz wybrać dowolny z nich, aby zobaczyć
klawisze przypisane do poszczególnych warstw.

.. _Device Manager:Remapping:

Przypisywanie na nowo
------------

W edytorze warstw możesz przypisać na nowo swój układ, używając
:ref:`kodów akcji<Device Manager:Using Action Codes>`.
Poniżej znajdziesz instrukcje, jak przypisać klawisze pojedynczo.

Jak przypisać klawisze na nowo
~~~~~~~~~~~~~~~~~~~~~~~

.. Note::
    Aby wykonać te kroki, Twoje urządzenie musi być już
    :ref:`połączone<Device Manager:Connecting to the Device Manager>` z Menedżerem Urządzenia.

1. Wybierz :ref:`warstwę<Device Manager:Layer Selector>`, na której chcesz zmienić przypisanie klawisza.

2. Kliknij klawisz, który chcesz zmienić. Otworzy się wówczas
   :ref:`menu kodów akcji<Device Manager:Action Code Menu>`.

3. Skorzystaj z wyszukiwarki w :ref:`menu kodów akcji<Device Manager:Action Code Menu>`
   lub przeglądaj dostępne :ref:`kody akcji<Device Manager:What are Action Codes>`.
   Po znalezieniu odpowiedniego :ref:`kodu akcji<Device Manager:Using Action Codes>`, kliknij go.

    Po wybraniu :ref:`kodu akcji<Device Manager:Using Action Codes>`, zobaczysz, że
    diagram układu odzwierciedla teraz wybrany
    :ref:`kod akcji<Device Manager:Using Action Codes>` podświetlony zgodnie z Twoim
    :ref:`schematem kolorów<Device Manager:Color Scheme>`, a obok pojawi się
    unosząca się kropka.

    .. Tip::
        Możesz edytować wiele klawiszy przed :ref:`zapisaniem<Device Manager:Save Button>` zmian.
        Przełączanie się między :ref:`warstwami<Device Manager:Layer Selector>` nie anuluje zmian
        dokonanych w układzie.

4. Gdy skończysz przypisywanie klawiszy, kliknij :ref:`przycisk zapisu<Device Manager:Save Button>`.

    .. note::
        Twoje zmiany nie zostaną zastosowane, dopóki nie klikniesz :ref:`zapisz<Device Manager:Save Button>`.

    Po kliknięciu :ref:`zapisz<Device Manager:Save Button>`, podświetlenie klawiszy zniknie,
    a unosząca się kropka zostanie usunięta. Diagram układu stanie się ponownie czarno-biały.

.. _Device Manager:Using Action Codes:

Używanie kodów akcji
~~~~~~~~~~~~~~~~~~~

Możesz używać kodów akcji zarówno w :ref:`wyjściach akordów<Chords:Chord Output>`, jak i podczas
:ref:`przypisywania<Device Manager:Remapping>` klawiszy.

.. _Device Manager:What are Action Codes:

Czym są kody akcji
^^^^^^^^^^^^^^^^^^^^^^^

Kody akcji to dane, które :doc:`CCOS<CCOS>` interpretuje jako znaki.
**Mówiąc prosto, są to znaki, które widzimy podczas pisania.**
Obejmują one litery, cyfry, znaki specjalne, klawisze funkcyjne i inne.

.. _Device Manager:Action Code Menu:

Menu kodów akcji
^^^^^^^^^^^^^^^^^^^^^^^

Menu kodów akcji możesz otworzyć na dwa sposoby:

1. Podczas wpisywania :ref:`wyjścia akordu<Chords:Chord Output>` w
   :ref:`bibliotece<Device Manager:Library>`, zauważysz nad kursorem
   bańkę z ``+``. Kliknij ją, aby otworzyć menu kodów akcji.

2. Podczas edycji układu w :ref:`edytorze układu<Device Manager:Layout>`,
   kliknij dowolny klawisz, aby wywołać menu kodów akcji.

W menu możesz przeglądać :ref:`dostępne kody akcji<Device Manager:Available Action Codes>`
według :ref:`kategorii<Device Manager:Action Code Categories>`, lub wyszukiwać konkretne akcje.

Jeżeli chcesz zamknąć menu kodów akcji, kliknij ikonę X w prawym górnym rogu menu.
Spowoduje to zamknięcie okna bez wprowadzania zmian.

.. _Device Manager:Action Code Categories:

Kategorie kodów akcji
..........................

Istnieje osiem kategorii w menu kodów akcji:

- Makra ASCII
- ASCII
- CharaChorder One
- CharaChorder
- CP-1252
- Klawiatura
- Mysz
- Kody klawiszy

Przycisk Usuń
................

Możesz skorzystać z przycisku "Usuń" w prawym górnym rogu menu kodów akcji, aby usunąć aktualnie
przypisany kod akcji dla wybranego klawisza w :ref:`edytorze układu<Device Manager:Layout>`.

Jeżeli wybierzesz "Usuń" podczas wpisywania :ref:`wyjścia akordu<Chords:Chord Output>` w
:ref:`bibliotece<Device Manager:Library>`, nie usunie to akcji, lecz doda "pustą" akcję
oznaczoną jako ``0x0``.

.. _Device Manager:Available Action Codes:

Dostępne kody akcji
^^^^^^^^^^^^^^^^^^^^^^^

Poniżej możesz zobaczyć dostępne kody akcji, albo przejrzeć je zewnętrznie
`tutaj <https://docs.google.com/spreadsheets/d/1--T9bXshCIC-OVly-CY3rK87fgb7AHgJl3IySh7cmHc/edit#gid=0>`__.

.. raw:: html

    <iframe src="https://docs.google.com/spreadsheets/d/1--T9bXshCIC-OVly-CY3rK87fgb7AHgJl3IySh7cmHc/edit#gid=0" width="600" height="600"></iframe>
