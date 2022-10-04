# Pokročilé metódy analýzy dát

Návody na cvičenia môžete spustiť v prostredí [DataLab](https://datalab.kkui.fei.tuke.sk).

### Spustenie na lokálnom počítači:

1. Nainštalujte si [Docker](https://https://docs.docker.com/get-docker/)
2. V príkazovom riadku sa prepnite do vášho lokálneho adresára v ktorom máte súbory s ktorými chcete pracovať a spustite kontajner s prostredím JupyterLab.

   **pre Linux**
   ```console
   docker container run -it --rm -p 8888:8888 -v "${PWD}":/home/jovyan/work peterbednar/tensorflow-notebook:2.3.1
   ```
   **pre Windows**
   ```console
   docker container run -it --rm -p 8888:8888 -v "%CD%":/home/jovyan/work peterbednar/tensorflow-notebook:2.3.1
   ```
3. V prehliadači sa pripojte na ```http://localhost:8888```. Pre prihlásenie zadajte token zobrazený v konzole príkazového riadku.

### GPU

Ak máte operačný systém Linux a grafickú kartu Nvidia, môžete spustit kontajner s podporou výpočtov na grafickej karte.
```console
docker container run -it --rm -p 8888:8888 -v "${PWD}":/home/jovyan/work peterbednar/tensorflow-gpu-notebook:2.3.1
```
