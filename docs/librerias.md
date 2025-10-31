# Librerias

### Python Standard Library  
- The `re` module, which provides functions used for searching for patterns in log files  
- The `csv` module, which provides functions used when working with .csv files  
- The `glob` and `os` modules, which provide functions used when interacting with the command line  
- The `time` and `datetime` modules, which provide functions used when working with timestamps
- `statistics`

### Import

```py
import statistics
monthly_failed_attempts = [20, 17, 178, 33, 15, 21, 19, 29, 32, 15, 25, 19]
mean_failed_attempts = statistics.mean(monthly_failed_attempts)
print("mean:", mean_failed_attempts)
```  
`mean: 35.25`  
  
### Importar solo modulos
```py
from statistics import mean, median
monthly_failed_attempts = [20, 17, 178, 33, 15, 21, 19, 29, 32, 15, 25, 19]
mean_failed_attempts = mean(monthly_failed_attempts)
print("mean:", mean_failed_attempts)
median_failed_attempts = median(monthly_failed_attempts)
print("median:", median_failed_attempts)
```
`mean: 35.25`  
`median: 20.5`  

---

## Librerias externas
Ejemplo: _Beautiful Soup (bs4)_ for parsing HTML files and _NumPy (numpy)_ for arrays and mathematical computations.  
En bash:  
`%pip install numpy`  
luego ya se puede utilizar en py
```py
import numpy
```


