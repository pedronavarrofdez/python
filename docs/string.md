# String

### Bracket notation
```py
device_id = "h32rb17"
print("h32rb17"[0])
print(device_id[0])
```  
`h`  
`h`  

</br>

```py
print("h32rb17"[0:3])
```
`h32`  

---

### str() and len()
Pasar a string un numero  
```py
string_id = str(19329302)
```  

</br>

```py
device_id_length = len("h32rb17")
if device_id_length == 7:
    print("The device ID has 7 characters.")
```  
`The device ID has 7 characters.`  

---

### .upper() and .lower()
`"Information Technology".upper()`  
> "INFORMATION TECHNOLOGY"

</br>

`"Information Technology".lower()`  
> "information technology"

---

### .index()
```py
print("h32rb17".index("r"))
```
> 3

</br>

```py
print("r45rt46".index("r"))
```
> 0

---

### Finding substrings with .index()

```py
tshah_index = "tsnow, tshah, bmoreno - updated".index("tshah")
print(tshah_index)
```  
> 7

