# eNom / eNomCentral dynamic dns

eNom supports dynamic dns, however documentation sucks and all provided programs are outdated. After some research I figure out a simple way to update via curl:

`curl "https://reseller.enom.com/interface.asp?command=setdnshost&zone=$ZONE&domainpassword=$DOMAIN_PASSWORD&address=$CURRENT_IP&hostname=$HOSTNAME”`

where:

- `$ZONE` - is your domain name
- `$DOMAIN_PASSWORD` - is NOT account password but password per domain - you can find it in General Settings for your domain name
- `$CURRENT_IP` - an IP address you would like to update to
- `$HOSTNAME` - is a host name ( example: `*` or `www` )



Don’t hesitate to contact me if you have any questions. 
