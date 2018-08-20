# smartmirror
Configuración de mi smart mirror


#CRON
$:~ crontab -e

//APAGARÁ LA PANTALLA A LAS 12 DE LA NOCHE Y LA ENCENDERÁ A LAS 8 AM
//https://raspberrypi.stackexchange.com/questions/67991/raspbian-put-monitor-to-sleep-at-night-and-wake-in-morning
* 0 * * * DISPLAY=:0 xset dpms force off
* 8 * * * DISPLAY=:0 xset dpms force on
