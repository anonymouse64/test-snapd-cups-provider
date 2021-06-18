# test-snapd-cups-provider

This repo is a test of the cups slot interface provider. 

To build it, use snapcraft, and install the snap with:

```
snap install test-snapd-cups-provider --dangerous
```

Then build the corresponding consumer snap at https://github.com/anonymouse64/test-snapd-cups-consumer and run:


```
snap install test-snapd-cups-consumer --dangerous
```

and connect the cups interface plug to the slot:

```
snap connect test-snapd-cups-consumer:cups test-snapd-cups-provider:cups
```

and then try out the connection between the two:

```
sudo test-snapd-cups-consumer.bin
# nc -U /var/cups/cups.sock
echo
echo
hello
hello
```

where the double output comes from the server listening on the socket echoing 
back the input.