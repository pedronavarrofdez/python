# Parsing
## .split()
```py
approved_users = "elarson,bmoreno,tshah,sgilmore,eraab"
approved_users = approved_users.split(",")
print("after .split():", approved_users)
```
`after .split(): ['elarson', 'bmoreno', 'tshah', 'sgilmore', 'eraab']`  

</br>

```py
removed_users = "wjaffrey jsoto abernard jhill awilliam"
print("before .split():", removed_users)
removed_users = removed_users.split()
print("after .split():", removed_users)
```
`before .split(): wjaffrey jsoto abernard jhill awilliam`  
`after .split(): ['wjaffrey', 'jsoto', 'abernard', 'jhill', 'awilliam']`  

### Applying .split() to files
```py
with open("update_log.txt", "r") as file:
    updates = file.read()
updates = updates.split()
```
Se abre y se convierte en variable acabada en `.read()`. Luego se separa con .split().  

## .join()
Lo contrario, une todo:  
```py
approved_users = ["elarson", "bmoreno", "tshah", "sgilmore", "eraab"]
print("before .join():", approved_users)
approved_users = ",".join(approved_users)
print("after .join():", approved_users)
```
`before .join(): ['elarson', 'bmoreno', 'tshah', 'sgilmore', 'eraab']`  
`after .join(): elarson,bmoreno,tshah,sgilmore,eraab`  

### Applying .join() to files
Despues de operar en la variable `updates` quizas quiera pasarlo al documento `"update_log.txt"`  
Para ello usamos el comando open pero con `"w"`.
```py
updates = " ".join(updates)
with open("update_log.txt", "w") as file:
    file.write(updates)
```
