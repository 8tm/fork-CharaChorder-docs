.. _Layout:

Układ
=======

Dziwactwa układu
------

TL;DR, co to dla mnie oznacza?
^^^^

Przede wszystkim, oto kilka pułapek:

* Jeśli ustawisz na przykład znak `$`, CCOS wpisze go jako „przytrzymaj shift, naciśnij 4, zwolnij shift”.
  Oznacza to, że jeśli naciśniesz `$` i `3` jednocześnie, **w rzeczywistości wpiszesz "$#" zamiast "$3"**,
  ponieważ CCOS musi przytrzymać shift, aby wpisać znak `$`.
    - *Unikaj umieszczania znaków wymagających shiftu i zwykłych znaków na tej samej warstwie.*
* Używanie na przykład niemieckiego układu klawiatury w systemie operacyjnym zamieni miejscami litery z i y,
  tak jak na zwykłej klawiaturze.
* Używanie dowolnych znaków spoza zestawu ASCII, Chara lub spoza standardowej klawiatury będzie działać
  *wyłącznie* na systemie Windows.
* Hacki stosowane przez Chara mogą mieć nieoczekiwane skutki w niektórych programach, które przechwytują
  surowe dane wejściowe.

.. tip::
  Najprostszym rozwiązaniem jest użycie układu
  `US-Intl <https://en.m.wikipedia.org/wiki/QWERTY#US-International>`_ w systemie operacyjnym.
  Możesz używać prawego Alt, aby uzyskiwać znaki specjalne.
  Przytrzymanie prawego Alt i naciśnięcie `q` da Ci znak `ä`.

Drugim rozwiązaniem jest korzystanie z lokalnego układu i mentalne odwzorowanie klawiszy.
Na przykład, jeśli chcesz wpisać cyrylicką literę `Ф`, ustawiasz w systemie operacyjnym
rosyjski układ klawiatury i przypisujesz klawisz do `a` (co wysyła kod klawisza odpowiadający
literze `Ф` w rosyjskim układzie).

Co tu się właściwie dzieje?
^^^^^

Intuicyjnie można by się spodziewać, że klawiatury wysyłają do systemu literę nadrukowaną na
naciśniętym klawiszu. Niestety, tak nie jest. Nie istnieje *żaden sposób*, aby jakiekolwiek
urządzenie mogło poinformować system operacyjny, jaka litera powinna zostać wpisana — na
żadnym systemie operacyjnym.

Klawiatury wysyłają tzw. **kod klawisza (key-code)** do systemu operacyjnego, czyli identyfikator
naciśniętego klawisza. Ten kod klawisza nie ma żadnego związku z faktycznie wpisywaną literą — to
system operacyjny decyduje, jaki znak przypisać do danego kodu klawisza. Mapowanie to określa
układ klawiatury, który *nie może* być ustawiany przez samo urządzenie — *musi* być skonfigurowany
w systemie operacyjnym.

Jedyną konwencją jest tutaj *lokalizacja* klawiszy — *na standardowej klawiaturze QWERTY
(US layout)*. Istnieją pewne znormalizowane lokalizacje oparte na amerykańskim układzie, takie
jak zestaw znaków ASCII, klawisze GUI/Windows, CTRL, SHIFT itd. Jednak wszystkie (lub większość)
z nich zakładają amerykański układ klawiatury.

Nie ma żadnego standardu dla innych urządzeń do wprowadzania znaków, ani sposobu, w jaki urządzenie
mogłoby rozpoznać, jaki układ został ustawiony w systemie operacyjnym.

Jak CharaChorder sobie z tym radzi?
^^^^^^

Jeżeli ustawisz układ w CCOS, przesuwa on lokalizacje kodów klawiszy.
If you set a layout on the CCOS, it moves the key-code locations around. 

.. warning::
  Ustawienie litery `a` na przełączniku nie powoduje faktycznego wysłania "wpisz a" do
  komputera — wysyłany jest kod klawisza odpowiadającego pozycji litery `a` na układzie
  amerykańskim (US layout).

Jak dodać znaki äöüß itd., gdy nie ma ich w układzie US?
^^^^^^^

Istnieje specjalna funkcja w systemie Windows, która pozwala bezpośrednio wpisywać
*dowolny* znak Unicode za pomocą klawiatury, przytrzymując `alt` i wpisując kod numeryczny.

.. warning::
  Ustawienie litery `ä` na przełączniku powoduje, że urządzenie wysyła sekwencję:
  „przytrzymaj alt, naciśnij 0, naciśnij 2, naciśnij 2, naciśnij 8, zwolnij alt”.

Ponieważ jest to funkcja systemu Windows, działa tylko na Windows. Jednak nawet ona
*nie* jest niezależna od układu. Użycie układu zmieniającego pozycje liter, jak
Programmer Dvorak, całkowicie psuje tę metodę.

Istnieją podobne obejścia dla Linuksa i Maca, ale obecnie nie są one wspierane przez CCOS.

„Prawdziwe” rozwiązanie
^^^^^^^

Najlepszym rozwiązaniem jest zawsze poleganie na mapowaniu systemu operacyjnego.

Windows, Mac i Linux oferują możliwość tworzenia własnych niestandardowych układów.

* Windows: `MSKCL <https://www.microsoft.com/en-us/download/details.aspx?id=102134>`_
* Mac: `Ukelele <https://software.sil.org/ukelele/>`_
* Linux: `xkb <https://wiki.archlinux.org/index.php/X_keyboard_extension>`_
