Master Forge
===================

Witamy w Oficjalnym przewodniku Master Forge.
Możesz wybrać poniższe linki, aby przejść do tematów, które uznasz za najbardziej istotne.

.. _M4G:
.. image:: /assets/images/M4G.webp
  :width: 1200
  :alt: The Master Forge

Pakiet Master Forge składa się z dwóch :ref:`digitizerów<Digitizers>`,
:ref:`mechanicznego łącznika mostowego<Master Forge:Mechanical Bridge Connector>`, który łączy oba,
oraz — w zależności od zakupionej wersji — dodatkowych :doc:`nakładek<Bolt-Ons>`
i :doc:`rozszerzeń<Add-Ons>`. W tej sekcji omówimy każdy z elementów zawartych w dowolnym z pakietów
Master Forge, niezależnie od konkretnej konfiguracji.

:ref:`Kliknij tutaj, aby przejść do przewodnika dla początkujących.<Master Forge:Getting Started>`

.. contents:: Spis treści tej strony
   :local:

Zawartość opakowania
**************

Części
-----

.. _Case:

.. _M4G Schema:
.. image:: /assets/images/M4G-Separated.webp
  :width: 1200
  :alt: Części M4G


Gdy po raz pierwszy otrzymasz swój pakiet Master Forge, będzie on dostarczony w kartonowym pudełku.
Po jego otwarciu znajdziesz swojego nowego Master Forge w taktycznej walizce transportowej.
Znajdziesz tam również wkładkę zawierającą schemat urządzenia i niektóre funkcje, które posiada Master Forge.

.. _M4G Case:
.. image:: /assets/images/Case.webp
  :width: 1200
  :alt: Oryginalna walizka dla wspierających

Po otwarciu walizki spotkasz swój lśniący, nowy Master Forge. Master Forge składa się z dwóch digitizerów
z ośmioma pięciokierunkowymi przełącznikami, połączonych za pomocą
:ref:`mechanicznego łącznika mostowego<Master Forge:Mechanical Bridge Connector>`.

.. _Master Forge:The Digitizers:

Digitizery
~~~~~~~~~~~~~~~

Twoje urządzenie będzie zawierać dwa digitizery, które razem tworzą Master Forge. Każdy digitizer odpowiada
jednej ręce i został zaprojektowany z myślą o ergonomii i komforcie każdej dłoni. Digitizery składają się z
wydrukowanego w 3D endoszkieletu i obrabianego maszynowo aluminiowego egzoszkieletu. Egzoszkielet digitizera
składa się faktycznie z dwóch części: trapezoidalnej „powłoki” i płaskiej, częściowo wydrążonej
„płyty bazowej”. Są one połączone pięcioma śrubami M2 typu Philips, które znajdują się pod gumowymi
podkładkami ("stopkami") urządzenia. Podkładki te są okrągłe, gumowane i pomagają urządzeniu utrzymywać
stabilność na biurkach i innych gładkich powierzchniach.

Istnieją dwa różne typy digitizerów, z których każdy można zakupić osobno: lewy digitizer i prawy digitizer.
Każdy z nich zawiera :doc:`Platinum CharaChorder Core<CharaChorder Core>`, w którym przechowywane są
akordy, układy i ustawienia.

Na przedniej stronie każdego digitizera znajduje się szyna z rowkami, która umożliwia przykręcanie
:doc:`nakładek<Bolt-Ons>`. Przykładem takiej nakładki jest :ref:`łącznik mostowy<The Bridge Connector>`.
Wzdłuż tej szyny na każdym digitizerze znajdują się dwa porty USB-C — po jednym na zewnętrznej krawędzi
każdego "ramienia".

.. _M4G Frontside:
.. image:: /assets/images/M4G-Front.webp
  :width: 1200
  :alt: Zdjęcie przedstawiające łącznik mostowy i porty

Spód każdego digitizera jest częściowo wydrążony, aby umożliwić dyskretne prowadzenie kabli i połączeń pod
urządzeniem. Wewnątrz tej wnęki znajdują się dwa dodatkowe porty USB-C oraz skierowane w dół klastry diod LED.

.. _M4G Below:
.. image:: /assets/images/M4G-Under.webp
  :width: 1200
  :alt: Spód Master Forge

Na bokach każdego digitizera zauważysz :ref:`szyny końcowe<The Bookend Rails>`. Pod każdą szyną, na korpusie
digitizera, znajdują się otwory na śruby mocujące szyny końcowe na miejscu.

.. _M4G Side:
.. image:: /assets/images/M4G-Side.webp
  :width: 1200
  :alt: Oryginalna walizka dla wspierających

.. _Master Forge:The Bridge Connector:

Łącznik mostowy
~~~~~~~~~~~~~~~~~~~~~

Po wyjęciu z pudełka, Twoje :ref:`digitizery<The Digitizers>` będą połączone przez mechaniczną nakładkę
:doc:`bolt-on<Bolt-Ons>`. Ta :doc:`nakładka<Bolt-Ons>` również jest wykonana z obrabianego maszynowo aluminium
i zbudowana na bazie szyny z rowkami. Jest utrzymywana na miejscu przez dwie nylonowe śruby M3. Śruby nylonowe
nie "wbijają" się w aluminium tak jak śruby stalowe, co zapobiega uszkodzeniu rowkowanych szyn, ponieważ szyny
z przodu urządzenia nie mają otworów na śruby. Mocowanie opiera się bardziej na tarciu, co jest kluczową
zasadą :doc:`nakładek<Bolt-Ons>`.

.. _M4G Bridge Connector:
.. image:: /assets/images/Bridge.webp
  :width: 1200
  :alt: Połączenia mechaniczne i elektryczne

Dodatkowo, dwa :ref:`digitizery<The Digitizers>` są połączone za pomocą elektrycznego łącznika mostowego, znanego
również jako mini-connector. Ten element umieszcza się wewnątrz wnęki :ref:`mechanicznego łącznika
mostowego<Mechanical Bridge Connector>` i należy go wyjąć PRZED demontażem mechanicznego łącznika mostowego.

.. note::
    Podczas rozłączania digitizerów należy najpierw wyjąć :ref:`elektryczny łącznik
    mostowy<Electrical Bridge Connector>`, a dopiero później :ref:`mechaniczny łącznik
    mostowy<Mechanical Bridge Connector>`.

    Podobnie, podczas ponownego łączenia digitizerów należy wykonywać te czynności w
    odwrotnej kolejności niż przy rozłączaniu; czyli najpierw zabezpieczyć
    :ref:`mechaniczny łącznik mostowy<Mechanical Bridge Connector>`, a dopiero potem wpiąć
    :ref:`elektryczny łącznik mostowy<Electrical Bridge Connector>`.

Elektryczny łącznik mostowy to cienka płytka PCB zakończona wtykami USB-C po obu stronach. Powoduje to, że
przedni prawy port lewego digitizera łączy się z przednim lewym portem prawego digitizera.

Gdy urządzenie jest połączone oficjalnym łącznikiem Forge, lewy digitizer powinien być tym, który podłączasz
bezpośrednio do komputera. Zobacz sekcję :ref:`Pierwsze kroki<tag?>`, aby uzyskać więcej informacji na ten temat.

.. _Master Forge:The Bookend Rails:

Szyny końcowe
~~~~~~~~~~~~~~~~~~~

Każdy :ref:`digitizer<The Digitizers>` Master Forge zawiera trzy zdejmowane szyny końcowe. Te szyny umożliwiają
mocowanie digitizerów do innych :doc:`modułów kotwiczących<Anchor Bodies>` oraz :ref:`nakładek<Bolt-Ons>`.

.. _M4G Rails:
.. image:: /assets/images/Rails.webp
  :width: 1200
  :alt: Trzy szyny końcowe

Szyny końcowe są wykonane z obrabianego maszynowo aluminium i mocowane do korpusu
:ref:`digitizerów<The Digitizers>` za pomocą dwóch stalowych śrub (rozmiar).

.. _Master Forge:The Splitter:

Rozdzielacz
~~~~~~~~~~~~~~

W zestawie z każdym zamówieniem Master Forge znajduje się drukowany w 3D Rozdzielacz.
Ten element zapobiega wpadaniu czegokolwiek w przestrzeń pomiędzy :ref:`digitizerami<The Digitizers>`, gdy
są one połączone za pomocą :ref:`łącznika mostowego<The Bridge Connector>`.

.. _M4G Splitter:
.. image:: /assets/images/Splitter.webp
  :width: 1200
  :alt: Rozdzielacz

.. _Master Forge:The Switches:

Przełączniki
~~~~~~~~~~~~

Zamiast jednokierunkowych przycisków, które stosują tradycyjne klawiatury, :ref:`digitizer<The Digitizers>` Forge wykorzystują dźwignie, które nazywamy przełącznikami. Wykrywają one ruch w trzech wymiarach, dzięki czemu użytkownicy mają dostęp do 64 unikalnych wejść bez odrywania palców od urządzenia. Przełączniki :ref:`digitizer<The Digitizers>` generują wejście cyfrowe, w przeciwieństwie do analogowego. Wszystkie nasadki przełączników są drukowane w 3D i mają wymiary [wymiary]. Pod nasadką znajduje się trzpień o grubości [wymiary] i kwadratowym kształcie. Trzpień nie może być usunięty bez demontażu urządzenia, natomiast same nasadki są wymienialne na gorąco.

Każdy :ref:`digitizer<The Digitizers>` ma osiem pięciokierunkowych przełączników. Zaczynając od zewnętrznej strony każdego :ref:`digitizer<The Digitizers>` i przesuwając się do środka, przełączniki przypisane są do następujących palców: mały, serdeczny, środkowy i wskazujący. Dwa przełączniki wzdłuż „tułowia”, czyli najbardziej wewnętrznej strony każdego :ref:`digitizer<The Digitizers>`, przypisane są do kciuka. Domyślne znaki znajdujące się na każdym przełączniku możesz zobaczyć w :doc:`Układ<Layout>`. Dodatkowo, istnieją jeszcze dwa przełączniki poza „rzędem domowym”, do których dostęp mają serdeczny i środkowy palec. Poprawne ustawienie palców polega na podążaniu za łukiem, w jakim ułożone są przełączniki.

.. note::
   **WAŻNE**: W tym podręczniku będziemy odnosić się do przełączników w następujący
   sposób, zaczynając od małego palca i przesuwając się do środka: mały, serdeczny,
   środkowy, wskazujący, kciuk 1 oraz kciuk 2. Przełączniki znajdujące się poniżej
   „rzędu domowego” będą nazywane przełącznikami pomocniczymi aux 1 i aux 2, gdzie
   przełącznik najbardziej po lewej stronie lewego digitizera to aux 1.
   Symetrycznie, aux 1 na prawej części to przełącznik najbardziej po prawej stronie.

Każdy przełącznik posiada pięć kierunków nacisku. W całym przewodniku będziemy używać kierunków
geograficznych, gdzie _`północ` oznacza do przodu, w stronę od ciała. Przełączniki mogą poruszać
się: na północ, południe, zachód, wschód oraz w dół — do wnętrza urządzenia. Należy zauważyć, że
w przeciwieństwie do CC2, naciśnięcie przełączników do środka na Master Forge jest wejściem
akordowym, które aktywuje jednocześnie wszystkie cztery kierunki. Prosimy pamiętać, że w ramach
ergonomii urządzenia, każdy przełącznik ma nieco inny kąt nachylenia, dlatego warto zapoznać
się ze swoim nowym urządzeniem.

Spośród ośmiu przełączników, przełącznik małego palca został wykonany szerzej niż pozostałe, aby
ułatwić jego użycie, a także zoptymalizować funkcje przytrzymania klawisza, jak np. dla klawisza
Shift czy map warstwowych.

Jak wspomniano wcześniej, przełącznik może zostać aktywowany w pięciu kierunkach. Poza czterema
głównymi kierunkami, każdy przełącznik może być wciśnięty w głąb urządzenia. Nazywamy to często
naciśnięciem 3D, ponieważ nie jest to ruch boczny, lecz ruch w osi Z przełącznika. Ten specjalny
nacisk nie wymaga ruchu bocznego — wystarczy nacisnąć przełącznik „do środka” urządzenia.

Cztery główne kierunki przełącznika mogą być mapowane na dowolny klawisz — litery, cyfry, symbole,
klawisze sterujące, a nawet klawisze funkcyjne. Najnowszą listę kodów akcji można znaleźć w
`Device Manager <https://manager.charachorder.com/config/layout/>`__.
Naciśnięcie 3D nie może być przypisane do pojedynczego znaku, lecz pozwala na wciśnięcie wszystkich
czterech kierunków naraz, jako :doc:`akord<Chording>`.

.. _Master Forge:Connections:

Połączenia
-----------

Każde zamówienie Master Forge zawiera przewód zasilający, który podłączany jest do komputera.
Przewód zasilający dołączony do każdego Master Forge to standardowy, pleciony przewód USB-A do USB-C.
Niektóre :ref:`konfiguracje<Master Forge Configurations>` mogą zawierać dodatkowy przewód.
Aby dowiedzieć się, co zawiera Twoje zamówienie, przeczytaj sekcję
:ref:`konfiguracje<Master Forge:Master Forge Configurations>`.

.. _M4G Power Cable:
.. image:: /assets/images/Power-Cable.webp
  :width: 1200
  :alt: Przewód zasilający dołączony do Master Forge

Innym przewodem, który może być dołączony do Twojego zamówienia, jest pleciony przewód USB-C do USB-C, standard
3.2 gen 2. Przewód ten służy do użytku w przypadku, gdy zdecydujesz się rozdzielić swoje
:ref:`digitizery<The Digitizers>`.

.. dropdown:: O czym należy pamiętać, jeśli rozdzielasz digitizery
    
    Są dwie główne rzeczy, o których należy pamiętać w przypadku korzystania z rozdzielonych digitizerów Master Forge:
        1. Przewód łączący digitizery musi być przewodem 3.2 gen 2, USB-C do USB-C.
        2. Jak wskazano w sekcji :ref:`pierwsze kroki<Port Requirement>`, zasilanie dla
        :doc:`modułu kotwiczącego<Anchor Bodies>` lub :ref:`nakładki<Bolt-Ons>` musi być
        dostarczone przez lewy, przedni port USB-C. Oznacza to, że każdy moduł kotwiczący
        lub nakładka dodana do systemu musi być podłączona do Master poprzez przedni, lewy port.

.. _Master Forge:Getting Started:

Pierwsze kroki
*******************

Master Forge działa na zasadzie plug-and-play, więc nie wymaga dodatkowego oprogramowania, aby rozpocząć pracę.
Przed pierwszym podłączeniem Forge’a należy upewnić się, że
:ref:`elektryczny łącznik mostowy<Master Forge:The Bridge Connector>` lub przewód USB-C jest prawidłowo
podłączony do obu :ref:`digitizerów<Master Forge:The Digitizers>`.

.. _Port Requirement:
Wszystkie :doc:`moduły kotwiczące<Anchor Bodies>` Forge, w tym digitizery Master Forge, powinny być podłączone
do źródła zasilania przez przedni, lewy port USB-C. Należy używać tego konkretnego portu do połączenia z
komputerem, gdyż żaden inny port nie umożliwi poprawnego działania Forge. Zasadą jest, że wszystkie
:doc:`moduły kotwiczące<Anchor Bodies>` Forge muszą otrzymywać zasilanie przez przedni, lewy port.
Pozostałe trzy porty służą jako porty wyjściowe do łączenia kolejnych
:doc:`modułów kotwiczących<Anchor Bodies>` i :doc:`nakładek<Bolt-Ons>`.
Każdy dodatkowy :doc:`moduł kotwiczący<Anchor Bodies>` lub :doc:`nakładka<Bolt-Ons>` musi „odbierać”
zasilanie od "Master" :doc:`modułu kotwiczącego<Anchor Bodies>`, albo od podłączonego już
:doc:`modułu kotwiczącego<Anchor Bodies>` lub :doc:`nakładki<Bolt-Ons>`. "Master"
:doc:`moduł kotwiczący<Anchor Bodies>` to ten, który podłączony jest bezpośrednio do komputera.
Należy pamiętać, że niektóre :doc:`nakładki<Bolt-Ons>` mogą działać jako Master.

Jeśli jeszcze tego nie zrobiłeś, teraz jest odpowiedni moment, aby podłączyć do lewego
:doc:`digitizera<Master Forge:The Digitizers>` przewód USB-C do USB-A, który został dostarczony z zamówieniem.
Jeśli z powodów preferencji lub wymagań sprzętowych wolisz użyć przewodu USB-C do USB-C innego
producenta — również jest to możliwe. Bez względu na wybór, przewód podłączony bezpośrednio do komputera
będziemy nazywać głównym przewodem zasilającym (Power Cable). Jeśli posiadasz dodatkowe
:doc:`nakładki<Bolt-Ons>`, teraz jest dobry moment, aby je podłączyć do Master Forge.

.. warning::
   WAŻNE: Podczas pierwszego podłączenia Forge oraz za każdym razem, gdy masz włączoną funkcję
   :doc:`realtime-feedback<GenerativeTextMenu>`, zaleca się, aby kursor znajdował się w pustym polu tekstowym.
   Urządzenia :doc:`CCOS<CharaChorder Operating System (CCOS)>`, do których należy Master Forge, posiadają
   wiadomość powitalną, która może wysyłać polecenia do komputera, niezamierzone przez użytkownika.
   Funkcję tę można wyłączyć w :doc:`GTM<GenerativeTextMenu>`.

Po podłączeniu systemu możesz podłączyć przewód Master do komputera. Po połączeniu możesz zauważyć następujące
rzeczy:
    Jeśli kursor znajduje się w polu tekstowym...
        - Najpierw pojawi się tekst „Loading ### Chordmaps”, a po chwili „CCOS is ready.”
    Niezależnie od położenia kursora...
        - Diody LED pod :doc:`digitizerami<Digitizers>` rozpoczną cykl tęczowy.

Jeśli masz włączoną funkcję :ref:`realtime feedback<GenerativeTextMenu:Realtime feedback>`, gdy zobaczysz
wyróżniony tekst „CCOS is ready”, Twoje urządzenie jest gotowe do użycia.

.. note::
   WAŻNE: :ref:`Realtime feedback<GenerativeTextMenu:Realtime feedback>` jest domyślnie włączone w nowych
   urządzeniach CharaChorder.

Jeśli jest to Twój pierwszy raz z urządzeniem :doc:`CCOS<CharaChorder Operating System (CCOS)>`, zalecamy
następujące kroki:
    #. Umieść kursor w miejscu bezpiecznym do pisania
    #. Połóż dłonie na :doc:`digitizerach<Master Forge:The Digitizers>` i ustaw palce na przełącznikach
    #. Poruszaj palcami wskazującym, środkowym i serdecznym na południe, w kierunku swojego ciała, jeden po drugim.

Ruchy te odpowiadają literom U, O, E, T, N i S. Teraz spróbujmy wykonać :doc:`akord<Chording>`.

.. dropdown:: Jak wykonać akord?

    Akord to rodzaj wejścia, który pozwala na jednoczesne naciśnięcie wielu klawiszy w celu uzyskania
    zaprogramowanego :ref:`wyniku<Chords:Chord Output>`. Aby wykonać akord, należy nacisnąć wszystkie
    :ref:`klawisze wejściowe<Chords:Chord Input>` w tym samym czasie, w ramach
    :ref:`limitu czasu naciśnięcia<GenerativeTextMenu:Press Tolerance>`.
    Dodatkowo, należy zwolnić wszystkie klawisze jednocześnie — w ramach
    :ref:`limitu czasu zwolnienia<GenerativeTextMenu:Release Tolerance>`.
    Po poprawnym wykonaniu tych kroków, urządzenie CCOS szybko wpisze wciśnięte klawisze, usunie je, a
    następnie wprowadzi zaprogramowany akord.

Możemy przetestować fabrycznie wgrane akordy, których jest 500, wykonując :doc:`akord<Chords>`, naciskając
oba palce wskazujące na południe, w stronę ciała. Być może trzeba będzie poeksperymentować z czasem wciśnięcia.
Pamiętaj, że należy nacisnąć oba przełączniki jednocześnie, a następnie jednocześnie je zwolnić.
Jak wcześniej wspomniano, wymaga to pewnej wprawy, ale ostatecznie powinieneś zobaczyć, jak na ekranie
pojawia się słowo „the”. Gratulacje! Właśnie wykonałeś akord!

.. dropdown:: Inne przykładowe akordy do wypróbowania
    
    Oto inne fabrycznie wgrane akordy, które możesz wypróbować.
    W sekcji :ref:`notacja akordowa<Chords:Chord Notation>` znajdziesz instrukcje, jak interpretować
    poniższe akordy.
        - c+b = because
        - m+b = maybe
        - u+o+y = you

Gdy już opanujesz podstawy i nauczysz się wykonywać akordy, możesz przejść do :doc:`sekcji treningowej<Tools>`,
aby rozpocząć naukę obsługi urządzenia. Jeśli wolisz od razu przejść do ćwiczeń bez dalszego czytania, odwiedź
naszą stronę treningową: https://www.iq-eq.io/#/

.. _Dot I/O:
.. image:: /assets/images/DOTIO.png
  :width: 1200
  :alt: Ćwiczenia na DOT I/O

.. _Master Forge:Setting Up:

Konfiguracja
-----------

Jeśli jest to Twój pierwszy raz z Master Forge, istnieje kilka kroków, które prawdopodobnie będziesz
chciał wykonać. W poniższej sekcji zaktualizujemy Twoje urządzenie, wyjaśnimy nawigację w
:doc:`GTM<GenerativeTextMenu>` oraz zaprezentujemy domyślny układ na Twoim nowym urządzeniu.

.. _Master Forge:Updating your Device:

Aktualizacja urządzenia
~~~~~~~~~~~~~~~~~~~~~

.. _M4G-checking-your-devices-firmware:

Sprawdzanie wersji oprogramowania sprzętowego urządzenia
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Możesz sprawdzić aktualną wersję oprogramowania swojego urządzenia, wykonując poniższe kroki:

1. W przeglądarce opartej na Chromium, takiej jak Chrome, przejdź do CharaChorder
`Device Manager <https://charachorder.io/config/layout/>`__.

2. Kliknij „Connect” na dole ekranu.

.. _Connect Button:
.. image:: /assets/images/FW-connect-button.JPG
  :width: 600
  :alt: Przycisk Connect w Device Manager

3. Gdy pojawi się okno dialogowe „charachorder.io chce połączyć się z portem szeregowym”, wybierz
swoje urządzenie Master Forge, a następnie kliknij niebieski przycisk „connect”.

.. _Serial Port Popup:
.. image:: /assets/images/SerialPort-Message.webp
  :width: 600
  :alt: Okno wyboru urządzenia szeregowego

Po wykonaniu powyższych kroków zobaczysz wersję oprogramowania w lewym dolnym rogu ekranu.
Powinna wyglądać mniej więcej tak:
``CCOS 2.0.2``

.. _Firmware Check:
.. image:: /assets/images/DMFW.png
  :width: 600
  :alt: Sprawdzanie wersji firmware w Device Manager

.. _Master Forge:Updating the Firmware:


Aktualizacja firmware
^^^^^^^^^^^^^^^^^^^^^^^

Jeśli okaże się, że Twoje urządzenie nie działa na najnowszej wersji firmware, możesz wykonać poniższe
kroki, aby je zaktualizować. Aktualną wersję firmware możesz sprawdzić odwiedzając
`tę stronę <https://charachorder.io/ccos/m4g_s3/>`__.

.. warning::
   WAŻNE: Przed wykonaniem poniższych kroków upewnij się, że posiadasz
   :ref:`kopię zapasową swojego układu<Device Manager:Creating a Backup>`,
   :ref:`kopię biblioteki akordów<Device Manager:Creating a Backup>` oraz
   :ref:`kopię ustawień GTM<Device Manager:Creating a Backup>`.
   Aktualizacja może przywrócić ustawienia fabryczne, dlatego ważne jest, aby mieć przygotowane kopie zapasowe.
   Instrukcje przywracania znajdziesz w sekcji :ref:`Kopie zapasowe<Device Manager:Restoring from a Backup>`.

Master Forge obsługuje aktualizacje OTA (Over-The-Air). Aby zaktualizować urządzenie, wykonaj następujące kroki:
    #. Przejdź do `CharaChorder Device Manager <https://charachorder.io/ccos/>`__
    #. Jeżeli nie jesteś jeszcze na stronie aktualizacji firmware, kliknij ``CCOS Updates`` w
       lewym dolnym rogu strony.

        .. _Firmware Updates Page:
        .. image:: /assets/images/DM-CCOS-button.jpg
          :width: 600
          :alt: Przycisk CCOS w Device Manager

    #. Spośród dostępnych opcji wybierz ``m4g_s3``.
       
        .. _Firmware Selection:
        .. image:: /assets/images/m4g-firmware-selection.JPG
          :width: 600
          :alt: Wybór odpowiedniego firmware

    #. Porównaj najnowszą wersję (widoczną na górze listy) z wersją swojego urządzenia. Wybierz żądaną wersję.
    #. Jeżeli jeszcze tego nie zrobiłeś, podłącz urządzenie do Device Manager klikając "Connect" na dole strony.

        .. _Connect Button:
        .. image:: /assets/images/FW-connect-button.JPG
          :width: 600
          :alt: Przycisk Connect w Device Manager

    #. Gdy pojawi się okno dialogowe „charachorder.io chce połączyć się z portem szeregowym”, wybierz swoje
       urządzenie Master Forge i kliknij niebieski przycisk „connect”.

        .. _Serial Port Popup:
        .. image:: /assets/images/SerialPort-Message.webp
          :width: 600
          :alt: Okno wyboru urządzenia szeregowego

    #. Kliknij niebieski przycisk "Apply Update".
        
        .. _Apply Update Button:
        .. image:: /assets/images/DM-applyupdate-button.jpg
          :width: 600
          :alt: Przycisk Apply Update

Twoje urządzenie uruchomi się ponownie automatycznie i będzie miało wgraną nową wersję firmware po
ponownym uruchomieniu. Możesz :ref:`sprawdzić wersję firmware<M4G-checking-your-devices-firmware>`, aby
upewnić się, że aktualizacja przebiegła pomyślnie.

.. dropdown:: Tylko w sytuacjach awaryjnych

    Jeżeli z jakiegoś powodu nie udało Ci się przeprowadzić aktualizacji OTA, możesz wykonać poniższe kroki, aby ręcznie zaktualizować CCOS.

    W przypadku aktualizacji ręcznej Master Forge musi być aktualizowany pojedynczo — dla każdego
    :ref:`digitizera<Master Forge:The Digitizers>` oddzielnie.
        #. W przeglądarce opartej na Chromium, takiej jak Chrome, przejdź do CharaChorder
           `Device Manager <https://charachorder.io/ccos/>`__
        #. Jeżeli połączenie nie nastąpiło automatycznie, kliknij „Connect”

       	    .. _Connect Button:
            .. image:: /assets/images/FW-connect-button.jpg
              :width: 600
              :alt: Przycisk Connect w Device Manager

        #. Gdy pojawi się okno dialogowe „manager.charachorder.com chce połączyć się z portem szeregowym”,
        wybierz urządzenie CCOS, które chcesz zaktualizować, a następnie kliknij niebieski przycisk „connect”.

            .. _Serial Port Popup:
            .. image:: /assets/images/SerialPort-Message.jpg
              :width: 600
              :alt: Okno wyboru urządzenia szeregowego

        #. Jeżeli nie jesteś jeszcze na stronie aktualizacji firmware, kliknij "CCOS Updates" w lewym
           dolnym rogu strony.

               .. _Firmware Updates Page:
               .. image:: /assets/images/DM-CCOS-button.jpg
                 :width: 600
                 :alt: Przycisk CCOS w Device Manager

        #. Porównaj najnowszą wersję (na górze listy) z wersją Twojego urządzenia. Wybierz żądaną wersję.
        #. Kliknij niebieski napis "Bootloader", aby uruchomić urządzenie w trybie bootloadera.

       		  .. _Bootloader button:
              .. image:: /assets/images/DM-Bootloader-button.jpg
                :width: 600
                :alt: Przycisk Bootloader

        #. Kliknij niebieski napis "CURRENT.UF2", aby pobrać plik firmware.

      		   .. _Current.uf2 button:
               .. image:: /assets/images/DM-UF2-button.jpg
                 :width: 600
                 :alt: Przycisk CURRENT.UF2

            .. warning::
                WAŻNE: Upewnij się, że pobrany plik nazywa się dokładnie: CURRENT.UF2. Jeżeli w nazwie pliku
                znajdą się inne znaki, plik nie zadziała. Plik nazwany „CURRENT.UF2(1)” NIE zadziała.
                Dodatkowo, nazwa pliku jest czuła na wielkość liter — wszystkie litery muszą być pisane
                wielkimi literami.

        #. Skopiuj właśnie pobrany plik CURRENT.UF2 i wklej go do dysku Forge w eksploratorze plików.
        #. Gdy system zapyta, jak rozwiązać konflikt nazw plików, wybierz „Zastąp plik”.

            W tym momencie Forge automatycznie uruchomi się ponownie, a napęd Forge zniknie. Gratulacje!
            Pomyślnie zaktualizowałeś swoje urządzenie. Możesz sprawdzić wersję firmware, wykonując kroki
            :ref:`tutaj<m4g-checking-your-devices-firmware>`.

        #. Teraz, na stronie `Firmware Updates <https://charachorder.io/ccos/>`__, wybierz ``m4gr_s3``.
        #. Jeśli jeszcze tego nie zrobiłeś, ponownie połącz urządzenie z Managerem klikając
           "Connect" na dole strony.

            .. _Connect Button:
            .. image:: /assets/images/FW-connect-button.jpg
              :width: 600
              :alt: Przycisk Connect w Device Manager

        #. Gdy pojawi się okno dialogowe „charachorder.io chce połączyć się z portem szeregowym”, wybierz swoje
           urządzenie Master Forge, a następnie kliknij niebieski przycisk „connect”.

            .. _Serial Port Popup:
            .. image:: /assets/images/SerialPort-Message.jpg
              :width: 600
              :alt: Okno wyboru urządzenia szeregowego

        #. Użyj niebieskiego napisu "Bootloader", aby przełączyć prawy digitizer w tryb bootloadera.

            .. _Bootloader button:
            .. image:: /assets/images/DM-Bootloader-button.jpg
              :width: 600
              :alt: Przycisk Bootloader

        #. Kliknij niebieski napis "CURRENT.UF2", aby pobrać plik firmware.

            .. _Current.uf2 button:
            .. image:: /assets/images/DM-UF2-button.jpg
              :width: 600
              :alt: Przycisk CURRENT.UF2

            .. warning::
                WAŻNE: Upewnij się, że pobrany plik nazywa się dokładnie: CURRENT.UF2. Jeżeli w nazwie pliku
                znajdą się inne znaki, plik nie zadziała. Plik nazwany „CURRENT.UF2(1)” NIE zadziała.
                Dodatkowo, nazwa pliku jest czuła na wielkość liter — wszystkie litery muszą być pisane
                wielkimi literami.

        #. Skopiuj właśnie pobrany plik CURRENT.UF2 i wklej go do dysku Forge w eksploratorze plików.
        #. Gdy system zapyta, jak rozwiązać konflikt nazw plików, wybierz „Zastąp plik”.

Napęd Forge zniknie a urz adzenie automatycznie uruchomi się ponownie.
Możesz sprawdzić wersję firmware swojego urządzenia, wykonując kroki
:ref:`tutaj<m4g-checking-your-devices-firmware>`.

.. _Master Forge:Understanding the Settings:

Zrozumienie ustawień
----------------------------

Forge posiada ustawienia operacyjne, które mogą być konfigurowane przez użytkownika.
Ponieważ urządzenie działa na zasadzie plug-and-play, nie potrzebujesz żadnego dodatkowego
oprogramowania, aby edytować ustawienia urządzenia; wystarczy miejsce, w którym możesz wpisać tekst.
Te ustawienia nazywamy Generative Text Menu, w skrócie GTM.

Możesz uzyskać dostęp do :doc:`GTM<GenerativeTextMenu>`, wykonując :doc:`akord<Chords>` poprzez
jednoczesne naciśnięcie obu małych palców na `północ`_ w dowolnym miejscu, gdzie możesz wprowadzać
tekst — na przykład w notatniku. Aby uzyskać wyjaśnienie dotyczące akordów i sposobu ich wykonywania,
odwiedź sekcję :doc:`Chords<Chords>`.

Po wykonaniu akordu wywołującego :doc:`GTM<GenerativeTextMenu>`, Forge wpisze na ekranie menu i dostępne opcje.
Będzie to wyglądać mniej więcej tak:

``Master Forge GTM [ >K<eyboard || >M<ouse || >C<hording || >D<isplay || >R<esources ]``

Nawigacja po tym menu opiera się na naciskaniu liter.
W powyższym przykładzie możesz wybrać żądaną podkategorię, naciskając literę umieszczoną między
nawiasami (na przykład: ``>K<``) odpowiadającą danemu podmenu na Twoim CharaChorder One.
W powyższym przykładzie naciskasz ``K`` dla Klawiatury, ``M`` dla Myszki, ``C`` dla Chordingu,
``D`` dla Wyświetlania i ``R`` dla Zasobów.

W niektórych podmenu zobaczysz wartości liczbowe. Aby je zwiększać lub zmniejszać, możesz używać klawiszy
strzałek na :ref:`digitizerach<The Digitizers>`.

``CharaChorder > Chording > Press Tolerance [ Use up/down arrow keys to adjust: 25ms ]``

Możesz przeczytać wyjaśnienia wszystkich ustawień swojego urządzenia CharaChorder :doc:`tutaj<GenerativeTextMenu>`.

.. _Master Forge:Learning the Layout:

Nauka układu
---------------------

Domyślny układ :ref:`digitizerów<The Digitizers>` Master Forge, który będziemy nazywać układem M4 English,
został zaprojektowany tak, aby faworyzować :doc:`bigramy<Logic behind the Layout>` i
:doc:`trigramy<Logic behind the Layout>` powszechnie używane w języku angielskim, zapewniając jednocześnie
logiczny wybór znaków dla :doc:`leksykalnych<Chords>`. Mapę znajdziesz poniżej.

.. note::
   Ogólny konsensus wśród społeczności mówi, że choć układ domyślny nie jest idealny, to rozmieszczenie
   liter jest na tyle dobre, że dalsze modyfikacje przynoszą niewielką korzyść, biorąc pod uwagę, że
   osiągnięto już ponad 500 słów na minutę w warunkach szczytowych.

   **Najczęściej zmienia się jedynie rozmieszczenie znaków specjalnych i cyfr**, np. dla ułatwienia programowania.

   Istnieją wyjątki polegające na optymalizacji pod VIM, choć wielu użytkowników skutecznie korzystało z
   domyślnego układu w VIM i korzyści z takich modyfikacji są dyskusyjne.

.. _M4English Layout:
.. image:: /assets/images/M4-Layout.png
  :width: 1200
  :alt: Układ M4 English

.. _Master Forge:Layers:

Warstwy
~~~~~~

Układ Master Forge posiada 3 warstwy: warstwę bazową zwaną warstwą A1, drugorzędną warstwę A2 oraz
trzeciorzędną warstwę A3.
Ponieważ Master Forge posiada 8 przełączników na każdym :ref:`digitizerze<Master Forge:The Digitizers>`,
biorąc pod uwagę, że każdy przełącznik może mieć przypisane 4 różne pozycje indywidualne, oraz
uwzględniając, że każda warstwa daje dostęp do wszystkich 8 przełączników, mamy ponad 190 dostępnych
slotów przypisywalnych pomiędzy dwoma :ref:`digitizerami<Master Forge:The Digitizers>`.

W tej sekcji będziemy odnosić się wyłącznie do domyślnego układu M4 English.
Jeżeli zmodyfikowałeś swój układ, dalsza część może nie odpowiadać dokładnie Twojemu urządzeniu.
Jeśli zakupiłeś urządzenie bezpośrednio od CharaChorder, poniższe informacje są zgodne z Twoim urządzeniem.

Domyślnie warstwy pomocnicze są dostępne po naciśnięciu i przytrzymaniu klawiszy dostępu do warstw.
Powoduje to tymczasowe „przesunięcie” do jednej z warstw pomocniczych. Obecnie istnieje „obejściowa”
metoda ustawienia warstw przełączanych zamiast tymczasowych, jednak nie jest to funkcja oficjalna.
Przełączane warstwy, o ile istnieją w aktualnych wersjach CCOS, nie zostały gruntownie przetestowane
i mogą zawierać błędy.

.. _Toggleable Layers:
.. dropdown:: Warstwy przełączane

    Jeżeli nie interesuje Cię wyjaśnienie dlaczego to działa, możesz przejść od razu do kroków opisanych
    poniżej w celu włączenia warstw przełączanych.

    Urządzenia CCOS używają metody „przesuwanych” warstw, wymagającej przytrzymania klawisza, aby uzyskać
    dostęp do klawiszy w warstwach pomocniczych. Domyślnie klawisze dostępu do warstw informują urządzenie
    o wejściu w daną warstwę. Zwolnienie przełącznika powoduje powrót do warstwy bazowej, ponieważ ta sama
    „lokalizacja” jest przypisana do przycisku dostępu do warstwy w docelowej warstwie. Możemy wykorzystać
    tę funkcjonalność i zmusić urządzenie CCOS do pozostania w danej warstwie, po prostu usuwając klawisz
    dostępu do warstwy z docelowej warstwy. W ten sposób urządzenie nie wie, że powinno wrócić do warstwy
    bazowej po zwolnieniu przełącznika.

    Aby skonfigurować urządzenie na tryb warstw przełączanych zamiast przesuwanych, należy przejść do
    `Device Manager <https://charachorder.io/config/layout/>`__ i zmodyfikować mapowanie klawiszy.
    Poniżej opisujemy, jak przemapować klawisz dostępu do warstwy A2, jednak te same kroki obowiązują
    dla warstwy A3. Instrukcje te zakładają, że urządzenie zostało już podłączone do
    `Device Managera <https://charachorder.io/config/layout/>`__.

        1. Upewnij się, że klawisz dostępu do warstwy A2 jest przypisany do wybranego miejsca na warstwie Alfa
           (warstwa A1). To będzie klawisz, którego będziesz używać do przełączania na warstwę A2.

        2. Na warstwie A2 znajdź tę samą lokalizację, gdzie przypisałeś klawisz dostępu A2 i zmień go
           (na warstwie A2) na ``No Key Pressed``. Ta zmiana zapobiega automatycznemu powrotowi urządzenia do
           warstwy A1 po zwolnieniu przełącznika.

        3. Na warstwie A2 wybierz inną lokalizację i przypisz tam klawisz dostępu A2. Będzie to klawisz, którym
           wrócisz do warstwy Alfa.

.. _M4G Alpha Layer:

Warstwa A1
^^^^^^^^

.. _M4G Alpha Layer:
.. image:: /assets/images/AlphaL.JPG
  :width: 1200
  :alt: Warstwa Alfa

Warstwa A1 to główna warstwa, która jest aktywna domyślnie. Układ M4 English zawiera wszystkie 26 liter
alfabetu angielskiego na warstwie A1, dzięki czemu masz dostęp do wszystkich liter bez konieczności
przytrzymywania lub naciskania dodatkowych klawiszy. Urządzenie zawsze uruchamia się domyślnie w warstwie A1.

Chociaż domyślnie aktywna na :ref:`digitizerach<Master Forge:The Digitizers>` jest warstwa A1, możesz
przypisać klawisz dostępu do warstwy A1 (o nazwie „Primary Keymap (Left)” lub „Primary Keymap (Right)”)
w `Device Manager <https://charachorder.io/config/layout/>`__.

.. note::
    Przypisanie klawisza dostępu do warstwy A1 jest zbędne, chyba że skonfigurujesz urządzenie do
    :ref:`przełączania między warstwami<Toggleable Layers>` zamiast ich przesuwania.

.. _M4G Num Layer:

Warstwa A2
^^^^^^^^

.. _M4G Num Layer:
.. image:: /assets/images/NumberL.JPG
  :width: 1200
  :alt: Warstwa Numeryczna

Warstwa A2, czasami nazywana „warstwą numeryczną”, jest dostępna za pomocą
:doc:`klawisza dostępu do A2<CharaChorder Keys>`. Na powyższej :ref:`grafice<CCEnglish Layout>`
oznaczono ją jako „num-shift”. W `Device Manager <https://charachorder.io/config/layout/>`__
klawisz ten ma nazwę „Numeric Layer (Left)” oraz „Numeric Layer (Right)”, osobno dla każdego
:ref:`digitizera<Master Forge:The Digitizers>`.

Domyślnie warstwa A2 jest dostępna poprzez naciśnięcie i przytrzymanie dowolnego z małych palców na
zewnątrz, tj. w lewo (zachód) na lewym małym palcu lub w prawo (wschód) na prawym małym palcu.
Nie musisz przytrzymywać obu — wystarczy jeden.

Każdy klawisz dostępny na warstwie A2 może być aktywowany poprzez naciśnięcie i przytrzymanie klawisza
dostępu do warstwy A2 razem z docelowym klawiszem. Nie musisz ich :doc:`akordować<Chords>`; wystarczy, że
klawisz dostępu do A2 jest wciśnięty w momencie naciśnięcia klawisza docelowego.

.. note::
   PRZYKŁAD: Na układzie M4 English możesz uzyskać cyfrę ``4``, przytrzymując prawy mały palec na wschód
   oraz lewy środkowy palec na wschód.

.. _M4G Function Layer:

Warstwa A3
^^^^^^^^

.. _M4G Function Layer:
.. image:: /assets/images/FunctionL.JPG
  :width: 1200
  :alt: Warstwa Funkcyjna

Warstwa A3, czasami nazywana „warstwą funkcyjną”, jest dostępna za pomocą
:ref:`klawisza dostępu do A3<CharaChorder Keys>`. Klawisz ten nie jest widoczny na powyższej
:ref:`grafice<CCEnglish Layout>`, a dostęp do niego uzyskuje się poprzez [INFO].
W `Device Manager <https://charachorder.io/config/layout/>`__ klawisz ten nosi nazwę
„Function Layer (Left)” i „Function Layer (Right)”, po jednym dla każdego
:ref:`digitizera<Master Forge:The Digitizers>`.

Domyślnie warstwa A3 jest dostępna poprzez [INFO]. Nie musisz przytrzymywać obu klawiszy jednocześnie,
aby uzyskać dostęp do warstwy A3. Każdy klawisz na warstwie A3 może być aktywowany poprzez naciśnięcie
i przytrzymanie :doc:`klawisza dostępu do A3<CharaChorder Keys>` oraz docelowego klawisza.
Nie trzeba :doc:`akordować<Chords>` tych klawiszy; wystarczy, że klawisz dostępu do A3 jest przytrzymywany
podczas naciskania klawisza docelowego.

.. note::
   PRZYKŁAD: Na układzie M4 English możesz uzyskać klawisz F1, naciskając i przytrzymując [INFO], a następnie
   dodając literę ``a`` lub ``r`` (miejsce odpowiadające cyfrze 1 w domyślnym układzie).

.. _Shift Modifier:

Modyfikator Shift
^^^^^^^^^^^^^^

.. dropdown:: Lista akcji dla klawisza Shift
        
        .. csv-table:: Akcje klawiszy po wciśnięciu Shift
           :header-rows: 1
           :stub-columns: 0
           :widths: auto

           "Klawisz alfanumeryczny", "Klawisz po wciśnięciu Shift"
           "`", "~" 
           "1", "\!"
           "2", "\@"
           "3", "\#"
           "4", "\$" 
           "5", "\%"
           "6", "\^"
           "7", "\&"
           "8", "\*" 
           "9", "\("
           "0", "\)"
           "\-", "\_"
           "=", "\+" 
           "[", "\{"
           "]", "\}"
           "\\", "\|"
           ";", ":" 
           "\'", """"
           "\,", "\<"
           ".", ">"
           "/", "?"
   
 
Ponad trzema wspomnianymi warstwami, klawisz :doc:`Shift<CharaChorder Keys>`, który jest
:doc:`modyfikatorem<Glossary>`, umożliwia dostęp do dodatkowych znaków. Klawisz Shift działa dokładnie
tak samo, jak na tradycyjnej klawiaturze. Pozwala na wpisywanie wielkich liter oraz dostęp do symboli
przypisanych do cyfr. Działa na każdym klawiszu w każdej warstwie, podobnie jak inne modyfikatory
(takie jak Ctrl i Alt). Wyjście modyfikatora Shift jest obecnie kontrolowane przez system operacyjny,
do którego podłączony jest Forge, i nie jest możliwe dostosowywanie ich w urządzeniu.

Na powyższej grafice klawisz Shift oznaczono jako „Shift”.
W `Device Manager <https://charachorder.io/config/layout/>`__ klawisz ten nosi nazwę
„Shift Keyboard Modifier (Left)” oraz „Shift Keyboard Modifier (Right)” — po jednym dla każdego
:ref:`digitizera<The Digitizers>`.

Domyślnie dostęp do Shift uzyskuje się poprzez przytrzymanie dowolnego z małych palców do wewnątrz,
tj. wschód na lewym małym palcu lub zachód na prawym małym palcu. Nie trzeba przytrzymywać obu,
wystarczy jeden. Każdy klawisz wymagający modyfikatora Shift może być aktywowany poprzez naciśnięcie
i przytrzymanie klawisza Shift oraz docelowego klawisza. Nie trzeba ich :doc:`akordować<Chords>`;
wystarczy przytrzymać Shift podczas naciskania klawisza docelowego.

.. note::
   PRZYKŁAD: Na układzie M4 English możesz wpisać wielką literę ``A``, naciskając i przytrzymując
   lewy mały palec na wschód oraz prawy palec wskazujący na zachód.

   Na układzie M4 English możesz uzyskać symbol ``@``, naciskając i przytrzymując oba małe palce na
   wschód oraz lewy palec wskazujący na południe.

.. _Configurability:

Konfigurowalność
~~~~~~~~~~~~~~~

Układ Master Forge jest konfigurowalny, co oznacza, że możesz :doc:`przypisać na nowo<Glossary>` niemal
wszystkie klawisze. Chociaż układ M4 English został zoptymalizowany do pisania po angielsku za pomocą
:doc:`wpisywania akordowego<Glossary>` oraz :doc:`akordowania<Chords>`, niektórzy użytkownicy mogą
zdecydować się na :doc:`przypisanie<Glossary>` układu urządzenia, aby lepiej dostosować go do własnych potrzeb.
Szczegółowe wyjaśnienie sposobu działania przypisywania klawiszy oraz jak przypisać je na nowo znajdziesz
w sekcji :ref:`remapping<Device Manager:Remapping>`.

.. _Master Forge Configurations:

Konfiguracje Master Forge
****************************

Kiedy Master Forge został `zaprezentowany <https://youtu.be/fux9gU3M25E?si=u4KW7OaUUUNINfKD&t=1025>`__ w
listopadzie 2023 roku, CharaChorder rozpoczęło przyjmowanie zamówień w przedsprzedaży, oferując wszystkim
ten sam zestaw. We wrześniu 2024 roku CharaChorder przeprowadziło kampanię
`Kickstarter <https://www.kickstarter.com/projects/charachorder/the-master-forge-a-keyboard-built-for-you>`__
dla Master Forge, trwającą 5 tygodni, oferując trzy różne pakiety, każdy z inną konfiguracją. Po zakończeniu
kampanii Kickstarter Master Forge trafił do sprzedaży w systemie zamówień oczekujących na stronie
`Forge <https://forgekeyboard.com>`__. W poniższej sekcji przedstawiono, co zawierały poszczególne 5 pakietów.

.. _Forge Website Pre-Orders:

Zamówienia na stronie Forge
-------------------------

Master Forge został ogłoszony na dorocznym
`ChorderCon w 2023 roku <https://youtu.be/fux9gU3M25E?si=WmNs4bxXJcg0JbKM>`__ organizowanym przez CharaChorder.
Został zaprezentowany razem z marką Forge i innymi produktami Forge, takimi jak Coder's Forge i Gamer's Forge.
Po gwałtownym wzroście liczby zamówień na Master Forge, nadano mu priorytet rozwojowy.
Każde zamówienie na Master Forge złożone między listopadem 2023 roku a początkiem sierpnia 2024 roku zawierało:

    - :ref:`Jeden (1) lewy digitizer<Master Forge:The Digitizers>`
    - :ref:`Jeden (1) prawy digitizer<Master Forge:The Digitizers>`
    - :ref:`Jeden (1) elektryczny łącznik mostowy<Master Forge:The Bridge Connector>`
    - :ref:`Jedną (1) mechaniczną nakładkę mostową<Master Forge:The Bridge Connector>`
    - :ref:`Jeden (1) przewód zasilający USB-A do USB-C<Master Forge:Connections>`
    - :ref:`Jedną (1) nakładkę Ergo<Bolt-Ons:Ergo>`
    - :ref:`Dwie (2) nakładki Forge Trackball<Bolt-Ons:Trackball>`
    - :ref:`Jedną (1) taktyczną walizkę transportową<Case>`
    - :ref:`Jeden (1) Forge Cleat<Add-Ons:Cleat>`
    - Jedno (1) narzędzie imbusowe M3
    - :ref:`Jedną (1) podkładkę biurkową Original Backer<Add-Ons:Original Backer Deskmat>`

.. note::

    Na dzień marca 2025 roku nakładka Forge Trackball nie zakończyła jeszcze rozwoju.
    W związku z tym niektóre zamówienia przedsprzedażowe oraz wspierający na Kickstarterze mogą nie
    otrzymać swoich nakładek trackball wraz z Master Forge. Zostaną one wysłane w późniejszym terminie.

.. _Kickstarter Orders:

Zamówienia Kickstarter
----------------------
Kampania Kickstarter dla Master Forge rozpoczęła się 27 sierpnia 2024 roku i zakończyła 7 października 2024 roku.
Pakiety oferowane na Kickstarterze podzielono na trzy: Basic, Premium i Super.

.. _Basic:

Basic
~~~~~~
Pakiet Basic na Kickstarterze zawierał następujące elementy:

    - :ref:`Jeden (1) lewy digitizer<Master Forge:The Digitizers>`
    - :ref:`Jeden (1) prawy digitizer<Master Forge:The Digitizers>`
    - :ref:`Jeden (1) elektryczny łącznik mostowy<Master Forge:The Bridge Connector>`
    - :ref:`Jedną (1) mechaniczną nakładkę mostową<Master Forge:The Bridge Connector>`
    - :ref:`Jeden (1) przewód zasilający USB-A do USB-C<Master Forge:Connections>`
    - :ref:`Jedną (1) „Original Backer” taktyczną walizkę transportową<Case>`
    - Jedno (1) narzędzie imbusowe M3
    - Nieograniczony dostęp do Forge CAD

.. _Premium:

Premium
~~~~~~~~
Pakiet Premium na Kickstarterze zawierał następujące elementy:

    - :ref:`Jeden (1) lewy digitizer<Master Forge:The Digitizers>`
    - :ref:`Jeden (1) prawy digitizer<Master Forge:The Digitizers>`
    - :ref:`Jeden (1) elektryczny łącznik mostowy<Master Forge:The Bridge Connector>`
    - :ref:`Jedną (1) mechaniczną nakładkę mostową<Master Forge:The Bridge Connector>`
    - :ref:`Jeden (1) przewód zasilający USB-A do USB-C<Master Forge:Connections>`
    - :ref:`Jeden (1) przewód USB-C do USB-C<Master Forge:Connections>`
    - :ref:`Jedną (1) nakładkę Forge Trackball<Bolt-Ons:Trackball>`
    - :ref:`Jedną (1) „Original Backer” taktyczną walizkę transportową<Case>`
    - :ref:`Jedną (1) podkładkę biurkową „Original Backer”<Add-Ons:Original Backer Deskmat>`
    - Jedno (1) narzędzie imbusowe M3
    - :ref:`Jedną (1) nakładkę Forge Cleat<Add-Ons:Cleat>`
    - :ref:`Cztery (4) zestawy nakładek Ergo<Bolt-Ons:Ergo>`
    - Nieograniczony dostęp do Forge CAD
    - 2 lata członkostwa VIP

.. _Super:

Super
~~~~~~~

Pakiet Super na Kickstarterze zawierał następujące elementy:

    - :ref:`Jeden (1) lewy digitizer<Master Forge:The Digitizers>`
    - :ref:`Jeden (1) prawy digitizer<Master Forge:The Digitizers>`
    - :ref:`Jeden (1) elektryczny łącznik mostowy<Master Forge:The Bridge Connector>`
    - :ref:`Jedną (1) mechaniczną nakładkę mostową<Master Forge:The Bridge Connector>`
    - :ref:`Jeden (1) przewód zasilający USB-A do USB-C<Master Forge:Connections>`
    - :ref:`Jeden (1) przewód USB-C do USB-C<Master Forge:Connections>`
    - :ref:`Jedną (1) nakładkę Forge Trackball<Bolt-Ons:Trackball>`
    - :ref:`Jedną (1) „Original Backer” taktyczną walizkę transportową<Case>`
    - :ref:`Jedną (1) podkładkę biurkową „Original Backer”<Add-Ons:Original Backer Deskmat>`
    - Jedno (1) narzędzie imbusowe M3
    - :ref:`Jedną (1) nakładkę Forge Cleat<Add-Ons:Cleat>`
    - :ref:`Cztery (4) zestawy nakładek Ergo<Bolt-Ons:Ergo>`
    - Nieograniczony dostęp do Forge CAD
    - Członkostwo VIP dożywotnio
    - Wpisanie do GTM Immortalization
    - Egzoszkielet digitizera podpisany przez Riley’a Keena, założyciela i CEO CharaChorder

.. _Post-Kickstarter:

Po Kickstarterze
-----------------

Po zakończeniu kampanii Kickstarter Master Forge został udostępniony do zamówień w przedsprzedaży na stronie
`Forge <https://forgekeyboard.com>`__. Zamówienia złożone na stronie Forge od października 2024 roku zawierały:

    - :ref:`Jeden (1) lewy digitizer<Master Forge:The Digitizers>`
    - :ref:`Jeden (1) prawy digitizer<Master Forge:The Digitizers>`
    - :ref:`Jeden (1) elektryczny łącznik mostowy<Master Forge:The Bridge Connector>`
    - :ref:`Jedną (1) mechaniczną nakładkę mostową<Master Forge:The Bridge Connector>`
    - :ref:`Jeden (1) przewód zasilający USB-A do USB-C<Master Forge:Connections>`
    - :ref:`Jedną (1) taktyczną walizkę transportową<Case>`
    - Jedno (1) narzędzie imbusowe M3
