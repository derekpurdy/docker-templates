# unRAID Docker Templates

- Chronograf
- Kapacitor
  - To generate a kapacitor.conf file in /etc/kapacitor perform the following command.
  
    `kapacitord config > /etc/kapacitor/kapacitor.conf`
  - Then override any required parameters in the file generated above and restart container.
  - Once Kapacitor is up and running add it into Chronograf.
