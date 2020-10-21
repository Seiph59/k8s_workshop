# Introduction à Docker

## 1.Installation
Connectez-vous à votre VM et procédez à l'installation de docker avec les commandes ci-dessous:

```bash
sudo apt-get update
sudo apt-get install -y docker.io
```

Afin de pouvoir utiliser Docker sans élévation de privilège (sudo), coller la commande ci-dessous:

```bash
sudo setfacl -m user:$USER:rw /var/run/docker.sock
```

Puis vérifiez votre installation avec le traditionnel 'Hello world'

```bash
docker run hello-world
```

## 2.Lancement de son premier conteneur

Téléchargez une image nginx depuis [docker-hub](https://hub.docker.com), qui référence toutes les images publiques proposées pour docker.
Pour des questions de sécurité, il est toujours conseillé de 'pull' en priorité les images officielles.

![Image officielle Nginx](/assets/images/hub-nginx.jpg)

Pour télécharger l'image, sans la lancer, faites la commande suivante:

```bash
docker pull nginx
```

Vous devriez désormais avoir 2 images, si vous lancez la commande:

```bash
docker images
```
### Lancez votre première image
Pour lancer le serveur Nginx, vous devez lancer la commande suivante:

```bash
docker run nginx
```

Vous devriez désormais voir apparaitre votre conteneur en tapant la commande:

```bash
docker ps
```


