# Basicos de Python
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



