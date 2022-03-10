# MAP-Inventory-microsoft



## URL para download
```bash
https://www.microsoft.com/en-us/download/details.aspx?id=7826
```
## Liberar acesso do MAP
```bash
netsh advfirewall set currentprofile settings remotemanagement enable
```
## Salvar modificação
```bash
winrm quickconfig
```
## liberar portas no firewall
```bash
netsh advfirewall firewall add rule name="MAP Rules" dir=in action=allow protocol=TCP localport=53465,49154
```
