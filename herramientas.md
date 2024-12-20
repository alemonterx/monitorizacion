# MONITORIZACIÓN DE PROCESOS

## COMANDO PS

> El comando `ps` en Linux muestra información sobre los procesos en ejecución

*ps aux*

![COMANDO ps aux](img/psaux.png)

- Este comando muestra información detallada de todos los procesos del sistema, incluidos los que no están asociados a terminales, junto con datos como usuario, uso de CPU y memoria.

---

*ps -C nano*

![COMAND ps -C](img/psCnano.png)

- Este comando muestra información específica sobre los procesos cuyo nombre coincida exactamente con `nano`.

---

*ps -eo user,pid,$cpu,%mem,time --sort=-%cpu | head -n 6*

![COMANDO ps -eo](img/pseo.png)

- Este comando muestra los 6 procesos principales (incluyendo el encabezado) ordenados por el uso de CPU en orden descendente, con información del usuario, PID, porcentaje de CPU y memoria utilizada, y el tiempo de ejecución del proceso.

---

## COMANDO TOP

> El comando `top` en Linux muestra en tiempo real los procesos en ejecución y el uso de recursos del sistema, como CPU, memoria y carga promedio.

![COMANDO top](img/top.png)

---

*top -b -n 1 > top.txt*

![COMANDO top -b -n 1 > top.txt](img/topbn.png)

> Este comando ejecuta `top` en modo batch (sin interacción) y captura una sola instantánea de los procesos en ejecución, redirigiendo la salida al archivo **top.txt**

---

## COMANDO ATOP

> El comando `atop` en Linux es una herramienta de monitoreo de rendimiento que muestra estadísticas detalladas sobre el uso de recursos del sistema, como CPU, memoria, disco, red y procesos, en tiempo real y con la capacidad de registrar estos datos.

![COMANDO atop](img/atop.png)

---

## COMANDO HTOP

> El comando `htop` en Linux es una herramienta interactiva que muestra una vista en tiempo real de los procesos en ejecución, similar a top, pero con una interfaz más amigable y visual, permitiendo gestionar procesos, ordenar información y ver el uso de recursos como CPU, memoria y red de manera más detallada.

![COMANDO htop](img/htop.png)
