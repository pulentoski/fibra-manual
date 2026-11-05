# ⚡ Manual Técnico Operativo: Termofusión de Fibra Óptica

**Asignatura:** Infraestructura de Redes  
**Docente:** [Nombre del Docente]  
**Sede:** La Serena | **Institución:** Inacap  
**Autor:** Daniel Ruz  

---

## 📄 1. Glosario Técnico de Trabajo

* **Núcleo (Core):** Centro de vidrio por donde viaja el haz de luz.
* **Cladding (Revestimiento):** Capa de vidrio exterior ($125\,\mu m$) que mantiene la luz dentro del núcleo.
* **Acrilato / Buffer:** Capas plásticas de protección ($250\,\mu m$ / $900\,\mu m$) que deben retirarse antes de cortar el vidrio.
* **Stripping:** Proceso de pelado mecánico para expeler las protecciones plásticas.
* **Cleaving:** Corte de precisión perpendicular ($\approx 90^\circ$) sobre la fibra desnuda.
* **V-Grooves (Bloques V):** Ranuras mecánicas en la fusionadora para alinear las fibras.
* **Heat Shrink:** Manguito termocontraíble con alma de acero para proteger el empalme.
* **Pérdida por Inserción ($IL$):** Pérdida de potencia de luz introducida por la fusión (medida en $dB$).

---

## 🛠️ 2. Herramientas y Materiales de Laboratorio

| Herramienta / Material | Función Principal |
| :--- | :--- |
| **Fusionadora de Arco** ⚡ | Alineación de núcleos y fusión por descarga eléctrica. |
| **Cortadora (Cleaver)** 🔪 | Corte transversal plano de alta precisión sobre vidrio desnudo. |
| **Pinza Stripper (Miller)** ✂️ | Decapado de chaqueta, buffer ($900\,\mu m$) y acrilato ($250\,\mu m$). |
| **Alcohol Isopropílico y Paños** 🧴 | Descontaminación de grasas e impurezas en el vidrio. |
| **Protector Termocontraíble** 🛡️ | Refuerzo estructural del empalme (colocar *antes* de fusionar). |
| **Contenedor Rígido de Residuos** 🗑️ | Depósito exclusivo para fragmentos de fibra sobrantes. |

---

## ⚠️ 3. Reglas de Seguridad Específicas

1. 🥽 **Protección Ocular:** Usar gafas de seguridad en todo momento.
2. 📌 **Manejo de Residuos:** Tirar **cada trozo de fibra cortada inmediatamente** en el contenedor rígido. Nunca dejarlos en la mesa o el suelo.
3. 🚫 **No Comer ni Beber:** Previene la ingestión accidental de micropartículas de vidrio.
4. 🔥 **Manipulación de Alcohol:** Mantener el alcohol isopropílico lejos del arco eléctrico de la fusionadora.

---

## 🔄 4. Procedimiento Operativo Paso a Paso

```text
 1. Insertar Manga 🛡️ ➔ 2. Pelado (Stripping) ✂️ ➔ 3. Limpieza 🧴
                                                         │
 6. Curado en Horno 🔥  5. Fusión por Arco ⚡  4. Corte (Cleaving) 🔪
```

### 1️⃣ Inserción del Protector Termocontraíble
* Introducir el manguito *heat shrink* en uno de los extremos de la fibra.  
* 💡 *Tip:* Si olvidas este paso antes de fusionar, tendrás que romper el empalme y repetir todo.

### 2️⃣ Pelado de la Fibra (*Stripping*)
* Usar la muesca adecuada de la pinza *stripper* para retirar el buffer y el acrilato hasta exponer el vidrio desnudo ($125\,\mu m$).
* Desnudar entre $30\,\text{mm}$ y $40\,\text{mm}$ de longitud total.
* ⚠️ *Atención:* Mantener la pinza recta a $90^\circ$ para no mellar ni fisurar el vidrio.

### 3️⃣ Limpieza de Precisión
* Humedecer un paño libre de pelusa con alcohol isopropílico.
* Limpiar la fibra desnuda desde el límite del recubrimiento hacia la punta en **una sola dirección**.
* ⚠️ *Atención:* No pasar el paño hacia atrás ni volver a tocar la fibra con los dedos.

### 4️⃣ Corte de Precisión (*Cleaving*)
* Acomodar la fibra limpia en las guías del *cleaver*, dejando el borde del acrilato en la marca indicada por la máquina ($10\,\text{mm}$ a $16\,\text{mm}$).
* Accionar la cuchilla con un movimiento firme y constante.
* 📸 *(Insertar imagen de corte en la carpeta `assets/img/corte_bueno.png`)*

### 5️⃣ Alineación y Termofusión
* Colocar los extremos de las fibras cortadas sobre las ranuras en "V" (*V-grooves*) de la fusionadora.
* Asegurarse de que las puntas queden cerca de los electrodos sin chocarlos ni cruzarlos.
* Cerrar la tapa y presionar **SET / AUTO**. La máquina alineará las fibras, aplicará la descarga eléctrica y estimará la pérdida ($IL$).

### 6️⃣ Protección y Curado Térmico
* Abrir la cubierta, retirar la fibra con cuidado y deslizar el manguito *heat shrink* sobre la zona descubierta del empalme.
* Colocar el ensamble en el horno integrado de la fusionadora y activar el ciclo de calentamiento.

---

## 🔍 5. Control de Calidad e Inspección

* **Visual en Pantalla:** La unión debe verse recta y cilíndrica, sin deformaciones ni líneas marcadas en el punto de contacto.
* **Pérdida Estimada:** Comprobar que el valor mostrado por la fusionadora sea menor a **$0.02\,\text{dB}$**.
* **Prueba de Continuidad (VFL):** Inyectar luz con el localizador visual de fallas (láser rojo); no debe haber fuga brillante de luz en la zona del empalme.

---

## 🛠️ 6. Guía Diagnóstica de Fallas (*Troubleshooting*)

| Pantalla de Fusionadora | Causa Probable | Acción Correctiva |
| :--- | :--- | :--- |
| 🫧 **Burbuja en el Empalme** | Fibra sucia, húmeda o con aire atrapado. | Repelar, limpiar bien con alcohol y volver a cortar. |
| 🪓 **Ángulo de Corte Alto (> 1.0°)** | Cuchilla del *cleaver* sucia o gastada. | Limpiar la cuchilla o rotar la posición de corte. |
| 🔀 **Error de Alineación (Eje X/Y)** | Suciedad o polvo en los *V-grooves*. | Limpiar las ranuras V con un hisopo seco o alcohol. |
| 🥪 **Empalme Grueso o Abultado** | Exceso de avance mecánico al fusionar. | Ajustar parámetros de motor o recalibrar arco. |
| ⏳ **Empalme Delgado / Separado** | Corriente de arco muy alta o falta de avance. | Ejcutar rutina de calibración de arco (*Arc Calibrate*). |

---

## 📋 7. Registro de Prácticas de Laboratorio

| Empalme N° | Tipo de Fibra | Ángulo Izq. | Ángulo Der. | Pérdida ($dB$) | Resultado | Observaciones |
| :---: | :---: | :---: | :---: | :---: | :---: | :--- |
| **01** | SM (OS2) | 0.3° | 0.4° | 0.01 dB | ✅ Aprobado | Fusión limpia y centrada. |
| **02** | SM (OS2) | 1.3° | 0.4° | -- | ❌ Rechazado | Ángulo alto; se repitió corte. |
| **03** | | | | | | |
| **04** | | | | | | |

---

## 📚 8. Referencias
* Estándares internacionales **ITU-T G.652** y **TIA-568-C.3**.
* Manuales de operación de fusionadoras de fibra óptica.