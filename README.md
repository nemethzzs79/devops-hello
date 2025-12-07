# DevOps Hello – Flask alkalmazás

Ez egy egyszerű „Hello world” Flask alkalmazás, amely a DevOps alap lépéseit mutatja be:
- kódkészítés (Python)
- verziókövetés (Git, trunk-based)
- buildelés
- konténerizálás Dockerrel

Az alkalmazás HTTP-n elérhető, és egy egyszerű szöveget ad vissza.

---

## Alkalmazás

A Flask alkalmazás egy egyszerű HTTP endpointot tartalmaz.

- URL: http://localhost:8080
- Válasz: `Hello DevOps világ!`

---

## Követelmények

- Python 3.11+  
- pip  
- Docker Desktop (Windows)  
- Git  

---

## Build és futtatás

### Fejlesztői futtatás (Docker nélkül)

```bash
python -m pip install -r requirements.txt
python app.py

### 1. Függőségek telepítése

```bash
python -m pip install -r requirements.txt


## 2. Választható feladat: Dev Container (3.1)

Mivel VS Code-ot és Dockert már használsz, a Dev Container a legkényelmesebb opció.

### 2.1. `.devcontainer` mappa létrehozása

1. VS Code-ban a bal oldali **Explorerben** kattints jobb gombbal a projekt gyökerére (`devops-hello` mappa).  
2. **New Folder** → neve:  
   ```text
   .devcontainer