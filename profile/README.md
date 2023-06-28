# :blue_car: CarService
Projekt systemu dla serwisu samochodowego wykonany w architekturze mikorusługowej z wykorzystaniem styków REST API.

## Wstęp
Projekt składa się z 8 modułów:
- 4 mikrousługi danych odpowiedzialne za operacje na danych
- 2 mikrousługi aplikacyjne odpowiedzialne za operacje użytkownika
- 2 aplikacje użytkownika

## Role
Przewidziane są dwie role użytkownika:
### Mechanik
Ma dostęp do wszystkich aut, wizyt, edycji niektórych właściwości wizyt.
### Użytkownik
Ma dostęp do swoich aut, wizyt, dodawania nowych aut, a także zapisywania na wizyty.

## CI/CD
Dla każdej z mikrousług jest utworzony proces CI/CD, zarządzający kompilacją, testami jednostkowymi, konteneryzacją oraz uruchominiem w środowisku produkcyjnym.

## Produkcja
System można uruchomić na platformie DockerCompose, bądź Kubernetes. Dzięki procesowi CI/CD możliwe jest "hot-swapping", z zerowym czasem "downtime", nowych wersji oprogramowania zamkniętych w kontenerze. 
