# Lists
### Concatenar o unir listas
```py
lista_uno = [1, 2, 3, 4]
lista_dos = ["pero", "manzana", "cuatro", "gato"]

print(lista_uno + lista_dos)
```
> 1, 2, 3, 4, pero, manzana, cuatro, gato.

### Bracket notation
```py
username_list = ["elarson", "fgarcia", "tshah", "sgilmore"]
print(username_list[2])
```
> tshah

</br>

```py
print(["elarson", "fgarcia", "tshah", "sgilmore"][2])
```  
> tshah  

---

### Extracting a slice from a list
```py
username_list = ["elarson", "fgarcia", "tshah", "sgilmore"]
print(username_list[0:2])
```
> ['elarson', 'fgarcia']

---

### Changing the elements in a list

```py
username_list = ["elarson", "fgarcia", "tshah", "sgilmore"]
print("Before changing an element:", username_list)
username_list[1] = "bmoreno"
print("After changing an element:", username_list)
```

`Before changing an element: ['elarson', 'fgarcia', 'tshah', 'sgilmore']`  
`After changing an element: ['elarson', 'bmoreno', 'tshah', 'sgilmore']`  

---

## List methods
List methods are functions that are specific to the list data type.  
These include the `.insert()` , `.remove()`, `.append()` and `.index()`. 

### .insert()
Inserta en la lista.
```py
username_list = ["elarson", "bmoreno", "tshah", "sgilmore"]
print("Before inserting an element:", username_list)
username_list.insert(2,"wjaffrey")
print("After inserting an element:", username_list)
```
`Before inserting an element: ['elarson', 'bmoreno', 'tshah', 'sgilmore']`  
`After inserting an element: ['elarson', 'bmoreno', 'wjaffrey', 'tshah', 'sgilmore']`  

---

### .remove()
Borra de la lista.
```py
username_list = ["elarson", "bmoreno", "wjaffrey", "tshah", "sgilmore"]
print("Before removing an element:", username_list)
username_list.remove("elarson")
print("After removing an element:", username_list)
```
`Before removing an element: ['elarson', 'bmoreno', 'wjaffrey', 'tshah', 'sgilmore']`  
`After removing an element: ['bmoreno', 'wjaffrey', 'tshah', 'sgilmore']`  

---

### .append() 
Añade al final de la lista.
```py
username_list = ["bmoreno", "wjaffrey", "tshah", "sgilmore"]
print("Before appending an element:", username_list)
username_list.append("btang")
print("After appending an element:", username_list)
```  
`Before appending an element: ['bmoreno', 'wjaffrey', 'tshah', 'sgilmore']`  
`After appending an element: ['bmoreno', 'wjaffrey', 'tshah', 'sgilmore', 'btang']`  

</br>

> [!NOTE]
> Append method is often used with for loops to populate an empty list with elements.  
> You can explore how this works with the following code:  

```py
numbers_list = []
print("Before appending a sequence of numbers:", numbers_list)
for i in range(10):
    numbers_list.append(i)
print("After appending a sequence of numbers:", numbers_list)
```
`Before appending a sequence of numbers: []`  
`After appending a sequence of numbers: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]`  

---

### .index()
Igual que con strings pero en vez de caracteres busca palabras completas.  
```py
username_list = ["bmoreno", "wjaffrey", "tshah", "sgilmore", "btang"]
username_index = username_list.index("tshah")
print(username_index)
```
> 2 

---
