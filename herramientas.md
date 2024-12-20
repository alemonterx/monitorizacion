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

- Este comando Muestra los 6 procesos principales (incluyendo el encabezado) ordenados por el uso de CPU en orden descendente, con información del usuario, PID, porcentaje de CPU y memoria utilizada, y el tiempo de ejecución del proceso.
