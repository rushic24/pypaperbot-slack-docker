
# To host on Oracle ARM

## Open port 5000
    Networking -> Virtual Cloud Networks -> vcn-xxyxyyzzz -> Security List Details
    
![image](https://user-images.githubusercontent.com/6279035/183801116-49ca2392-4ff2-418d-a8b0-21acaf3321ae.png)

## Enable connections on port 5000 through firewall

```bash
sudo  firewall-cmd  --permanent --zone=public --list-ports
sudo firewall-cmd --get-active-zones
sudo firewall-cmd --permanent --zone=public --add-port=5000/tcp
sudo firewall-cmd --reload
```

# Follow the same instructions above to enable port 5002 and 3000

## Add the public ip of the server in the Slack API for / commands

![image](https://user-images.githubusercontent.com/6279035/183801561-a218404a-27df-4766-bc75-2299eec4b2f6.png)
