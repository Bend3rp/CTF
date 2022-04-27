# Catch Me If You Can 01

- Une entreprise soupçonne une personne de revendre sa marchandise sur internet. Grace au pseudo fournis retrouvé le prénom et le nom de cette personne.
- pseudo : cclkawa

- Utiliser un outil pour retrouver des info à partir d'un nom d'utilisateur:
- https://github.com/thewhiteh4t/nexfil


# TXT in Black (réseau)

- Vous connaissez les fameux sites : google.com, netflix.com, stackoverflow.com (ne faites pas les innocents) Mais saviez vous que d'autres types d'enregistrements existent ? Retrouvez le flag parmi les autres informations pouvant être trouvées pour le domaine btth.enigme-ctf.fr

- On a un indice dans le titre : TXT
- Un enregistrement TXT est un type d'enregistrement DNS (Domain Name System) qui fournit des informations sous forme textuelle à des sources extérieures
- On peut faire une recherche de "btth.enigme-ctf.fr" sur https://dnslookup.online/txt.html

# Les dents de la mer 2 (réseau)

- Encore du traffic! Retrouver les informations permettant de valider ce challenge. Le premier indice proposé n'est peut être pas le plus rapide mais ca vaut le coup de le connaître! A vous de voir.
- on a un fichier pcap à ouvrir dans WireShark
- La taille des requêtes ICMP doit nous mettre sur la piste

# Les dents de la mer 1 (réseau)

- Il y a du traffic ICMP dans cette capture de trames! Mais de quel OS provient ce traffic?
- Pour valider ce challenge, renseigner le nom de l'OS plus les 2 derniers caractères qui permettent de l'identifier. Format du flag : ENI{nomDeLOS??}

- Le format des requêtes ICMP diffère selon les OS

