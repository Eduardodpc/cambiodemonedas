# 💱 Conversor de Monedas en Java

Este es un proyecto en **Java** que implementa un conversor de monedas en consola, utilizando la API pública de [exchangerate.host](https://exchangerate.host) para obtener tasas de cambio en tiempo real.

## 🚀 Características
- Conversión en **tiempo real** consultando una API gratuita.
- Uso de `HttpClient` (Java 11+).
- Parseo de JSON con la librería **Gson**.
- Filtro de monedas disponibles usando su **Currency Code**.
- Manejo de errores al consultar la API.

## 💵 Monedas disponibles
El conversor admite únicamente las siguientes monedas:
- 🇦🇷 **ARS** – Peso argentino  
- 🇧🇴 **BOB** – Boliviano boliviano  
- 🇧🇷 **BRL** – Real brasileño  
- 🇨🇱 **CLP** – Peso chileno  
- 🇨🇴 **COP** – Peso colombiano  
- 🇺🇸 **USD** – Dólar estadounidense  

## 📂 Estructura del proyecto
```
ConversorMonedas/
 ├─ src/
 │   └─ com/ejemplo/conversor/
 │       ├─ Main.java
 │       ├─ CurrencyConverter.java
 │       └─ ExchangeRateResponse.java
 ├─ pom.xml
 └─ README.md
```

## ⚙️ Requisitos
- Java 11 o superior  
- Maven (si deseas compilar con dependencias)  

Dependencia necesaria (en `pom.xml`):
```xml
<dependency>
  <groupId>com.google.code.gson</groupId>
  <artifactId>gson</artifactId>
  <version>2.11.0</version>
</dependency>
```

## ▶️ Ejecución
1. Clona el repositorio:
   ```bash
   git clone https://github.com/tuusuario/ConversorMonedas.git
   cd ConversorMonedas
   ```
2. Compila con Maven:
   ```bash
   mvn compile
   ```
3. Ejecuta el programa:
   ```bash
   mvn exec:java -Dexec.mainClass="com.ejemplo.conversor.Main"
   ```

## 🖥️ Ejemplo de uso
```
=== Conversor de Monedas ===
Monedas disponibles: [ARS, BOB, BRL, CLP, COP, USD]
Ingrese la moneda base: USD
Ingrese la moneda destino: COP
Ingrese el monto a convertir: 20

20.00 USD = 84000.00 COP
```

*(El valor depende de la tasa de cambio actual).*

## 📜 Licencia
Este proyecto es de uso libre para fines educativos.
