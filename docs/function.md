# Function

```py
# Esta parte define la funcion
def display_investigation_message():
    print("investigate activity")
# Para que se "active" hay que llamarla
display_investigation_message()
```

ejemplo:    
```py
# funcion
def display_investigation_message():
    print("investigate activity")

# Variables
application_status = "potential concern"
email_status = "okay"

# "Codigo"
if application_status == "potential concern":
    print("application_log:")
    display_investigation_message()

if email_status == "potential concern":
    print("email log:")
```
> output

`application_log:`  
`investigate activity`  

---

## Return

```py
# Define la funcion
def remaining_login_attempts(maximum_attempts, total_attempts):
    return maximum_attempts - total_attempts

# Nombra variable global con el resultado de la variable local.
remaining_attempts = remaining_login_attempts(3, 3)

# if de vuelta
if remaining_attempts <= 0:
    print("Your account is locked")
```

> [!NOTE]
> Las variables locales (dentro de la funcion) solo funcionan dentro, por eso se asigna a una global.  

```py
username = "elarson"
print("1:" + username)
def greet():
    username = "bmoreno"
    print("2:" + username)
greet()
print("3:" + username)
```  
> output  
`1:elarson`  
`2:bmoreno`  
`3:elarson`  

---


