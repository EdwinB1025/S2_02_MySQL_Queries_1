# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 22 correctas de 41 queries

## ✅ Query 1: Correcto

⏱ Tiempo: 0.38 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.27 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 3: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ❌ Query 4: Incorrecto
```diff
--- 
+++ 
@@ -1,12 +1,12 @@
 nombre | precio_eur | precio_usd
-Disco duro SATA3 1TB | 86.99 | 86.99
-Memoria RAM DDR4 8GB | 120.00 | 120.00
-Disco SSD 1 TB | 150.99 | 150.99
-GeForce GTX 1050Ti | 185.00 | 185.00
-GeForce GTX 1080 Xtreme | 755.00 | 755.00
-Monitor 24 LED Full HD | 202.00 | 202.00
-Monitor 27 LED Full HD | 245.99 | 245.99
-Portátil Yoga 520 | 559.00 | 559.00
-Portátil Ideapd 320 | 444.00 | 444.00
-Impresora HP Deskjet 3720 | 59.99 | 59.99
-Impresora HP Laserjet Pro M26nw | 180.00 | 180.00
+Disco duro SATA3 1TB | 86.99 €  | 86.99 $	
+Memoria RAM DDR4 8GB | 120 €  | 120 $	
+Disco SSD 1 TB | 150.99 €  | 150.99 $	
+GeForce GTX 1050Ti | 185 €  | 185 $	
+GeForce GTX 1080 Xtreme | 755 €  | 755 $	
+Monitor 24 LED Full HD | 202 €  | 202 $	
+Monitor 27 LED Full HD | 245.99 €  | 245.99 $	
+Portátil Yoga 520 | 559 €  | 559 $	
+Portátil Ideapd 320 | 444 €  | 444 $	
+Impresora HP Deskjet 3720 | 59.99 €  | 59.99 $	
+Impresora HP Laserjet Pro M26nw | 180 €  | 180 $	
```

⏱ Tiempo: 0.27 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 5: Incorrecto
```diff
--- 
+++ 
@@ -1,12 +1,12 @@
-nom del producte | euros | dòlars
-Disco duro SATA3 1TB | 86.99 | 95.69
-Memoria RAM DDR4 8GB | 120.00 | 132.00
-Disco SSD 1 TB | 150.99 | 166.09
-GeForce GTX 1050Ti | 185.00 | 203.50
-GeForce GTX 1080 Xtreme | 755.00 | 830.50
-Monitor 24 LED Full HD | 202.00 | 222.20
-Monitor 27 LED Full HD | 245.99 | 270.59
-Portátil Yoga 520 | 559.00 | 614.90
-Portátil Ideapd 320 | 444.00 | 488.40
-Impresora HP Deskjet 3720 | 59.99 | 65.99
-Impresora HP Laserjet Pro M26nw | 180.00 | 198.00
+nombre | precio_eur | precio_usd
+Disco duro SATA3 1TB | 86.99 €  | 95.69 $	
+Memoria RAM DDR4 8GB | 120.00 €  | 132.00 $	
+Disco SSD 1 TB | 150.99 €  | 166.09 $	
+GeForce GTX 1050Ti | 185.00 €  | 203.50 $	
+GeForce GTX 1080 Xtreme | 755.00 €  | 830.50 $	
+Monitor 24 LED Full HD | 202.00 €  | 222.20 $	
+Monitor 27 LED Full HD | 245.99 €  | 270.59 $	
+Portátil Yoga 520 | 559.00 €  | 614.90 $	
+Portátil Ideapd 320 | 444.00 €  | 488.40 $	
+Impresora HP Deskjet 3720 | 59.99 €  | 65.99 $	
+Impresora HP Laserjet Pro M26nw | 180.00 €  | 198.00 $	
```

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 6: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nombre | precio
+UPPER(nombre) | precio
 DISCO DURO SATA3 1TB | 86.99
 MEMORIA RAM DDR4 8GB | 120.00
 DISCO SSD 1 TB | 150.99
```

⏱ Tiempo: 0.28 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 7: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nombre | precio
+LOWER(nombre) | precio
 disco duro sata3 1tb | 86.99
 memoria ram ddr4 8gb | 120.00
 disco ssd 1 tb | 150.99
```

⏱ Tiempo: 0.28 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 8: Correcto

⏱ Tiempo: 0.28 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 9: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nombre | precio
+nombre | ROUND(precio)
 Disco duro SATA3 1TB | 87.00
 Memoria RAM DDR4 8GB | 120.00
 Disco SSD 1 TB | 151.00
```

⏱ Tiempo: 0.27 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 10: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nombre | precio truncado
+nombre | TRUNCATE(precio,0)
 Disco duro SATA3 1TB | 86.00
 Memoria RAM DDR4 8GB | 120.00
 Disco SSD 1 TB | 150.00
```

⏱ Tiempo: 0.26 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 11: Correcto

⏱ Tiempo: 0.30 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 12: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-codigo_fabricante
+codigo
 1.00
 2.00
 3.00
```

⏱ Tiempo: 0.29 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ✅ Query 13: Correcto

⏱ Tiempo: 0.27 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 14: Correcto

⏱ Tiempo: 0.26 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 15: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 16: Correcto

⏱ Tiempo: 0.25 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 17: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 18: Correcto

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 19: Correcto

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 20: Correcto

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ✅ Query 21: Correcto

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 22: Incorrecto
```diff
--- 
+++ 
@@ -1,12 +1,12 @@
 nombre | precio | nombre del fabricante
+Disco duro SATA3 1TB | 86.99 | Seagate
+Disco SSD 1 TB | 150.99 | Samsung
+GeForce GTX 1050Ti | 185.00 | Gigabyte
+GeForce GTX 1080 Xtreme | 755.00 | Crucial
+Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
+Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
+Memoria RAM DDR4 8GB | 120.00 | Crucial
 Monitor 24 LED Full HD | 202.00 | Asus
 Monitor 27 LED Full HD | 245.99 | Asus
-Memoria RAM DDR4 8GB | 120.00 | Crucial
-GeForce GTX 1080 Xtreme | 755.00 | Crucial
-GeForce GTX 1050Ti | 185.00 | Gigabyte
-Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
-Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
+Portátil Ideapd 320 | 444.00 | Lenovo
 Portátil Yoga 520 | 559.00 | Lenovo
-Portátil Ideapd 320 | 444.00 | Lenovo
-Disco SSD 1 TB | 150.99 | Samsung
-Disco duro SATA3 1TB | 86.99 | Seagate
```

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 23: Incorrecto
```diff
--- 
+++ 
@@ -1,12 +1,12 @@
-codigo | nombre | codigo fabricante | nombre fabricante
-1.00 | Disco duro SATA3 1TB | 5.00 | Seagate
-2.00 | Memoria RAM DDR4 8GB | 6.00 | Crucial
-3.00 | Disco SSD 1 TB | 4.00 | Samsung
-4.00 | GeForce GTX 1050Ti | 7.00 | Gigabyte
-5.00 | GeForce GTX 1080 Xtreme | 6.00 | Crucial
-6.00 | Monitor 24 LED Full HD | 1.00 | Asus
-7.00 | Monitor 27 LED Full HD | 1.00 | Asus
-8.00 | Portátil Yoga 520 | 2.00 | Lenovo
-9.00 | Portátil Ideapd 320 | 2.00 | Lenovo
-10.00 | Impresora HP Deskjet 3720 | 3.00 | Hewlett-Packard
-11.00 | Impresora HP Laserjet Pro M26nw | 3.00 | Hewlett-Packard
+nombre | precio | codigo del fabricante | nombre del fabricante
+Disco duro SATA3 1TB | 86.99 | 5.00 | Seagate
+Memoria RAM DDR4 8GB | 120.00 | 6.00 | Crucial
+Disco SSD 1 TB | 150.99 | 4.00 | Samsung
+GeForce GTX 1050Ti | 185.00 | 7.00 | Gigabyte
+GeForce GTX 1080 Xtreme | 755.00 | 6.00 | Crucial
+Monitor 24 LED Full HD | 202.00 | 1.00 | Asus
+Monitor 27 LED Full HD | 245.99 | 1.00 | Asus
+Portátil Yoga 520 | 559.00 | 2.00 | Lenovo
+Portátil Ideapd 320 | 444.00 | 2.00 | Lenovo
+Impresora HP Deskjet 3720 | 59.99 | 3.00 | Hewlett-Packard
+Impresora HP Laserjet Pro M26nw | 180.00 | 3.00 | Hewlett-Packard
```

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 24: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,2 @@
-nombre | precio | fabricant
+nombre | precio | nombre del fabricante
 Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
```

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 25: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,2 @@
-nombre | precio | fabricante
+nombre | precio | nombre del fabricante
 GeForce GTX 1080 Xtreme | 755.00 | Crucial
```

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 26: Correcto

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ✅ Query 27: Correcto

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 28: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nombre | precio | fabricante
+nombre | precio | nombre del fabricante
 Disco duro SATA3 1TB | 86.99 | Seagate
 Monitor 24 LED Full HD | 202.00 | Asus
 Monitor 27 LED Full HD | 245.99 | Asus
```

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 29: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nombre | precio | fabricante
+nombre | precio | nombre del fabricante
 Disco duro SATA3 1TB | 86.99 | Seagate
 Monitor 24 LED Full HD | 202.00 | Asus
 Monitor 27 LED Full HD | 245.99 | Asus
```

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

🚨 **Problemas detectados:**
⚠️ Considerar `EXISTS` en lugar de `IN` para eficiencia.

---

## ❌ Query 30: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,3 @@
-nombre | precio | fabricante
+nombre | precio | nombre del fabricante
 Disco duro SATA3 1TB | 86.99 | Seagate
 GeForce GTX 1050Ti | 185.00 | Gigabyte
```

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 31: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,2 @@
-nombre | precio | fabricante
-Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
+nombre | precio | nombre del fabricante
 Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
```

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 32: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nombre | precio | fabricante
+nombre | precio | nombre del fabricante
 GeForce GTX 1080 Xtreme | 755.00 | Crucial
 Portátil Yoga 520 | 559.00 | Lenovo
 Portátil Ideapd 320 | 444.00 | Lenovo
```

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 33: Correcto

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 34: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-fabricante | producto
+nombre | nombre del producto
 Asus | Monitor 27 LED Full HD
 Asus | Monitor 24 LED Full HD
 Lenovo | Portátil Ideapd 320
@@ -10,5 +10,5 @@
 Crucial | GeForce GTX 1080 Xtreme
 Crucial | Memoria RAM DDR4 8GB
 Gigabyte | GeForce GTX 1050Ti
-Huawei | NULL
-Xiaomi | NULL
+Huawei | Sin producto
+Xiaomi | Sin producto
```

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ❌ Query 35: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,3 @@
-fabricante
+nombre
 Huawei
 Xiaomi
```

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ✅ Query 36: Correcto

⏱ Tiempo: 0.38 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 37: Correcto

⏱ Tiempo: 0.40 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 38: Correcto

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ✅ Query 39: Correcto

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ✅ Query 40: Correcto

⏱ Tiempo: 0.37 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ❌ Query 41: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,2 @@
-codigo | nombre | precio | codigo_fabricante
-7.00 | Monitor 27 LED Full HD | 245.99 | 1.00
+nombre | precio
+Monitor 27 LED Full HD | 245.99
```

⏱ Tiempo: 0.42 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---
