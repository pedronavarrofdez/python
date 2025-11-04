# Import
## Opening files in Python
Para abrir el documento `"update_log.txt"`:  
```py
with open("update_log.txt", "r") as file:
```  

### open()
El documento a abrir tiene que estar en el mismo directorio que el archivo de python.  
Si no: 
```py
with open("/home/analyst/logs/access_log.txt", "r") as file:
```

## Read, write, a
### read
Metodo `.read()` convierte el contenido del documento en un string.  
```py
with open("update_log.txt", "r") as file:
    updates = file.read()
print(updates)
```  
Una vez convertido en string puedes aplicar [*Strings*](docs/string.md)

### write
Lo contrario, convierte de python a documento. Usa o `w` o `a`   
```py
line = "jrafael,192.168.243.140,4:56:27,True"
with open("access_log.txt", "a") as file:
    file.write(line)
```
