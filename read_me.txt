Kometar rjesenja:

Napravio sam dvije Jupyter bilježnice. Jedna mi služi za stvaranje baze, dok druga prima upit i radi retrieval.

Stvaranje Docker slike:
docker build -f Dockerfile.retrieval -t vid-bebek-vm .

Pokretanje:
docker run -it --rm -p 9090:8888 vid-bebek-vm

Prvi korak je extract foldera database. Pripaziti da se nakon extracta database.zip folder dataset sa dokumentima prebaci u direktorij.

Database skripta se lokalno vrti oko 9 minuta i stvara 2 file-a koje koristi retrieval bilježnica.
Online izvođenje skripte traje duže od toga te iz tog razloga uploadam već spremne fileove za lakše testiranje.

U retrieval bilježnicu potrebno je unijeti API ključ za model.

U bilježnicama sam ostavio ispis ćelija prilikom testiranja.

