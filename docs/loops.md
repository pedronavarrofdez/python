# LOOPS
## FOR
- 1
```py
for i in ["elarson", "bmoreno", "tshah", "sgilmore"]:
    print(i)
```
`elarson`  
`bmoreno`  
`tshah`  
`sgilmore`  

---

- 2
```py
computer_assets = ["laptop1", "desktop20", "smartphone03"]
for asset in computer_assets:
    print(asset)
```
`laptop1`  
`desktop20`  
`smartphone03`  

- 2 (string de letras  )
```py
string = "security"
for character in string:
    print(character)
```
`s`  
`e`  
`c`  
`u`  
`r`  
`i`  
`t`  
`y`  

---

- USING RANGE 
```py
for i in range(0, 5):
    print(i)
```
`0`  
`1`  
`2`  
`3`  
`4`  

- lo mismo
```py
for i in range(5):
    print(i)
```
`misma salida que antes`  

---

## WHILE

- 1
```py
i = 1
while i < 5:
    print(i)
    i = i + 1
```
`1`  
`2`  
`3`  
`4`  

---

- integers
```py
login_attempts = 0
while login_attempts < 5:
    print("Login attempts:", login_attempts)
    login_attempts = login_attempts + 1
```
`Login attempts: 0`  
`Login attempts: 1`  
`Login attempts: 2`  
`Login attempts: 3`  
`Login attempts: 4`  

---

- Boolean
```py
count = 0
login_status = True
while login_status == True:
    print("Try again.")
    count = count + 1
    if count == 4:
        login_status = False
```
`Try again.`  
`Try again.`  
`Try again.`  
`Try again.`  

---

### BREAK

```py
computer_assets = ["laptop1", "desktop20", "smartphone03"]
for asset in computer_assets:
    if asset == "desktop20":
        break
    print(asset)
```
`laptop1`  

### CONTINUE
```py
computer_assets = ["laptop1", "desktop20", "smartphone03"]
for asset in computer_assets:
    if asset == "desktop20":
        continue
    print(asset)
```
`laptop1`  
`smartphone03`  


