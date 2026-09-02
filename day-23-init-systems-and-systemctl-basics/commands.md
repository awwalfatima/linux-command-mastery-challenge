#systemctl start this command is for starting a service immediately, i.e sudo systemctl start nginx
#systemctl stop this stops a running service immediately, syntax: sudo systemctl stop service 
#systemctl restart this command stops and starts a service again. syntax sudo systemctl restart service, i.e sudo systemctl restart nginx
#systemctl reload this command reloads a service's configuration without completely stopping the service, provided the service supports reloads. syntax: sudo systemctl reload service.
#systemctl enable configures a service to start automatically when the system boots.
#systemctl disable prevents a service from automatically starting during boot.
#systemctl enable --now enables a service and starts it immediately. 
#systemctl status displays detailed information about a service.
#systemctl is-active checks whether a service is currently running. sytanx systemctl is-active service.
#systemctl is-enabled checks whether a service is configured to automatically start during boot.