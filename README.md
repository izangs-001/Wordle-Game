# 🎮 WORDLE GAME - Juego de Palabras

¡Bienvenido al **Wordle Game**! Un juego de palabras donde debes adivinar una palabra secreta de 5 letras en 6 intentos.

## 🎯 ¿Qué es Wordle?

**Wordle** es un juego de palabras donde debes adivinar una palabra oculta de 5 letras.

### Reglas del Juego

1. **Objetivo:** Adivinar la palabra secreta de 5 letras
2. **Intentos:** Tienes 6 oportunidades
3. **Feedback:** Después de cada intento, el juego te indica:

| Color | Significado |
|-------|-------------|
| 🟩 **Verde** | Letra correcta en posición correcta |
| 🟨 **Amarillo** | Letra está en la palabra, pero en otra posición |
| ⬜ **Gris** | Letra no está en la palabra |

### Ejemplo de Partida

```
Palabra secreta: VERDE

Intento 1:  P I Z A R  →  ⬜🟨⬜⬜🟩  (I y R están en la palabra)
Intento 2:  L I M O N  →  🟩⬜⬜🟨⬜  (I correcta, O y N presentes)
Intento 3:  I D I O M  →  ⬜⬜🟨⬜⬜  (O está en la palabra)
Intento 4:  B O T O N  →  ⬜🟩🟩🟩🟩  (Casi perfecta!)
Intento 5:  V E R D E  →  🟩🟩🟩🟩🟩  ¡GANASTE!
```

### Características de este Juego

- ✅ **Sistema de usuarios** - Regístrate y guarda tu progreso
- ✅ **Estadísticas** - Tracking de partidas ganadas/perdidas
- ✅ **Persistencia** - Tus datos se guardan permanentemente
- ✅ **Validación** - 5,757 palabras válidas en español
- ✅ **Responsive** - Funciona en PC, tablet y móvil

---

## 🚀 Instalar el Juego

### Paso 1: Extraer los Archivos

1. Si descargaste el ZIP, **extrae el contenido** en una carpeta
2. La carpeta debe contener:
   ```
   wordle-para-compartir/
   ├── docker-compose.yml
   ├── .env.example
   ├── start.ps1
   ├── start.bat
   ├── wordle.ps1
   ├── wordle.bat
   └── backend/
       ├── main.py
       ├── Dockerfile
       ├── requirements.txt
       ├── data/wordle_words.txt
       ├── static/script.js
       ├── static/style.css
       └── templates/index.html
   ```

### Paso 2: Abrir la Carpeta

1. Abre el **Explorador de Archivos**
2. Navega a la carpeta donde extrajiste los archivos
3. Deberías ver los archivos listados

### Paso 3: Abrir PowerShell en la Carpeta

**Opción A - Click Derecho:**
1. Click derecho en un espacio vacío de la carpeta
2. Selecciona **"Abrir en Terminal"** o **"Abrir ventana de PowerShell aquí"**

**Opción B - Desde el Menú:**
1. Haz clic en la barra de direcciones del explorador
2. Escribe `powershell` y presiona Enter

### Paso 4: Ejecutar el Script de Inicio

En PowerShell, escribe:

```powershell
Entrar a la ruta de la carpeta con cd /ruta/a/la/carpeta
.\start.ps1
```

**Si da error de permisos**, ejecuta:

```powershell
powershell -ExecutionPolicy Bypass -File .\start.ps1
```

### Paso 5: Esperar a que se Instale

El script hará lo siguiente automáticamente:

1. ✅ Verifica que Docker esté instalado y ejecutándose
2. ✅ Crea la configuración necesaria
3. ✅ Descarga las imágenes de Docker (primera vez: ~500 MB)
4. ✅ Construye los contenedores
5. ✅ Inicia el juego

**Tiempo estimado:**
- **Primera vez:** 3-5 minutos (descarga de imágenes)
- **Siguientes veces:** 10-20 segundos

### Paso 6: Acceder al Juego

Cuando veas el mensaje **"WORDLE GAME LISTO"**, abre tu navegador web y ve a:

```
http://localhost
```
---

## 🎮 Primeros Pasos

### 1. Registrarse

1. En la página principal, haz clic en **"Registrarse"**
2. Ingresa un **nombre de usuario** (3-20 caracteres, solo letras, números y guiones bajos)
3. Ingresa una **contraseña** (mínimo 4 caracteres)
4. Haz clic en **"Registrarse"**

### 2. Iniciar Sesión

1. Ingresa tu **usuario** y **contraseña**
2. Haz clic en **"Iniciar Sesión"**

### 3. Jugar

1. **Escribe** una palabra de 5 letras en el teclado o usando el teclado en pantalla
2. **Presiona Enter** o haz clic en **"Adivinar"**
3. **Analiza** los colores para saber qué letras están correctas
4. **Repite** hasta adivinar la palabra (máximo 6 intentos)

### 4. Ver Estadísticas

Después de cada partida, puedes ver:
- **Partidas jugadas**
- **Partidas ganadas**
- **Porcentaje de victorias**
- **Historial de partidas**

## 🏆 Consejos para Jugar

1. **Empieza con vocales:** Usa palabras con muchas vocales (A, E, I, O, U)
2. **Letras comunes:** R, S, T, L, N son las más frecuentes en español
3. **Analiza los colores:**
   - 🟩 Verde = Mantén la letra en esa posición
   - 🟨 Amarillo = Usa la letra pero en otra posición
   - ⬜ Gris = No uses esa letra de nuevo
4. **No repitas letras grises:** Si una letra es gris, no la uses de nuevo
5. **Piensa en patrones:** Muchas palabras terminan en -CIÓN, -DAD, -MENTE

---

## 💾 Tus Datos se Guardan

- ✅ **Usuarios registrados** - No necesitas registrarte cada vez
- ✅ **Contraseñas** - Encriptadas de forma segura
- ✅ **Partidas jugadas** - Historial completo
- ✅ **Estadísticas** - Victorias, derrotas, porcentaje

**Los datos se guardan permanentemente** mientras no elimines los contenedores con `docker compose down -v`.

---

## 🎉 ¡A Jugar!

¡Ya estás listo para disfrutar del **Wordle Game**!

**Accede ahora:** http://localhost

**¡Buena suerte y que comience el juego! 🎮**

---


