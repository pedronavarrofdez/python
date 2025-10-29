# Basicos de Python
`#` para comentarios  
## Data type
- String: "cualqui3r sEcueNcia de caract3res" 
- List: [12, 36, 54, 1, 7] o [15, "approved", True, 45.5, False]  
- Integer: "-100" o "69"
- Float: "-2.2" o "45.3" o "0.0" o "0.34"
- Boolean: "True" o "False"
- Tuple data: como una lista pero no se puede modificar   
- Set: {"jlanksy", "drosas", "nmason"} valores unicos no se pueden repetir
- Dictionary:
```py
{ 1: "East",

  2: "West",

  3: "North",

  4: "South" }
```

---

## Asignar variables
Usar nombres sencillos para las variables
```py
username = "nzhao"
old_username = username
username = "zhao2"
print("Previous username:", old_username)
print("Current username:", username)
```
  
`Previous username: nzhao`  
`Current username: zhao2`  

---

## Codigo comprobar tipo de variable
```py
device_id = "72e08x0"
device_id_type = type(device_id)
print(device_id_type)
```
`<class 'str'>`  

---

## Condicionales
`==` igual  
`!=` distinto  
`<` , `>`, `<=`, `>=`  

## IF | ELSE | ELIF
```py
if status == 200:
    print("OK")
elif status == 500:
    print("Bad Request")
else:
    print("check other status")
```
## AND | OR | NOT
```py
if status >= 200 and status <= 226:
    print("successful response")
```
```py
if status == 100 or status == 102:
    print("informational response")
```  
```py
if not(status >= 200 and status <= 226):
    print("check status")
```  

