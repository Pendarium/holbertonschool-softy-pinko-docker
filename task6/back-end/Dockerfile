FROM ubuntu:latest

# Mise à jour et upgrade
RUN apt-get update
RUN apt-get upgrade -y

# Installer Python3 et pip3
RUN apt-get install -y python3 python3-pip

# Corriger l'erreur "externally managed" si elle apparaît
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Installer Flask avec pip3
RUN pip3 install flask

RUN pip3 install flask-cors


# Définir le dossier de travail
WORKDIR /app

# Copier le script Python dans l'image
COPY ./api.py /app/api.py

# Lancer Flask au démarrage
CMD ["python3", "api.py"]
