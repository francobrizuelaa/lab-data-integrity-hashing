# lab-data-integrity-hashing
#  Integridad de Datos: Prueba de Concepto con Hashing

###  Resumen del Lab
Este proyecto documenta una prueba práctica sobre el principio de **Integridad** (Tríada CIA). El objetivo fue demostrar el "Efecto Avalancha" en criptografía: cómo una modificación imperceptible en un archivo altera radicalmente su firma digital (Hash).

###  Herramientas Utilizadas
* **Entorno:** Linux (Ubuntu Virtual Machine).
* **Algoritmo:** SHA-256 (Secure Hash Algorithm 256-bit).
* **Comandos:** `sha256sum`, `echo`, `Output Redirection`.

---

###  Procedimiento y Evidencia

1. **Estado Original:** Se creó un archivo simulando una base de datos crítica (`usuarios.db`) y se calculó su hash inicial (`08266...`).
2. **Compromiso de Integridad:** Se simuló una alteración de datos inyectando un solo caracter al final del archivo.
3. **Verificación:** Se recalculó el hash (`24906...`), evidenciando un cambio total en la firma.

####  Captura de Pantalla de la Terminal
En la siguiente imagen se observa la ejecución de los comandos y el cambio de hash:

![Evidencia del Lab](evidencia.png)

---

###  Conclusión Técnica
Este laboratorio demuestra la importancia del **Hashing** en ciberseguridad. Cualquier modificación no autorizada en un archivo o base de datos rompe la integridad de la firma digital, alertando inmediatamente sobre el incidente.
