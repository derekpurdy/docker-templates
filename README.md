# unRAID Docker Templates

- Chronograf
- Kapacitor
  - To generate a kapacitor.conf file in /etc/kapacitor perform the following command.
  
    `kapacitord config > /etc/kapacitor/kapacitor.conf`
  - Then override any required parameters in the file generated above and restart container.
  - Once Kapacitor is up and running add it into Chronograf.
- matrix-dimension
  - You need to grab the default.yaml file and save it as /data/config.yaml
  `https://raw.githubusercontent.com/turt2live/matrix-dimension/master/config/default.yaml`
  - Start the server, and then stop it
  - You need to edit the /data/config.yaml file

homeserver:
  name:
  clientServerUrl:
  federationUrl:
  accessToken:

admins:

database:
  file: "/data/dimension.db"
  botData: "/data/bot.json"

dimension:
  publicUrl:
