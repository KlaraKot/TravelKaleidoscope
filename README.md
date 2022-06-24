#create virtual environement <br />
`pip install virtualenv` <br />
`mkvirtualenv tk` <br />

#activate your virtual environment<br />
`workon tk` <br />

#install requirements<br />
`pip install -r requirements.txt` <br />

#for add new requirements<br />
`pip freeze > requirements` <br />

#create constraints <br />
`python manage.py install_labels` <br />

#run api server <br />
`python manage.py runserver` <br />

#open Django shell <br />
`python manage.py shell` <br />

<br />
<br />


# Kalejdoskop Podróży
Nasza aplikacja pozwala na wyszukiwanie najodpowiedniejszego miejsca do odwiedzenia, bazując na informacji podanej przez użytkownika, a także na doświadczeniach innych osób zarejestrowanych w systemie.

## Z perspektywy użytkownika
Aby skorzystać z aplikacji należy założyć konto oraz wypełnić krótką ankietę, która pomoże aplikacji w zarekomendowaniu miejsca najlepiej spełniającego oczekiwania użytkownika. Po zarejestrowaniu użytkownik może poprosić o zarekomendowanie miejsca, które najlepiej do niego pasuje. Może również samodzielnie wyszukiwać miejsca w systemie i sprawdzać opinie i recenzje dodane uprzednio przez inne osoby lub opisać własne doświadczenia, aby ułatwić decyzję innym. Oprócz miejsc można także wyszukiwać innych użytkowników i przeglądać ich profile.


## Ankieta

Aplikacja wymaga założenia konta i wypełnienia krótkiej ankiety pozwalającej na określenie preferencji. Pytania zawarte w ankiecie to:
1. Hobby?
2. Ulubione miejsce?
3. Odwiedzone miejsca?
4. Ulubione jedzenie?
5. Preferowana pogoda?
6. Czy miejce ma być przystosowane do kwaterowania zwierząt?
7. Czy podróżujesz z małym dzieckiem/dziećmi?
8. Czy miejsce ma posiadać udogodnienia dla osoby niepełnosprawnej?

Uzyskanie powyższych informacji pozwoli aplikacji na porównanie podanych odpowiedzi z odpowiedziami innych użytkowników oraz ich ocenami i wybranie najodpowiedniejszego miejsca do odwiedzenia.

## Opinie
Każde miejsce odwiedzone przez użytkownika może zostać ocenione w skali 1 - 5 gwiazdek. Pozwoli nam to na lepsze dopasowywanie miejsc w przyszłości. Użytkownik może również napisać recenzję odwiedzonego miejsca i pomóc innym w szukaniu wycieczki.

## Wyszukiwanie
Aby znaleźć informacje o interesującym miejscu użytkownik może skorzystać z wyszukiwarki aby uzyskać dostęp do ocen i recenzji osób, które zdążyły już je odwiedzić.

## Rekomendacja
Aplikacja bierze pod uwagę informacje podane w ankiecie oraz opinie użytkowników o podobnych preferencjach aby, na życzenie użytkownika, polecić mu miejsce do odwiedzenia.

## Historia
Zmiany dokonywane przez użytkowników są zapisywane w historii. Dzięki temu można je w łatwy sposób wycofać.

## Administrator
Konto administratora posiada więcej uprawnień niż zwykły użytkownik. Może usuwać oraz blokować inne konta na określony czas, na przykład w przypadku nieprzestrzegania regulaminu.

## Kwestie techniczne
Backend aplikacji zostanie zaprogramowany w Pythonie, ze względu na jego przystosowanie do algorytmów rekomendujących, oraz przy użyciu Django REST framework, natomiast do wykonania frontendu wykorzystany zostanie typeScript oraz React. Systemem zarządzającym bazą danych jest MongoDB.

Poniżej diagram klas aplikacji:

![enter image description here](https://media.discordapp.net/attachments/893836286035640333/903968201937915966/unknown.png?width=1060&height=489)
