## Integrantes:
Nilson Diaz Hasbun
Sergio Rodríguez
David Maury

# Simulación de Ransomware - Examen Final de Criptografía

Este proyecto es una simulación educativa de un ransomware como parte del examen final del curso de **Criptografía** en la Universidad del Norte. La simulación se enfoca en demostrar los conceptos criptográficos vistos en clase y no representa una amenaza real.

## 🔐 Funcionalidades implementadas

1. **Generación de certificados digitales** usando RSA 2048 bits.
2. **Protocolo AKE v.2** para establecer un secreto común entre víctima y atacante:
   - Cifrado asimétrico con `PKCS1_OAEP`
   - Firmas digitales con `pkcs1_15` y `SHA256`
3. **Derivación de llave simétrica** a partir del secreto usando una KDF.
4. **Cifrado de archivos** reales usando `AES-CBC`.
5. **Verificación de integridad** de los archivos mediante hash SHA-256.
6. **Simulación de descifrado** tras el "pago" del rescate.
7. **Preguntas de reflexión**: rol del atacante y del defensor.

## 📁 Estructura del proyecto

- `simulacion_ransomware_final.ipynb`: Notebook principal con la simulación completa.
- `requirements.txt`: Dependencias necesarias para ejecutar el proyecto.
- `victima_archivos/`: Carpeta con archivos a cifrar (se descarga desde Google Drive al iniciar el notebook).
- `README.md`: Este archivo.

## ▶️ Cómo ejecutar el proyecto

```
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
pip install -r requirements.txt
```
