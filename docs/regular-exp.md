# Basics of regular expressions
Primero importar el modulo:  
```py
import re
```
## Regular expression symbols
### Symbols for character types
Ejemplo:   
```py
import re
re.findall("\w", "h32rb17")
```
`['h', '3', '2', 'r', 'b', '1', '7']`  

- **`\w`:** Matches any alphanumeric character (A-z, 0-9) OR an underscore (_).  
EJ: `In "ID_A17", matches I,D,_,A,1,7.`  
- **`\d`:** Matches any single digit (0-9).  
EJ: `In "ID_A17", matches 1,7.`  
- **`\s`:** Matches any single whitespace character (space, tab, newline).  
EJ: `Matches the space in "user 1".`  
- **`.`:** Matches any character (letters, digits, symbols, spaces), except for a newline.  
- **`\.`:** Matches the literal period character (.) The backslash \ is necessary to escape the special meaning of the dot.  

</br>

EJ:
```py
import re
re.findall("\d", "h32rb17")
```  
`['3', '2', '1', '7']`  

---

### Symbols to quantify occurrences
- **`+`:** One or more occurrences. EJ: `\d+ matches 1,12,12345`  
- **`*`:** Zero, one, or more occurrences.  
- **`{n}`:** Exactly n occurrences.
`\d{4} matches four consecutive digits (e.g., 1234).`  
- **`{n,n}`:** Between m (minimum) and n (maximum) occurrences.
`\d{1,3} matches 1,12, or 123.`  

</br>

EJ `+`:  
```py
import re
re.findall("\d+", "h32rb17")
```  
`['32', '17']`  

</br>

EJ `*`:  
```py
import re
re.findall("\d*", "h32rb17")
```
`['', '32', '', '', '17', '']`  

</br>

EJ `{n}`:  
```py
import re
re.findall("\d{2}", "h32rb17 k825t0m c2994eh")
```  
`['32', '17', '82', '29', '94']`  

</br>

EJ `{n,n}`:  
```py
import re
re.findall("\d{1,3}", "h32rb17 k825t0m c2994eh")
```
`['32', '17', '825', '0', '299', '4']`  

```py

```


```py

```


```py

```


```py

```
