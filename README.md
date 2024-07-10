# Zoom-Polyphone-ZTP
Onboarding Poly Z series phone to Zoom Phone

Configuring DHCP server option [Reference](https://h30434.www3.hp.com/t5/Desk-and-IP-Conference-Phones/FAQ-Do-Poly-Phones-support-the-DHCP-Option-60-Vendor-Data/td-p/9006061)
```
Define vendor-class=Poly-EdgeE350
option 161 https://provpp.zoom.us/api/v2/pbx/provisioning/Polycom/edge-e350
```

Below is the configuration to configure Poly Edge-Z series IP Phone to auto connect wifi during ZTP.
Modify countryCode, SSID name and SSID Password for your environment.

```
sec.pwd.length.admin="1"
sec.pwd.length.user="1"
device.auth.localAdminPassword="123456"
device.auth.localAdminPassword.set="1"
device.auth.localUserPassword="654321"
device.auth.localUserPassword.set="1"
device.wifi.enabled="1"
device.wifi.enabled.set="1"
device.wifi.country="XX"
device.wifi.country.set="1"
device.wifi.dhcpEnabled="1"
device.wifi.dhcpEnabled.set="1"
device.wifi.ssid="WIFINAME"
device.wifi.ssid.set="1"
device.wifi.securityMode="WPA2-PSK"
device.wifi.psk.key="WIFIPASSWORD"
device.wifi.psk.key.set="1"
device.wifi.securityMode.set="1"
```

Poly IP Phone Edge-Z series configuration document attached.
