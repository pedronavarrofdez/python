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




