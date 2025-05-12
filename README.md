# Programowanie Aplikacji w Chmurze Obliczeniowej - Zadanie 1 (Część obowiązkowa)
### 1. Budowa obrazu
```bash
docker build -t pogoda-app:1.0 .
```
![build](img/img_p/build.png)

### 2. Sprawdzenie liczby warstw i rozmiaru obrazu
```bash
docker image inspect weather-app:1.0 --format='Warstwy: {{len .RootFS.Layers}}, Rozmiar: {{.Size}} bajtów'
```
![inspect](img/img_p/inspect.png)

### 3. Uruchomienie kontenera
```bash
docker run -d -p 3000:3000 --name weather-app weather-app:1.0
```
![run](img/img_p/run.png)

### 4. Wyświetlenie logów
```bash
docker logs weather-app
```
![logs](img/img_p/logs.png)

### 5. Działanie aplikacji
![app1](img/img_p/app1.png)
![app2](img/img_p/app2.png)
