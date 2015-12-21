# [Sheep](https://telegram.me/Sheeppy) 
**Questa è un semplicissimo fork in italiano di TeleSeed, un avanzato e potente bot che semplifica e migliora l'amministrazione dei gruppi su Telegram. TeleSeed è basato su Yagop ([yagop/telegram-bot](https://github.com/yagop/telegram-bot)) licensed under [GNU General public License](https://github.com/SEEDTEAM/TeleSeed/blob/master/LICENSE)**
# Features

* **Anti spam con possibilità di settare la sensibilità per ogni gruppo**
* **Realms multipli (gruppi di amministrazione)**
* **Immune ad ogni genere di spam con bot XY, con possibilità di bloccare nome, foto, membri, aggiunta di bot**
* **Ban globale**
* **Possibilità di broadcast su ogni gruppo**
* **Permette di ottenere il link del gruppo**
* **Kicka, banna ed unbanna con una semplice risposta**
* **Lista dei gruppi, degli utenti bannati, anche globalmente**
* **Log completo degli eventi che avvengono nel gruppo!**
* **Invita by username**
* **Possibilità di amministrare un gruppo interagendo in privato col bot**
* **Blocco della lingua arabica**
* **Ed altro...**


```bash
# Testato su Ubuntu 14.04 e c9.io, per altri OS consulta https://github.com/yagop/telegram-bot/wiki/Installation
sudo apt-get install libreadline-dev libconfig-dev libssl-dev lua5.2 liblua5.2-dev libevent-dev make unzip git redis-server g++ libjansson-dev libpython-dev expat libexpat1-dev
```

```bash
# Installiamo il bot
cd $HOME
git clone https://github.com/Rmazz96/TeleSheep.git
cd TeleSeed
chmod +x launch.sh
./launch.sh install
./launch.sh # Inserisci il numero di telefono ed il codice di verifica.
```
### un solo comando
Per installare con un solo comando su distro basate su debian (utile per distribuzioni VPS), usa:
```sh
#https://github.com/yagop/telegram-bot/wiki/Installation
sudo apt-get update; sudo apt-get upgrade -y --force-yes; sudo apt-get dist-upgrade -y --force-yes; sudo apt-get install libreadline-dev libconfig-dev libssl-dev lua5.2 liblua5.2-dev libevent-dev libjansson* libpython-dev make unzip git redis-server g++ -y --force-yes && git clone https://github.com/SEEDTEAM/TeleSeed.git && cd TeleSeed && chmod +x launch.sh && ./launch.sh install && ./launch.sh
```
### Avviare Redis
```bash
cd $HOME
redis-server
#Controllare se Redis funziona correttamente
redis-cli ping
#(Dovrebbe restituire la stringa PONG)
```

### Configurazione del primo Realm

Dopo aver avviato il bot per la prima volta, spegnilo

Crea un gruppo vuoto ed aggiungi il bot

Avvia nuovamente il bot

Ottieni l'id del gruppo creato con /id ed aggiungilo al table dei realms in config.lua

```lua
realm = {},--Realms Id
```
Riavvia il bot


# Supporto e sviluppo

Non contattare i creatori di Seed bot in privato.

Se individui qualche errore grammaticale/problema/malfunzionamento, contattami in privato ([@Rlotar](https://telegram.me/Rlotar)) od utilizza github.


# Ringraziamenti speciali a:
[@seyedan25](https://telegram.me/seyedan25)

Per gestire [@teleseed](https://telegram.me/TeleSeed) su Telegram

[@topkecleon](https://github.com/topkecleon)

[@JuanPotato](https://github.com/JuanPotato)

# TUTTI I CREDITI A:

[Alphonse](https://github.com/hmon) ([Telegram](https://telegram.me/iwals))

[I M /-\ N](https://github.com/imandaneshi) ([Telegram](https://telegram.me/imandaneshi))

[Siyanew](https://github.com/Siyanew) ([Telegram](https://telegram.me/Siyanew))

Canale ufficiale > [@TeleSeedCH](https://telegram.me/teleseedch)

Me, l'inutile essere che ha tradotto TeleSeed in italiano: [@Rlotar](https://telegram.me/Rlotar)
