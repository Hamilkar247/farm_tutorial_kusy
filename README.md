
0. Upewnić się mamy uruchomioną conda w odpowiednim środowisku
na geologii to farm-kusy

`conda activate farm-kusy`

1. Włączyć baze danych MONGODB
w geologii to u mnie /home/matball/Projects/mongodb pod tym miejscem mam obraz dockera
bazy danych bez hasla

`docker-compose up`

odpalamy przeglądarkę 127.0.0.1/27017 (domyślny port mongodb) i sprawdzamy czy wykrywa nam coś na tym porcie.

2. odpalenie compass do przegladania danych mongodb

`mongodb-compass`

3. w folderze backend znajduje się main.py uruchamiamy komendę

`uvicorn main:app --port 8000 --reload`

dzięki czemu odpali sie na ustawionym porcie 127.0.0.1:8000

co sprawdzmy najpierw wstukujac to, a potem dodajac postfix /docs
(jest też alternatywna dokumentacja wtedy postfix jest /redoc


4. odpalenie frontenda reacta

przechodzimy do folderu 'frontend' ( z wlaczonym conda activate 'farm-kusy' )
i odpalamy 'npm start' w konsoli
