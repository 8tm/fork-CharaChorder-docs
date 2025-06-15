.. _Generative Text Menu (GTM):

Menu Tekstu Generowanego (GTM)
=============================

``CharaChorder GTM [ >K<eyboard || >M<ouse || >C<hording || >D<isplay || >R<esources ]``

Menu Tekstu Generowanego, znane pod skrótem GTM, to wbudowane, tekstowe menu, do którego można
uzyskać dostęp wszędzie tam, gdzie można pisać. Za jego pomocą możemy modyfikować ustawienia
:doc:`CCOS<CCOS>`, w tym m.in.: :ref:`tolerancje akordowania<GenerativeTextMenu:Press Tolerance>`,
:ref:`prędkości myszy<GenerativeTextMenu:Slow Speed>` oraz
:ref:`informacje zwrotne w czasie rzeczywistym<GenerativeTextMenu:Realtime Feedback>`, a także
inne ustawienia i funkcje — bez potrzeby używania oprogramowania. Jest to podstawowa funkcja
:doc:`CCOS<CCOS>`, którą warto opanować, aby dostosować urządzenie do własnych potrzeb.

Zauważysz, że niektóre ustawienia mają osobne wartości dla naciśnięcia i zwolnienia. Wynika to z
faktu, że :doc:`CCOS<CCOS>` odczytuje stan przełączników w dwóch różnych momentach: gdy są naciskane
oraz gdy są zwalniane. Zaprojektowaliśmy :doc:`CCOS<CCOS>` tak, aby umożliwiał konfigurację ustawień
dla każdego z tych "zdarzeń" oddzielnie, dla maksymalnej możliwości dostosowania. Intuicyjnie, każde
ustawienie związane z **naciśnięciem**, takie jak :ref:`debounce press<GenerativeTextMenu:Debounce Press>`,
wpływa na sposób, w jaki :doc:`CCOS<CCOS>` odczytuje przełącznik w momencie jego naciśnięcia w dowolnym
kierunku. Analogicznie, ustawienia **zwolnienia**, takie jak
:ref:`debounce release<GenerativeTextMenu:Debounce Release>`, wpływają na sposób, w jaki
:doc:`CCOS<CCOS>` odczytuje przełącznik w momencie jego zwolnienia, czyli odpuszczenia naciśnięcia w
dowolnym kierunku.

.. note::
    Chociaż możesz konfigurować ustawienia CCOS wszędzie tam, gdzie możesz pisać za pomocą GTM, możesz je
    również edytować w :doc:`CharaChorder Device Manager<Device Manager>`.

.. warning::
    Należy pamiętać, że aktualizacja urządzenia CCOS może zresetować ustawienia GTM do wartości domyślnych.
    Upewnij się, że posiadasz :ref:`kopię zapasową ustawień GTM<Device Manager:Creating a Backup>` przed
    aktualizacją urządzenia CCOS. Instrukcje dotyczące przywracania kopii zapasowych znajdują się w sekcji
    :ref:`Przywracanie z kopii zapasowej<Device Manager:Restoring from a Backup>`.

.. contents:: Spis treści tej strony
   :local:

.. _GenerativeTextMenu:How to access the GTM:

Jak uzyskać dostęp do GTM
*********************

Najpierw przesuń kursor do dowolnego obszaru, w którym możesz pisać. Dla najlepszych rezultatów zalecamy
wybrać takie pole tekstowe, które nie formatuje automatycznie tekstu, ponieważ niektóre klawisze
wykorzystywane przez GTM mogą wywoływać niepożądane formatowanie. Zalecamy użycie prostego edytora
tekstu, takiego jak Notepad. Należy jednak pamiętać, że w Notepadzie systemu Windows mogą występować
problemy z wyświetlaniem GTM na komputerach z Windows 11.

Skorzystaj z poniższej tabeli, aby dowiedzieć się, jak wywołać GTM na swoim urządzeniu CCOS. Należy pamiętać,
że wywołanie GTM wymaga wykonania akcji ":doc:`akordowania<Chords>`".

.. csv-table::
    :header: "Urządzenie", "Jak uzyskać dostęp"

    "CharaChorder One", "Akorduj oba małe palce na północ (klawisze ``Alt``)"
    "CharaChorder Lite", "Akorduj ``G`` i środkowy klawisz ``Alt`` (klawisz ``Dup``)"
    "CharaChorder X", "Akorduj ``G`` i klawisz ``Esc``"
    "CharaChorder Engine", "Akorduj ``G`` i klawisz ``Esc``"

.. _GenerativeTextMenu:How to navigate through the GTM:

Jak poruszać się po GTM
*******************************

GTM posiada różne podmenu, które nazywamy „stronami”. Każda „strona” GTM zawiera różne opcje, które mogą
umożliwiać dostosowanie konkretnego ustawienia lub przenosić do kolejnego podmenu.

Po wykonaniu akordu wywołującego menu, :doc:`CCOS<CCOS>` wypisze na ekranie menu i dostępne opcje.
Będzie to wyglądać w następujący sposób:

``CharaChorder GTM [ >K<eyboard || >M<ouse || >C<hording || >D<isplay || >R<esources ]``

Nawigacja po tym menu opiera się na naciskaniu liter. W powyższym przykładzie, aby wybrać żądane podmenu,
należy nacisnąć literę znajdującą się w nawiasach kątowych (na przykład: ``>K<``) na swoim urządzeniu
:doc:`CCOS<CCOS>`. W powyższym przykładzie należy nacisnąć ``K`` dla Klawiatury, ``M`` dla Myszy, ``A``
dla Akordowania, ``W`` dla Wyświetlania oraz ``Z`` dla Zasobów.
Aby wrócić do poprzedniego menu, naciśnij strzałkę w lewo. Aby w dowolnym momencie opuścić GTM, naciśnij
``ESC``. Wyjście z GTM za pomocą ``ESC`` spowoduje zapisanie wprowadzonych zmian. Możesz także potwierdzić
zmiany, naciskając ``ENTER``.

W niektórych podmenu pojawią się wartości liczbowe. Aby je zwiększać lub zmniejszać, możesz używać klawiszy
strzałek góra/dół na swoim urządzeniu :doc:`CCOS<CCOS>`.

	``CharaChorder > Chording > Press Tolerance [ Use up/down arrow keys to adjust: 25ms ]``

.. _GenerativeTextMenu:Available Menus:

Dostępne menu
***************

.. csv-table::
    :header: "Menu", "Opis"

    ":ref:`Klawiatura<GenerativeTextMenu:Keyboard>`", "Ustawienia związane z obsługą wprowadzania znaków na urządzeniu"
    ":ref:`Mysz<GenerativeTextMenu:Mouse>`", "Ustawienia związane z obsługą funkcji myszy na urządzeniu"
    ":ref:`Akordowanie<GenerativeTextMenu:Chording>`", "Ustawienia związane z akordowaniem na urządzeniu"
    ":ref:`Wyświetlanie<GenerativeTextMenu:Display>`", "Ustawienia dotyczące wersji urządzenia i innych tekstów CCOS"
    ":ref:`Zasoby<GenerativeTextMenu:Resources>`", "Menu zasobów, głównie linki"

.. _GenerativeTextMenu:Keyboard:

Klawiatura
--------

W tym menu możesz modyfikować ustawienia dotyczące sposobu, w jaki Twoje urządzenie CCOS współpracuje z komputerem.

.. _GenerativeTextMenu:Scan Rate:

Częstotliwość skanowania
~~~~~~~~~

``Path: GTM > Keyboard > Scan Rate``

Częstotliwość skanowania, czasami nazywana „czasem skanowania klawiszy”, odnosi się do częstotliwości, z
jaką urządzenie sprawdza stan klawiszy wejściowych.
Dla odniesienia: 5 ms odpowiada 200 Hz, co oznacza, że :doc:`CCOS<CCOS>` sprawdza pozycję klawiszy co 5
milisekund, czyli 200 razy na sekundę. Niższa wartość zwykle jest lepsza, ponieważ zwiększa responsywność
CCOS, choć przy niskich wartościach różnice są zazwyczaj minimalne. W GTM to ustawienie jest regulowane w
jednostkach milisekund (ms).

Domyślne wartości częstotliwości skanowania dla różnych urządzeń CharaChorder przedstawiono w poniższej tabeli:

+------------------+------------------+--------------+--------------+-----------+
| Urządzenie       | Wartość domyślna | Min. wartość | Max. wartość | Przyrosty |
+==================+==================+==============+==============+===========+
| CharaChorder One | 2 ms             | 0 ms         | 20 ms        | 1 ms      |
+------------------+------------------+--------------+--------------+-----------+
| CharaChorder Lite| 2 ms             | 0 ms         | 20 ms        | 1 ms      |
+------------------+------------------+--------------+--------------+-----------+
| CharaChorder X   | 2 ms             | 0 ms         | 20 ms        | 1 ms      |
+------------------+------------------+--------------+--------------+-----------+

.. _GenerativeTextMenu:Debounce Press:

Odbijanie (naciśnięcie)
~~~~~~~~~~~~~~

``Path: GTM > Keyboard > Debounce Press``

Ustawienie odbijania (naciśnięcie) odnosi się do przedziału czasowego (mierzonego w milisekundach), w którym
:doc:`CCOS<CCOS>` odfiltrowuje powtórne aktywacje klawisza podczas zdarzenia naciśnięcia. Innymi słowy,
wszelkie powtórne aktywacje w danym przedziale czasu będą liczone jako jedno naciśnięcie.

Należy dostosować to ustawienie, jeśli podczas pisania pojawiają się niezamierzone podwójne znaki.
Zwiększenie tej wartości zmniejszy prawdopodobieństwo pojawienia się niechcianych podwójnych znaków,
ponieważ nakazuje :doc:`CCOS<CCOS>` poczekać dłużej przed przyjęciem kolejnego naciśnięcia w tym
samym kierunku przełącznika. Jednak ustawienie tej wartości zbyt wysoko może spowodować problemy
z odczytywaniem zamierzonych podwójnych naciśnięć, dlatego zaleca się testowanie różnych wartości
małymi krokami. Ustawienie to powinno być dostosowywane razem z parametrem
:ref:`odbicia (zwolnienia)<GenerativeTextMenu:Debounce Release>`.

Domyślne wartości odbijania (naciśnięcie) dla różnych urządzeń CharaChorder przedstawiono w tabeli:


+------------------+------------------+--------------+--------------+---------------+
| Urządzenie       | Wartość domyślna | Min. wartość | Max. wartość | Przyrosty     |
+==================+==================+==============+==============+===============+
| CharaChorder One | 7 ms             | 0 ms         | 100 ms       | 1 ms          |
+------------------+------------------+--------------+--------------+---------------+
| CharaChorder Lite| 12 ms            | 0 ms         | 100 ms       | 1 ms          |
+------------------+------------------+--------------+--------------+---------------+
| CharaChorder X   | 1 ms             | 0 ms         | 100 ms       | 1 ms          |
+------------------+------------------+--------------+--------------+---------------+

.. _GenerativeTextMenu:Debounce Release:

Odbijanie (zwolnienie)
~~~~~~~~~~~~~~~~

``Path: GTM > Keyboard > Debounce Release``

Ustawienie odbijania (zwolnienie) odnosi się do przedziału czasowego (mierzonego w milisekundach), w
którym :doc:`CCOS<CCOS>` odfiltrowuje powtórne aktywacje klawisza podczas zdarzenia zwolnienia.
Innymi słowy, wszelkie powtórne aktywacje w danym przedziale czasu będą liczone jako jedno zwolnienie.

Należy dostosować to ustawienie, jeśli podczas pisania pojawiają się niezamierzone podwójne znaki.
Zwiększenie tej wartości zmniejszy prawdopodobieństwo pojawienia się niechcianych podwójnych znaków,
ponieważ nakazuje :doc:`CCOS<CCOS>` poczekać dłużej przed przyjęciem kolejnego zwolnienia w tym samym
kierunku przełącznika. Jednak ustawienie tej wartości zbyt wysoko może spowodować problemy z
odczytywaniem zamierzonych podwójnych zwolnień, dlatego zaleca się testowanie różnych wartości
małymi krokami. Ustawienie to powinno być dostosowywane razem z parametrem
:ref:`odbicia (naciśnięcia)<GenerativeTextMenu:Debounce Press>`.

Domyślne wartości odbijania (zwolnienie) dla różnych urządzeń CharaChorder przedstawiono w tabeli:

+------------------+------------------+--------------+--------------+---------------+
| Urządzenie       | Wartość domyślna | Min. wartość | Max. wartość | Przyrosty     |
+==================+==================+==============+==============+===============+
| CharaChorder One | 7 ms             | 0 ms         | 100 ms       | 1 ms          |
+------------------+------------------+--------------+--------------+---------------+
| CharaChorder Lite| 12 ms            | 0 ms         | 100 ms       | 1 ms          |
+------------------+------------------+--------------+--------------+---------------+
| CharaChorder X   | 1 ms             | 0 ms         | 100 ms       | 1 ms          |
+------------------+------------------+--------------+--------------+---------------+

.. _GenerativeTextMenu:Keystroke Delay:

Opóźnienie naciśnięcia klawisza
~~~~~~~~~~~~~~~

``Path: GTM > Keyboard > Keystroke Delay``

To ustawienie dodaje niewielkie opóźnienie do wprowadzania naciśnięć klawiszy.
Jest mierzone w mikrosekundach (μs) i domyślnie jest bardzo małe.

Powinieneś zwiększyć tę wartość, jeśli Twój komputer nie przyjmuje wszystkich znaków wysyłanych przez
Twoje urządzenie, na przykład podczas korzystania z GTM. Jeśli występuje taki problem, Twoje GTM może
wyglądać dziwnie, z brakującymi fragmentami lub znakami.

Jeśli masz szybszy komputer, możesz zmniejszyć tę wartość, aby akordowanie i GTM działały szybciej i
bardziej responsywnie.

Wartość ta jest regulowana w przyrostach po 40 μs. Domyślne wartości opóźnienia naciśnięcia klawisza
dla różnych urządzeń CharaChorder przedstawiono w tabeli:

+------------------+------------------+--------------+---------------+--------------+
| Urządzenie       | Wartość domyślna | Min. wartość | Max. wartość  | Przyrosty    |
+==================+==================+==============+===============+==============+
| CharaChorder One | 480 μs           | 0 μs         | 10200 μs      | 40 μs        |
+------------------+------------------+--------------+---------------+--------------+
| CharaChorder Lite| 480 μs           | 0 μs         | 10200 μs      | 40 μs        |
+------------------+------------------+--------------+---------------+--------------+
| CharaChorder X   | 480 μs           | 0 μs         | 10200 μs      | 40 μs        |
+------------------+------------------+--------------+---------------+--------------+

.. _GenerativeTextMenu:Capslock:

Capslock
~~~~~~~~

``Path: GTM > Keyboard > Capslock``

To ustawienie działa podobnie do funkcji Capslock na komputerze: przełącza stan wielkich liter.
Gdy jest włączone, wszystkie litery wprowadzane przez urządzenie CCOS będą pisane wielkimi literami.
Gdy jest wyłączone, wszystkie litery będą pisane małymi literami.

.. _GenerativeTextMenu:Operating System:

System operacyjny
~~~~~~~~~~~~~~~~

``Path: GTM > Keyboard > Operating System``

To ustawienie odnosi się do systemu operacyjnego komputera, do którego podłączone jest Twoje urządzenie.
Ponieważ układy klawiszy na różnych systemach operacyjnych mogą się różnić, możesz skonfigurować swoje
urządzenie CCOS tak, aby odpowiadało Twojemu systemowi.

Obecnie w CCOS możesz wybrać pomiędzy Windows, Mac, Linux, iOS lub Android.

Celem tego ustawienia jest zapewnienie dokładniejszego mapowania klawiszy.
Dlatego zaleca się ustawienie wartości odpowiadającej systemowi operacyjnemu używanemu na komputerze,
do którego podłączone jest Twoje urządzenie CCOS.

.. csv-table::
    :header: "Urządzenie", "Domyślnie"

    "CharaChorder One", "Windows"
    "CharaChorder Lite", "Windows"
    "CharaChorder X", "Windows"

.. Warning::
    Na dzień grudnia 2023 roku to ustawienie nie wpływa na działanie urządzeń CCOS.

.. _GenerativeTextMenu:GUI-CTRL Soft Swap:

GUI-CTRL Soft Swap (tylko CharaChorder Lite)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

``Path: GTM > Keyboard > GUI-CTRL Soft Swap``

To ustawienie zamienia funkcje dwóch klawiszy w lewym dolnym rogu urządzenia CharaChorder Lite.

Tradycyjne klawiatury QWERTY mają klawisz ``CTRL`` w lewym dolnym rogu, a obok niego klawisz ``GUI``
(Command na Macu, Windows na Windowsie, Super na Linuksie itd.). Domyślnie CharaChorder Lite ma te
klawisze zamienione miejscami, co dla niektórych użytkowników jest niewygodne i trudne do przyzwyczajenia.
Fabrycznie nowe urządzenie CharaChorder Lite ma klawisz ``GUI`` w lewym dolnym rogu, a ``CTRL`` po jego
prawej stronie.

Za pomocą tego ustawienia możesz zamienić te klawisze na poziomie CCOS, tak aby ``CTRL`` znajdował się
w lewym dolnym rogu.

Ustawienie to ma dwie opcje: GUI-CTRL oraz CTRL-GUI. Domyślnie ustawione jest GUI-CTRL.

**Domyślne mapowanie klawiszy:**

.. _GUI-CTRL:
.. image:: /assets/images/GUI-CTRL.jpg
  :width: 1200
  :alt: Domyślne mapowanie CTRL w CharaChorder Lite

**Mapowanie klawiszy po zamianie:**

.. _CTRL-GUI:
.. image:: /assets/images/CTRL-GUI.jpg
  :width: 1200
  :alt: Alternatywne mapowanie CTRL w CharaChorder Lite

Użytkownicy przyzwyczajeni do tradycyjnego układu klawiatur będą chcieli skorzystać z tego ustawienia,
aby nie musieć uczyć się nowego położenia tych klawiszy.

.. _GenerativeTextMenu:Mouse:

Mysz
-----

CCOS umożliwia używanie urządzenia jako myszy, włącznie z funkcjami przewijania i poruszania kursorem.
W tej sekcji omówione są ustawienia związane z funkcją myszy na urządzeniach CCOS.

.. _GenerativeTextMenu:Poll Rate:

Częstotliwość odpytywania
~~~~~~~~~

``Path: GTM > Mouse > Poll Rate``

Częstotliwość odpytywania (poll rate) to częstotliwość, z jaką dane z funkcji myszy w CharaChorder są
wysyłane do podłączonego urządzenia. Innymi słowy — jak często pozycja kursora jest aktualizowana na
komputerze. Zazwyczaj wyraża się ją w Hz (hercach); na przykład standardowa mysz gamingowa odświeża
dane 1000 razy na sekundę (1000 Hz).

Jednak :doc:`CCOS<CCOS>` używa jednostki ms (milisekundy), która jest odwrotnością Hz. 1 ms odpowiada
1000 Hz, 2 ms to 500 Hz, a 1000 ms to 1 Hz.

 .. dropdown:: Wyjaśnienie konwersji Hz na ms

    W kontekście częstotliwości i okresu (czasu trwania cyklu) zależność jest odwrotna.
    Częstotliwość to liczba cykli na sekundę (Hz). Okres to czas trwania jednego cyklu (s). Wzór to:

    ``Częstotliwość (Hz) = 1 / Okres (s), gdzie s = 1000 ms``

    Po przeliczeniu na milisekundy (ms) zależność pozostaje odwrotna. Na przykład częstotliwość 1000 Hz
    oznacza okres 1 ms (bo 1 s = 1000 ms). Im wyższa częstotliwość, tym krótszy okres (w ms).

Domyślne wartości dla każdego urządzenia przedstawiono w tabeli poniżej:

.. csv-table::
    :header: "Urządzenie", "Domyślnie", "Min. wartość", "Max. wartość", "Przyrosty"

    "CharaChorder One", "20 ms", "0 ms", "100 ms", "1 ms (Hz)"
    "CharaChorder Lite", "20 ms", "0 ms", "100 ms", "1 ms (Hz)"
    "CharaChorder X", "20 ms", "0 ms", "100 ms", "1 ms (Hz)"

To ustawienie współpracuje z parametrami :ref:`wolna prędkość<GenerativeTextMenu:Slow Speed>` i
:ref:`szybka prędkość<GenerativeTextMenu:Fast Speed>`. Oba —
:ref:`wolna prędkość<GenerativeTextMenu:Slow Speed>` oraz
:ref:`szybka prędkość<GenerativeTextMenu:Fast Speed>` — zależą od częstotliwości odpytywania.

.. _GenerativeTextMenu:Slow Speed:

Wolna prędkość
~~~~~~~~~~

``Path: GTM > Mouse > Slow Speed``

Wolna prędkość aktywuje się, gdy używasz tylko jednego klawisza myszy w danym kierunku (w przeciwieństwie
do używania dwóch klawiszy w tym samym kierunku). Zwiększenie tej wartości spowoduje szybsze przesuwanie
wskaźnika CCOS.

To ustawienie współpracuje z parametrem :ref:`częstotliwości odpytywania<GenerativeTextMenu:Poll Rate>`.
Wyjaśnienie poniżej:

.. dropdown:: Wyjaśnienie prędkości myszy CCOS

    Prędkość myszy określa szybkość przesuwania kursora w funkcji myszy CharaChorder. Kursor będzie przesuwał
    się o liczbę pikseli (px) wskazaną przez to ustawienie, pomnożoną przez częstotliwość odpytywania
    :ref:`poll rate<GenerativeTextMenu:Poll Rate>` (wyrażoną w Hz).

    Innymi słowy, jeśli prędkość ustawisz na 2 px, a :ref:`poll rate<GenerativeTextMenu:Poll Rate>` wynosi
    20 ms (~50 Hz), kursor CharaChorder przesunie się o 100 pikseli na sekundę (px/s). Wzór:

    ``Prędkość (px) x poll rate (Hz) = liczba pikseli przesuwu na sekundę``

Domyślne wartości dla każdego urządzenia przedstawiono w tabeli poniżej:

.. csv-table::
    :header: "Urządzenie", "Domyślnie", "Min. wartość", "Max. wartość", "Przyrosty"

    "CharaChorder One", "5 px", "0 px", "250 px", "1 px"
    "CharaChorder Lite", "16 px", "0 px", "250 px", "1 px"
    "CharaChorder X", "16 px", "0 px", "250 px", "1 px"

.. _GenerativeTextMenu:Fast Speed:

Szybka prędkość
~~~~~~~~~~

``Path: GTM > Mouse > Fast Speed``

Szybka prędkość aktywuje się, gdy używasz dwóch klawiszy myszy w tym samym kierunku (w przeciwieństwie
do używania tylko jednego klawisza w danym kierunku). Zwiększenie tej wartości spowoduje szybsze
przesuwanie wskaźnika CCOS.

To ustawienie współpracuje z parametrem :ref:`częstotliwości odpytywania<GenerativeTextMenu:Poll Rate>`.
Wyjaśnienie poniżej:

.. dropdown:: Wyjaśnienie prędkości myszy CCOS

    Prędkość myszy określa szybkość przesuwania kursora w funkcji myszy CharaChorder.
    Kursor będzie przesuwał się o liczbę pikseli (px) wskazaną przez to ustawienie,
    pomnożoną przez częstotliwość odpytywania :ref:`poll rate<GenerativeTextMenu:Poll Rate>` (wyrażoną w Hz).

    Innymi słowy, jeśli prędkość ustawisz na 2 px, a :ref:`poll rate<GenerativeTextMenu:Poll Rate>`
    wynosi 20 ms (~50 Hz), kursor CharaChorder przesunie się o 100 pikseli na sekundę (px/s). Wzór:

    ``Prędkość (px) x poll rate (Hz) = liczba pikseli przesuwu na sekundę``

Domyślne wartości dla każdego urządzenia przedstawiono w tabeli poniżej:

.. csv-table::
    :header: "Urządzenie", "Domyślnie", "Min. wartość", "Max. wartość", "Przyrosty"

    "CharaChorder One", "25 px", "0 px", "250 px", "1 px"
    "CharaChorder Lite", "32 px", "0 px", "250 px", "1 px"
    "CharaChorder X", "32 px", "0 px", "250 px", "1 px"

.. _GenerativeTextMenu:Scroll Speed:

Prędkość przewijania
~~~~~~~~~~~~

``Path: GTM > Mouse > Scroll Speed``

Prędkość przewijania odnosi się do szybkości przewijania w urządzeniu CCOS.

Zwiększenie tej wartości spowoduje szybsze przewijanie przez urządzenie CCOS.
To ustawienie współpracuje z parametrem :ref:`częstotliwości odpytywania<GenerativeTextMenu:Poll Rate>`.
Wyjaśnienie poniżej:

.. dropdown:: Wyjaśnienie prędkości myszy CCOS

    Prędkość przewijania określa szybkość przewijania przez urządzenie CharaChorder.
    CCOS będzie przewijać o liczbę pikseli (px) wskazaną przez to ustawienie, pomnożoną przez
    częstotliwość odpytywania :ref:`poll rate<GenerativeTextMenu:Poll Rate>` (wyrażoną w Hz).

    Innymi słowy, jeśli prędkość ustawisz na 2 px, a :ref:`poll rate<GenerativeTextMenu:Poll Rate>`
    wynosi 20 ms (~50 Hz), przewijanie CharaChorder nastąpi z prędkością 100 pikseli na sekundę (px/s). Wzór:

    ``Prędkość (px) x poll rate (Hz) = liczba pikseli przewiniętych na sekundę``

Domyślne wartości dla każdego urządzenia przedstawiono w tabeli poniżej:

.. csv-table::
    :header: "Urządzenie", "Domyślnie", "Min. wartość", "Max. wartość", "Przyrosty"

    "CharaChorder One", "2 px", "0 px", "25 px", "1 px"
    "CharaChorder Lite", "2 px", "0 px", "25 px", "1 px"
    "CharaChorder X", "2 px", "0 px", "25 px", "1 px"

.. _GenerativeTextMenu:Active Mode:

Tryb aktywny
~~~~~~~~~~~

``Path: GTM > Mouse > Active Mode``

Tryb aktywny przesuwa kursor myszy o jeden piksel mniej więcej co minutę (czas nie jest dokładnie określony).
Ustawienie to może być użyte do zapobiegania przechodzeniu komputera w tryb uśpienia.
Możesz wyłączyć to ustawienie, jeśli zauważysz, że aplikacje na komputerze blokują powiadomienia na
urządzeniach mobilnych (na przykład w Discordzie lub Microsoft Teams).

.. _GenerativeTextMenu:Chording:

Akordowanie
--------

Urządzenia CCOS oferują możliwość :doc:`akordowania<Chords>`.
Poniższe ustawienia wpływają na działanie akordowania na urządzeniu.

.. _GenerativeTextMenu:Character Only Mode:

Tryb tylko znaki
~~~~~~~~~~~~~~~~~~~

``Path: GTM > Chording > Character Only Mode``

To ustawienie jest przełącznikiem, który wyłącza funkcje akordowania na urządzeniach CCOS.
Domyślnie jest wyłączone, ale można je włączyć w przypadku, gdy nie chcemy w ogóle korzystać z akordowania.
Ustawienie to może być przydatne w sytuacjach, w których przypadkowe wywołanie akordów mogłoby
przeszkadzać — na przykład podczas grania w gry.

Jeżeli Twoje urządzenie CCOS nagle przestanie reagować na akordy, warto sprawdzić, czy to ustawienie
nie zostało przypadkiem włączone.

.. _GenerativeTextMenu:Press Tolerance:

Tolerancja naciśnięcia
~~~~~~~~~~~~~~~

``Path: GTM > Chording > Press Tolerance``

Tolerancja naciśnięcia określa przedział czasowy, w którym akord może zostać wykonany, mierzony w
milisekundach (ms). Licznik uruchamia się po pierwszym „naciśnięciu” pierwszego klawisza w akordzie i
kończy, gdy naciśnięty zostanie ostatni klawisz akordu lub gdy czas tolerancji się skończy — w
zależności, co nastąpi pierwsze.

.. _Tolerancje:

.. image:: /assets/images/Press-and-Release-Tolerances.png
  :width: 1200
  :alt: Diagram wyjaśniający tolerancje

Mówiąc prosto: zwiększenie tolerancji naciśnięcia (często wykonywane razem ze zwiększeniem
:ref:`tolerancji zwolnienia<GenerativeTextMenu:Release Tolerance>`) ułatwia wykonywanie akordów.

.. note::
    Tolerancja naciśnięcia skaluje się (zwiększa) wraz z liczbą klawiszy w akordzie.
    Okno czasowe będzie większe przy 6-klawiszowym akordzie niż przy 3-klawiszowym.
    Oznacza to, że choć ustawisz konkretną wartość, w rzeczywistości będzie ona
    wydłużona w zależności od liczby klawiszy w akordzie.

Możesz zwiększyć to ustawienie, aby wydłużyć okno czasowe i ułatwić wykonywanie akordów.

Minusem ustawienia wyższych wartości jest możliwość przypadkowego wyzwalania akordów podczas
zwykłego wprowadzania znaków. Dlatego, jeśli zauważasz przypadkowe uruchamianie akordów, warto
obniżyć tę wartość oraz :ref:`tolerancję zwolnienia<GenerativeTextMenu:Release Tolerance>`.

Domyślne wartości dla każdego urządzenia przedstawiono w tabeli:

.. csv-table::
    :header: "Urządzenie", "Domyślnie", "Min. wartość", "Max. wartość", "Przyrosty"

    "CharaChorder One", "25 ms", "0 ms", "150 ms", "1 ms"
    "CharaChorder Lite", "25 ms", "0 ms", "150 ms", "1 ms"
    "CharaChorder X", "25 ms", "0 ms", "150 ms", "1 ms"

.. _GenerativeTextMenu:Release Tolerance:

Tolerancja zwolnienia
~~~~~~~~~~~~~~~~~

``Path: GTM > Chording > Release Tolerance``

Tolerancja zwolnienia odnosi się do przedziału czasowego, w którym akord może zostać wykonany, mierzony
w milisekundach (ms). Licznik uruchamia się w momencie pierwszego „zwolnienia” któregokolwiek klawisza
w akordzie i kończy, gdy akord zostanie w pełni wykonany lub gdy czas tolerancji się skończy — w
zależności co nastąpi pierwsze.

.. image:: /assets/images/Press-and-Release-Tolerances.png
  :width: 1200
  :alt: Diagram wyjaśniający tolerancje

Mówiąc prosto: zwiększenie tolerancji zwolnienia (często wykonywane razem ze zwiększeniem
:ref:`tolerancji naciśnięcia<GenerativeTextMenu:Press Tolerance>`) ułatwia wykonywanie akordów.

.. note::
    Tolerancja naciśnięcia skaluje się (zwiększa) wraz z liczbą klawiszy w akordzie.
    Okno czasowe będzie większe przy 6-klawiszowym akordzie niż przy 3-klawiszowym.
    Oznacza to, że choć ustawisz konkretną wartość, w rzeczywistości będzie ona
    wydłużona w zależności od liczby klawiszy w akordzie.

Możesz zwiększyć to ustawienie, aby wydłużyć okno czasowe i ułatwić wykonywanie akordów.

Minusem ustawienia wyższych wartości jest możliwość przypadkowego wyzwalania akordów podczas
zwykłego wprowadzania znaków. Dlatego, jeśli zauważasz przypadkowe uruchamianie akordów, warto
obniżyć tę wartość oraz :ref:`tolerancję naciśnięcia<GenerativeTextMenu:Press Tolerance>`.

Domyślne wartości dla każdego urządzenia przedstawiono w tabeli:

.. csv-table::
    :header: "Urządzenie", "Domyślnie", "Min. wartość", "Max. wartość", "Przyrosty"

    "CharaChorder One", "18 ms", "0 ms", "150 ms", "1 ms"
    "CharaChorder Lite", "18 ms", "0 ms", "150 ms", "1 ms"
    "CharaChorder X", "18 ms", "0 ms", "150 ms", "1 ms"

.. _GenerativeTextMenu:Timeout:

Timeout
~~~~~~~

``Path: GTM > Chording > Timeout``

To ustawienie określa, jak długo CCOS liczy czas w celu zastąpienia znaków, które poprzedzają akord.

Urządzenia CCOS posiadają działający licznik czasu, który uruchamia się po każdym wprowadzeniu
pojedynczego znaku w trybie klasycznego wprowadzania znaków (chentry — wprowadzanie znak po znaku).
Ten licznik kontroluje, czy następny wykonany akord usunie poprzedzające znaki.

Ta funkcja pozwala użytkownikom na poprawienie błędnie wykonanego akordu — wystarczy szybko wykonać
poprawny akord bez potrzeby ręcznego kasowania błędnych znaków. W efekcie timeout automatycznie
usuwa wszystkie poprzedzające znaki (aż do ostatniego :doc:`znaku przerywającego </Breaking Character>`)
i zastępuje je właściwym akordem.

Możesz ustawić tę wartość w zakresie od 0,0 sekundy (s) do 25,0 sekund (s), dostosowując ją do własnego stylu
:doc:`akordowania<Chords>`.

.. warning::
    Ustawienie tej wartości na 0,0 s spowoduje, że :doc:`akordy<Chords>` nie będą działały w ogóle.
    Będą się aktywować, ale nie usuną automatycznie :ref:`wejść akordu<Chord Input>`.

Domyślne wartości dla każdego urządzenia przedstawiono w tabeli:

.. csv-table::
    :header: "Urządzenie", "Domyślnie", "Min. wartość", "Max. wartość", "Przyrosty"

    "CharaChorder One", "4 s", "0 s", "25 s", "0.1 s"
    "CharaChorder Lite", "4 s", "0 s", "25 s", "0.1 s"
    "CharaChorder X", "4 s", "0 s", "25 s", "0.1 s"

.. _GenerativeTextMenu:Spurring:

Akordowanie natychmiastowe
~~~~~~~~

``Path: GTM > Chording > Spurring``

Tryb wyłącznie akordowy, w którym urządzenie wyprowadza akordy już w momencie naciśnięcia klawiszy,
zamiast czekać na naciśnięcie i zwolnienie. W trybie akordowania natychmiastowego możesz naciskać
klawisze akordu pojedynczo z dużo dłuższym czasem oczekiwania, co czyni go użytecznym dla osób
chcących ćwiczyć akordowanie bez konieczności przejmowania się
:ref:`dokładnym czasem<GenerativeTextMenu:Press Tolerance>`.

Akordowanie natychmiastowe umożliwia także przechodzenie z jednego akordu do następnego bez całkowitego
zwalniania wszystkich klawiszy. Może to znacząco zwiększyć szybkość akordowania, jednak kosztem
elastyczności wprowadzania pojedynczych znaków. Przy odpowiednio przygotowanej bibliotece akordów,
tryb ten pozwala na maksymalne zwiększenie szybkości pisania.

Akordowanie natychmiastowe — Włącz/Wyłącz
^^^^^^^^^^^^^^^

``Path: GTM > Chording > Character Only Mode > Spurring Timeout``

To ustawienie przełącza tryb akordowania natychmiastowego WŁĄCZONY lub WYŁĄCZONY.

.. _GenerativeTextMenu:Spurring Timeout:

Limit czasu akordowania natychmiastowego
^^^^^^^^^^^^^^^^

``Path: GTM > Chording > Spurring > Spurring Timeout``

Określa czas bezczynności, po którym urządzenie powróci do standardowego trybu akordowania/znakowego
(czyli wyłącza tryb akordowania natychmiastowego).

Domyślne wartości dla każdego urządzenia przedstawiono w tabeli:

.. csv-table::
    :header: "Urządzenie", "Domyślnie", "Min. wartość", "Max. wartość", "Przyrosty"

    "CharaChorder One", "240 s", "0 s", "250 s", "1 s"
    "CharaChorder Lite", "240 s", "0 s", "250 s", "1 s"
    "CharaChorder X", "240 s", "0 s", "250 s", "1 s"

.. _GenerativeTextMenu:Arpeggiate:

Arpeggiacja
~~~~~~~~~~

``Path: GTM > Chording > Arpeggiate``

Arpeggiacje to działania czasowe, które mogą modyfikować akord po jego wykonaniu.
Prostym przykładem jest zastosowanie modyfikatorów akordów po wykonaniu akordu.
Możesz przeczytać więcej w sekcji o :doc:`modyfikatorach akordów<Chord Modifiers>`.

Gdy arpeggiacje są włączone, możesz np. wykonać akord dla słowa ``run``, a następnie, w ramach
:ref:`okna czasowego arpeggiacji<GenerativeTextMenu:Arpeggiate Timeout>`, nacisnąć modyfikator
czasu przeszłego, aby przekształcić słowo w wariant czasu przeszłego — w języku angielskim: ``ran``.

Arpeggiacja — Włącz/Wyłącz
^^^^^^^^^^^^^^^^^

``Path: GTM > Chording > Arpeggiate > Arpeggiate On/Off``

To ustawienie pozwala włączyć lub wyłączyć funkcję arpeggiacji.

Niektórzy użytkownicy nie przepadają za arpeggiacją, ponieważ przy bardzo szybkiej pracy może
prowadzić do niezamierzonych modyfikacji.

.. _GenerativeTextMenu:Arpeggiate Timeout:

Limit czasu arpeggiacji
^^^^^^^^^^^^^^^^^^

``Path: GTM > Chording > Arpeggiate > Arpeggiate Timeout``

Limit czasu arpeggiacji to okno czasowe po wykonaniu akordu, w którym CCOS oczekuje na wykonanie arpeggiacji.
Po upływie tego czasu CCOS PRZESTAJE modyfikować wcześniejszy akord.

Typowym problemem, na jaki mogą natrafić użytkownicy przy włączonej arpeggiacji, jest to, że klawisz
Shift modyfikuje poprzedni akord zamiast wpływać na następny znak. Z tego powodu niektórzy użytkownicy
zmniejszają limit czasu arpeggiacji do bardzo małych wartości, aby ograniczyć ryzyko takich
niezamierzonych modyfikacji.

.. _GenerativeTextMenu:Display:

Wyświetlanie
-------

W tej sekcji znajdziesz ustawienia dotyczące sposobu, w jaki CharaChorder wyświetla określone informacje.

.. _GenerativeTextMenu:Version:

Wersja
~~~~~~~

``Path: GTM > Display > Version``

Chociaż nie jest to ustawienie, które można modyfikować, stanowi przydatną informację tekstową
pokazującą wersję CCOS, na której aktualnie działa Twoje urządzenie CharaChorder.
Możesz w ten sposób szybko sprawdzić wersję oprogramowania w dowolnym miejscu, w którym możesz
odczytać menu GTM.

.. _GenerativeTextMenu:Realtime Feedback:

Informacje w czasie rzeczywistym
~~~~~~~~~~~~~~~~~

``Path: GTM > Display > Realtime Feedback``

To ustawienie przełącza wyświetlanie informacji w czasie rzeczywistym WŁĄCZONE lub WYŁĄCZONE.

Informacje w czasie rzeczywistym odnoszą się do pomocniczych komunikatów, takich jak
``AKORDOWANIE_NATYCHMIASTOWE_WŁĄCZONE`` (SPURRING_ON), ``AKORDOWANIE_NATYCHMIASTOWE_WYŁĄCZONE`` (SPURRING_OFF)
itd., które informują użytkownika o aktywacji bądź dezaktywacji określonych trybów w urządzeniu CharaChorder.
Ponieważ nie istnieje inna wizualna informacja o tym, czy dany akord aktywował lub dezaktywował pewne
ustawienia, pomocne jest wyświetlanie takich komunikatów w formie potwierdzenia.

.. Note::
    Ustawienie informacji w czasie rzeczywistym kontroluje również
    :ref:`ustawienie uruchamiania<GenerativeTextMenu:Startup>`.
    Jeżeli informacje w czasie rzeczywistym są WYŁĄCZONE, to uruchamianie również będzie
    WYŁĄCZONE, bez względu na indywidualny stan tego ustawienia.

.. _GenerativeTextMenu:Startup:

Uruchamianie
~~~~~~~

``Path: GTM > Display > Startup``

Włączenie tego ustawienia powoduje, że po podłączeniu urządzenia do komputera zostanie wyświetlony komunikat
„CCOS is ready.”. Wiadomość ta pojawi się w miejscu, gdzie ostatnio znajdował się kursor, o ile okno z
możliwością wprowadzania tekstu jest aktywne. Ustawienie to jest przydatne, ponieważ informuje, że
urządzenie CharaChorder jest gotowe do pracy — ponieważ proces uruchamiania może potrwać kilka sekund.

Należy jednak pamiętać, że jeśli podczas podłączania CharaChorder masz zaznaczony tekst, komunikat
uruchamiania zastąpi zaznaczony fragment. Dodatkowo, jeżeli nie ma aktywnego okna do wprowadzania
tekstu, kody klawiszy wysyłane przez CharaChorder w celu wyświetlenia komunikatu startowego mogą
zostać przez komputer zinterpretowane jako akcje i skutkować niepożądanym zachowaniem.

Jeżeli nie chcesz, aby ten komunikat był wyświetlany za każdym razem po podłączeniu urządzenia,
możesz wyłączyć to ustawienie.

.. Warning::
    Ustawienie Uruchamiania zależy od
    :ref:`ustawienia informacji w czasie rzeczywistym<GenerativeTextMenu:Realtime Feedback>`.
    Jeżeli informacje w czasie rzeczywistym są WYŁĄCZONE, wówczas komunikat startowy nie
    zostanie wyświetlony, nawet jeśli opcja Uruchamiania jest WŁĄCZONA.

.. _GenerativeTextMenu:LEDs:

Diody LED (tylko CharaChorder Lite)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

``Path: GTM > Display > LEDs``

:doc:`CharaChorder Lite<CharaChorder_Lite>` posiada diody RGB, które podświetlają klawisze od spodu
światłem statycznym. W tej sekcji znajdują się ustawienia dotyczące tych diod LED.

.. note::
    Ustawienia LED dostępne są w GTM wyłącznie dla urządzeń :doc:`CharaChorder Lite<CharaChorder_Lite>`,
    nie dla innych modeli CharaChorder.

Włącz/Wyłącz
^^^^^^

``Path: GTM > Display > LEDs > On/Off``

Szybkie włączanie lub wyłączanie podświetlenia LED za pomocą tego ustawienia.

Kolor
^^^^^

``Path: GTM > Display > LEDs > Color``

To ustawienie pozwala zmienić kolor podświetlenia LED w CharaChorder Lite.
W GTM dostępnych jest 11 kolorów do wyboru, pokazanych w tabeli poniżej:

.. csv-table::
    :header: "Litera", "Kolor"

    "W", "Biały"
    "R", "Czerwony"
    "O", "Pomarańczowy"
    "Y", "Żółty"
    "L", "Limonkowy"
    "G", "Zielony"
    "C", "Cyjan"
    "B", "Niebieski"
    "V", "Fioletowy"
    "P", "Różowy"
    "M", "Wielokolorowy"

Należy pamiętać, że na grudzień 2023 roku diody NIE są indywidualnie adresowalne.
Ustawienie koloru zmienia kolor WSZYSTKICH diod jednocześnie.

Jasność
^^^^^^^^^^

``Path: GTM > Display > LEDs > Brightness``

To ustawienie pozwala regulować jasność podświetlenia LED w CharaChorder Lite.
Możesz ustawić wartość od 0 do 50, gdzie 0 oznacza całkowite wyłączenie diod, a 50 — maksymalną jasność.

Należy pamiętać, że diody NIE są indywidualnie adresowalne (stan na grudzień 2023).
Jasność dotyczy wszystkich diod równomiernie.

.. note::
    Jeżeli używasz słabego źródła zasilania USB lub portu, wysoka jasność LED może powodować problemy
    z zasilaniem CharaChorder Lite. Jeżeli zauważysz problemy z uruchamianiem lub stabilnością
    urządzenia, warto obniżyć to ustawienie.

Domyślne wartości dla CharaChorder Lite przedstawiono w tabeli:

.. csv-table::
    :header: "Urządzenie", "Domyślnie", "Min. wartość", "Max. wartość", "Przyrosty"

    "CharaChorder Lite", "5", "0", "50", "1"

.. _GenerativeTextMenu:Resources:

Zasoby
---------

``Path: GTM > Resources``

Ta sekcja zawiera łącza, które mogą być dla Ciebie pomocne. Łącza te obejmują:

.. csv-table::
    :header: "Litera", "Element", "Opis"

    "A", "O nas", "Otwiera https://www.charachorder.com/pages/about."
    "G", "Rozpocznij", "Otwiera https://www.charachorder.com/pages/get-started."
    "D", "Discord", "Zaproszenie na serwer Discord CharaChorder"
    "T", "Trening", "Otwiera https://iq-eq.io — nasze bezpłatne narzędzie do nauki pisania z prędkością myśli"
    "M", "Wiadomość do Riley’a", "Kopiuje adres e-mail Riley Keen (CEO CharaChorder) do schowka"
    "L", "Nauka akordów", "Otwiera listę startową akordów"
    "S", "Sprawdź aktualizacje systemu", "Otwiera stronę z aktualizacjami wersji CCOS"
