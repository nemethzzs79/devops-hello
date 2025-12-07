# DevOps Hello World

Ez a projekt egy egyszerű Python Flask alkalmazást tartalmaz, amely DevOps alapfogalmak
bemutatására szolgál.

Az alkalmazás egyetlen HTTP végpontot (`/`) biztosít, amely egy szöveges választ ad vissza.

---

## Alkalmazás futtatása

### Futtatás Docker nélkül

1. Függőségek telepítése:
python -m pip install -r requirements.txt

2. Alkalmazás indítása:
python app.py

Az alkalmazás böngészőben elérhető:
http://localhost:8080

---

### Futtatás Docker használatával

Docker image build:
docker build -t devops-hello:v1 .

Konténer futtatása:
docker run -p 8080:8080 devops-hello:v1

Az alkalmazás böngészőben elérhető:
http://localhost:8080

---

## Git használata

A projekt Git verziókezelést használ trunk-based fejlesztési modellben.

- main branch: stabil verzió
- feature-minor-update branch: kisebb módosítás kipróbálására

A feature branch külön commitban készült, majd visszamerge-elve a main ágba.

---

## Választható feladat: Dev Container (VS Code)

A projekt tartalmaz VS Code Dev Container konfigurációt, amely lehetővé teszi
a fejlesztési környezet Docker konténerben történő használatát.

Használat:
- Projekt megnyitása VS Code-ban
- Dev Containers: Reopen in Container
- Alkalmazás indítása a konténerben: python app.py

Az alkalmazás elérhető:
http://localhost:8080

---

GitHub repository:
https://github.com/nemethzzs79/devops-hello