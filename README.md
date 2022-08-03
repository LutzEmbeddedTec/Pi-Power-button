# Pi-Power-button


sudo nano /boot/config.txt

# switch on an off

dtoverlay=gpio-shutdown,gpio_pin=3, active_low=1,gpio_pull=up



sudo systemctl daemon-reload

sudo systemctl start powerbutton.service

sudo systemctl status powerbutton.service

sudo systemctl enable powerbutton.service
