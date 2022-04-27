# OSINT
## Catch Me If You Can 01

- Une entreprise soupçonne une personne de revendre sa marchandise sur internet. Grace au pseudo fournis retrouvé le prénom et le nom de cette personne.
- pseudo : cclkawa

- Utiliser un outil pour retrouver des info à partir d'un nom d'utilisateur:
- https://github.com/thewhiteh4t/nexfil

# Reseau

## TXT in Black (réseau)

- Vous connaissez les fameux sites : google.com, netflix.com, stackoverflow.com (ne faites pas les innocents) Mais saviez vous que d'autres types d'enregistrements existent ? Retrouvez le flag parmi les autres informations pouvant être trouvées pour le domaine btth.enigme-ctf.fr

- On a un indice dans le titre : TXT
- Un enregistrement TXT est un type d'enregistrement DNS (Domain Name System) qui fournit des informations sous forme textuelle à des sources extérieures
- On peut faire une recherche de "btth.enigme-ctf.fr" sur https://dnslookup.online/txt.html

## Les dents de la mer 2 (réseau)

- Encore du traffic! Retrouver les informations permettant de valider ce challenge. Le premier indice proposé n'est peut être pas le plus rapide mais ca vaut le coup de le connaître! A vous de voir.
- on a un fichier pcap à ouvrir dans WireShark
- La taille des requêtes ICMP doit nous mettre sur la piste
- Après je sais pas...

## Les dents de la mer 1 (réseau)

- Il y a du traffic ICMP dans cette capture de trames! Mais de quel OS provient ce traffic?
- Pour valider ce challenge, renseigner le nom de l'OS plus les 2 derniers caractères qui permettent de l'identifier. Format du flag : ENI{nomDeLOS??}

- Le format des requêtes ICMP diffère selon les OS
- Après je sais pas...

## Take a SIP (réseau) 

- Retrouver le mot de passe utilisé par** l’administrateur** pour se connecter à l’infrastructure SIP.
- On a un fichier pdf, en descendant on tombe là-dessus:

`Authorization: Digest username="eniadmin", realm=«esdhackademy»,
nonce="626ab425", uri="sip:172.65.10.250", algorithm=MD5,
response="7c6a180b36896a0a8c02787eeafb0e4c"``

- le mot de passe est 7c6a180b36896a0a8c02787eeafb0e4c haché en MD5

# WEB
## Ghostbusters
- Allo, les chasseurs de fantômes ? Quelque chose de bizarre se passe sur ce site web. Pouvez-vous retrouver le fantome qui s'y cache ?
- !! Outils d'énumération OK !!
http://51.254.115.112:4567/ 

- On peut utiliser l'outil DirBuster avec la wordlist "RockYou.txt" et l'extension html, 
- Dans l'onglet "result", on voit apparaître "file /tinkerbell1.html
- Si on essaye de se rendre sur http://51.254.115.112:4567/tinkerbell1.html --> ENI{I_ain't_'fraid_of_no_ghost}

# Steganographie 

- quelques outils : Steghide ; exiftool
