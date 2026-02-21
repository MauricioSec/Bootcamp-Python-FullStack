# 🚀 Formación: Desarrollo Full Stack Python Trainee

Bienvenido a mi bitácora de aprendizaje. Este repositorio documenta mi progreso, apuntes y ejercicios prácticos en mi formación como Desarrollador Full Stack Python. 

Mi objetivo es fusionar mis conocimientos de infraestructura, sistemas lógicos (adquiridos como Oficial de Marina Mercante) y Ciberseguridad, para construir y comprender aplicaciones web robustas desde sus cimientos.

---

## 📚 Índice de Módulos

- [x] **Módulo 1:** Fundamentos de la Lógica y Entorno de Trabajo
- [ ] **Módulo 2:** Estructuras de Datos
- [ ] **Módulo 3:** Programación Orientada a Objetos (POO)
- [ ] **Módulo 4:** Bases de Datos Relacionales
- [ ] **Módulo 5:** Desarrollo Web - Backend
- [ ] **Módulo 6:** Desarrollo Web - Frontend
- [ ] **Módulo 7:** Proyecto Capstone

---

## 🟢 Módulo 1: Fundamentos de la Lógica y Entorno de Trabajo

### Lección 1.1: Introducción al Pensamiento Lógico y Algoritmos
Antes de escribir código, es vital entender cómo "piensa" una computadora. Una máquina es un procesador de **Entradas (Inputs)** que ejecuta instrucciones paso a paso para entregar **Salidas (Outputs)**.

**Concepto Clave: El Algoritmo**
Un algoritmo es una secuencia de pasos ordenados, lógicos y finitos para resolver un problema. Para entrenar el pensamiento procedimental, desarrollé este algoritmo de la vida real aplicando control de flujo y validaciones de estado:

<details>
<summary>☕ Ver Algoritmo: Preparación de un Café Instantáneo (Clic para desplegar)</summary>

1. Ir hasta la cocina.
2. Tomar el hervidor (ubicación: mueble junto al refrigerador).
3. Dirigirse al lavaplatos y abrir la tapa del hervidor.
4. Poner el hervidor bajo la canilla.
5. Levantar la manilla para dar el agua.
6. Llenar hasta la marca de 1.0 L.
7. Bajar la manilla para cortar el agua.
8. Volver y colocar el hervidor en su base original.
9. **[Validación]** Verificar si la base está enchufada:
   - Si no lo está: Enchufar.
   - Si lo está: Presionar botón de encendido (verificar luz de funcionamiento).
10. Abrir el mueble superior, sacar una taza y cerrarlo.
11. Colocar la taza junto a la base del hervidor.
12. Abrir el cajón inferior, sacar una cuchara de café (pequeña, punta ovalada) y cerrarlo.
13. Destapar el tarro de café.
14. Con la cuchara, sacar una porción sin rebalsar y vaciar en la taza. Tapar el tarro.
15. Destapar el frasco de azúcar.
16. **[Bucle]** Sacar una porción de azúcar y vaciar en la taza. Repetir este paso una vez más. Tapar el frasco.
17. **[Bucle de Espera]** Verificar estado del agua:
    - Mientras la luz esté encendida: Esperar.
    - Cuando la luz se apague: El agua está hervida. Continuar.
18. Levantar el hervidor por el mango y acercar a la taza.
19. Verter agua hasta llenar 3/4 de la taza.
20. Devolver el hervidor a su base y desenchufar.
21. Revolver el contenido de la taza con la cuchara por 30 segundos.
22. Retirar la cuchara. El café está listo para servir.
</details>

### Lección 1.2: Entorno de Desarrollo (VS Code + Python)
Para comunicarnos con la máquina utilizamos:
* **El Editor (VS Code):** Nuestra bitácora donde redactamos el código con resaltado de sintaxis para evitar errores visuales.
* **El Intérprete (Python):** El "motor" que traduce nuestras instrucciones (texto plano) a código máquina que el hardware puede procesar.
* **La Terminal:** La consola de mando directa al sistema operativo.

**Primer Script en Python:**
Uso de la función de salida estándar `print()` y comentarios en el código.

```python
# Academia Código Austral - Módulo 1.2
# Alumno: Mauricio Monsálvez

# Esto es una instrucción de salida
print("Iniciando sistemas de navegación...")

# Esto es un cálculo matemático simple impreso en pantalla
print("Calculando rumbo inicial:")
print(10 + 5) 

# Aquí simulamos un error corregido (Python es secuencial)
print("Rumbo: Norte")
print("Corrección: Nor-Noreste")

### Lección 1.3: Variables y Tipos de Datos (Las Bodegas del Barco)
Para que un programa sea útil, necesita "memoria" para guardar y manipular información. En Python, utilizamos **Variables** (contenedores con una etiqueta) y asignamos datos utilizando el signo `=`.

Los datos se clasifican en tipos (para saber qué podemos hacer con ellos):
* `String` (Texto): Siempre entre comillas `""`.
* `Integer` (Enteros): Números para contar, sin comillas.
* `Float` (Decimales): Números con precisión, usan punto `.`.
* `Boolean` (Booleanos): Estados de Verdadero o Falso (`True` / `False`).

**Práctica de Bodega:**
Definición de parámetros iniciales de navegación utilizando diferentes tipos de datos.

```python
# Lección 1.3 - Variables básicas
destino = "Canal de Chacao"         # String
velocidad_nudos = 12                # Integer
combustible_estimado = 1850.5       # Float
buen_clima = True                   # Boolean

print("Destino:", destino)
print("Velocidad en nudos:", velocidad_nudos)
print("Litros estimados de combustible:", combustible_estimado)
print("¿Hay buen clima?:", buen_clima)

# Lección 1.4 - Simulación de consumo de combustible
tanque_total = 5000
consumo_viaje = 1200

# Operador matemático (Resta)
combustible_restante = tanque_total - consumo_viaje

# Operador de comparación (Mayor que)
reserva_segura = combustible_restante > 1000

print("Combustible restante:", combustible_restante)
print("¿Reserva segura disponible?:", reserva_segura)

# Lección 1.5 - Sistema de Alarma de Presión de Aceite
presion_aceite = 25 # Forzamos falla para prueba de estrés

if presion_aceite < 30:
    print("🚨 ALARMA: Presión baja. Detener motor.")
elif presion_aceite > 60:
    print("⚠️ ALARMA: Sobrepresión. Revisar válvulas.")
else:
    print("✅ Presión normal. Continuar navegación.")
