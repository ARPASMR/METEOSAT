# METEOSAT
codice per l'elaborazione delle immagini meteosat

# crontab di libertario

```
# Elaborazione HRIT/LRIT Meteosat­9
#
00,15,30,45 * * * * (sh /home/meteo/scripts/elab_msg_batch.sh > /home/meteo/log/elab_msg_batch.log 2>&1)
#
# Elaborazione HRIT/LRIT Meteosat­8 RSS
#
1,6,11,16,21,26,31,36,41,46,51,56 * * * * (sh /home/meteo/scripts/elab_rss_batch.sh > /home/meteo/log/elab_rss_batch.log 2>&1)

```
# constraints

vengono utilizzati diversi applicativi esterni:

_minutes_ per il calcolo della data cui viene aggiunto un certo numero di minuti

_xrit-0.2.5_ utilities per la trattazione dei file METEOSAT

_XRITDecompress_ non riportato per problemi di licenza Eumetsat
