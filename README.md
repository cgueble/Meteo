# Meteo
Projet meteo de Chloé - connection internet, recuperarion des données méteo du jour et affichage via une aiguille

carte utilisée: ?

au power on:
activation de la liaison serie 115200
extinction de toutes les LED
aiguille fait un A/R complet et s'arrète en position "en attente de data"

Connexion internet:
connexion a un wifi propre préconfiguré
Si pas dispo => activation en continu du WPS  (clignottement rapide de la led bleu: 500ms on ; 500ms off)

Si connexion wifi owner => led blue clignotte lentement (100ms on ; 2s Off)
si connexion a un autre wifi via WPS => led bleu clignotte très lentement (100ms on ; 5s Off)

dès que la connexion wifi est ok
connexion au serveur meteo
recuperation des données
mise a 24h du compte a rebour de validité des données
mise a 1h du compte a rebour c
affichage des données

données:
LED pluie
Led Neige
Led alerte meteo clignotant
aiguille : temperature -5 à 35
-5; 5[ 
[5 ; 10[
[10; 15[
[15; 20[
[20 ; 25[
[25 ; 30[
[30 ; 35

quand compte a reboure de recherche de données arrive a zero -> on se re connecte au serveur meteo et on recommence

Si le compteur de validité des données arrive a zero, on etteint toutes les led et on met l'aiguille sur en attende de data et on relance setup



