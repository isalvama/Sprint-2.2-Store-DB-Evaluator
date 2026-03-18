# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 25 correctas de 62 queries

## ✅ Query 1: Correcto

⏱ Tiempo: 0.37 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.32 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 3: Incorrecto
```diff
--- 
+++ 
@@ -1,12 +1,5 @@
-codigo | nombre | precio | codigo_fabricante
-1.00 | Disco duro SATA3 1TB | 86.99 | 5.00
-2.00 | Memoria RAM DDR4 8GB | 120.00 | 6.00
-3.00 | Disco SSD 1 TB | 150.99 | 4.00
-4.00 | GeForce GTX 1050Ti | 185.00 | 7.00
-5.00 | GeForce GTX 1080 Xtreme | 755.00 | 6.00
-6.00 | Monitor 24 LED Full HD | 202.00 | 1.00
-7.00 | Monitor 27 LED Full HD | 245.99 | 1.00
-8.00 | Portátil Yoga 520 | 559.00 | 2.00
-9.00 | Portátil Ideapd 320 | 444.00 | 2.00
-10.00 | Impresora HP Deskjet 3720 | 59.99 | 3.00
-11.00 | Impresora HP Laserjet Pro M26nw | 180.00 | 3.00
+Field | Type | Null | Key | Default | Extra
+codigo | int unsigned | NO | PRI | NULL | auto_increment
+nombre | varchar(100) | NO |  | NULL | 
+precio | double | NO |  | NULL | 
+codigo_fabricante | int unsigned | NO | MUL | NULL | 
```

## ❌ Query 3: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'SHOW COLUMNS FROM tienda.producto' at line 2


## ✅ Query 4: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 5: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nom del producte | euros | dòlars
+nombre | euros | dòlars
 Disco duro SATA3 1TB | 86.99 | 95.69
 Memoria RAM DDR4 8GB | 120.00 | 132.00
 Disco SSD 1 TB | 150.99 | 166.09
```

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 7: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 8: Correcto

⏱ Tiempo: 0.32 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 10: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 11: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 12: Correcto

⏱ Tiempo: 0.31 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ✅ Query 13: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 14: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 15: Correcto

⏱ Tiempo: 0.33 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 16: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ❌ Query 17: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,3 @@
 codigo | nombre
+3.00 | Hewlett-Packard
 4.00 | Samsung
-5.00 | Seagate
```

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 18: Correcto

⏱ Tiempo: 0.33 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 19: Correcto

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 20: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,2 @@
 nombre
-Portátil Yoga 520
-Portátil Ideapd 320
+Lenovo
```

⏱ Tiempo: 0.31 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 21: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'del fabricante FROM tienda.producto p JOIN tienda.fabricante f ON p.codigo_fabri' at line 2


## ❌ Query 22: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'del fabricante FROM tienda.producto p JOIN tienda.fabricante f ON p.codigo_fabri' at line 2


## ❌ Query 23: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'del fabricante FROM tienda.producto p JOIN tienda.fabricante f ON p.codigo_fabri' at line 2


## ✅ Query 24: Correcto

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ✅ Query 25: Correcto

⏱ Tiempo: 0.41 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ✅ Query 26: Correcto

⏱ Tiempo: 0.42 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ✅ Query 27: Correcto

⏱ Tiempo: 0.42 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 28: Incorrecto
```diff
--- 
+++ 
@@ -1,6 +1,3 @@
 nombre | precio | fabricante
-Disco duro SATA3 1TB | 86.99 | Seagate
 Monitor 24 LED Full HD | 202.00 | Asus
 Monitor 27 LED Full HD | 245.99 | Asus
-Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
-Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
```

⏱ Tiempo: 0.44 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ✅ Query 29: Correcto

⏱ Tiempo: 0.44 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ✅ Query 30: Correcto

⏱ Tiempo: 0.43 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ✅ Query 31: Correcto

⏱ Tiempo: 0.42 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ✅ Query 32: Correcto

⏱ Tiempo: 0.44 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 33: Incorrecto
```diff
--- 
+++ 
@@ -1,8 +1,12 @@
 codigo | nombre
 1.00 | Asus
+1.00 | Asus
 2.00 | Lenovo
+2.00 | Lenovo
+3.00 | Hewlett-Packard
 3.00 | Hewlett-Packard
 4.00 | Samsung
 5.00 | Seagate
 6.00 | Crucial
+6.00 | Crucial
 7.00 | Gigabyte
```

⏱ Tiempo: 0.42 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 34: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-fabricante | producto
+nombre | producto
 Asus | Monitor 27 LED Full HD
 Asus | Monitor 24 LED Full HD
 Lenovo | Portátil Ideapd 320
```

⏱ Tiempo: 0.47 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ✅ Query 35: Correcto

⏱ Tiempo: 0.47 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ❌ Query 36: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,3 @@
-codigo | nombre | precio | codigo_fabricante
-8.00 | Portátil Yoga 520 | 559.00 | 2.00
-9.00 | Portátil Ideapd 320 | 444.00 | 2.00
+nombre
+Portátil Yoga 520
+Portátil Ideapd 320
```

⏱ Tiempo: 0.40 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 37: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,3 @@
-codigo | nombre | precio | codigo_fabricante
-8.00 | Portátil Yoga 520 | 559.00 | 2.00
+codigo | nombre | precio | codigo_fabricante | codigo | nombre
+8.00 | Portátil Yoga 520 | 559.00 | 2.00 | 2.00 | Lenovo
+9.00 | Portátil Ideapd 320 | 444.00 | 2.00 | 2.00 | Lenovo
```

## ❌ Query 37: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 38: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 39: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 40: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 41: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 42: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 43: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 44: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 45: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 46: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 47: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 48: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 49: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 50: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 51: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 52: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 53: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 54: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 55: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 56: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 57: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 58: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 59: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 60: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 61: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now


## ❌ Query 62: Error
- **Descripción**: 2014 (HY000): Commands out of sync; you can't run this command now

