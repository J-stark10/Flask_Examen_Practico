# 🖥️ Inventario Tec

Sistema de gestión de inventario para una tienda de tecnología, desarrollado con **Flask** y **SQLite**, interfaz con **Bootstrap 5** en tema oscuro azulado.

## 👤 Autor

Desarrollado como proyecto práctico para el curso **TEM-742**.

---

## 📁 Estructura del Proyecto

```
inventario_tec/
├── app.py                  # Aplicación principal Flask
├── requirements.txt        # Dependencias del proyecto
├── .gitignore
├── static/
│   └── style.css           # Estilos personalizados (tema oscuro)
└── templates/
    ├── base.html           # Plantilla base (herencia Jinja2)
    ├── index.html          # Listado de productos
    ├── create.html         # Formulario de registro
    └── edit.html           # Formulario de edición
```

---

## ⚙️ Requisitos

- Python 3.8 o superior
- pip

---

## 🚀 Instalación y Ejecución

**1. Clona el repositorio**

```bash
git clone https://github.com/J-stark10/Flask_Examen_Practico.git
cd inventario-tec
```

**2. Crea y activa el entorno virtual**

```bash
# Crear entorno virtual
python -m venv venv

# Activar en Windows
venv\Scripts\activate

# Activar en Linux / macOS
source venv/bin/activate
```

**3. Instala las dependencias**

```bash
pip install -r requirements.txt
```

**4. Ejecuta la aplicación**

```bash
python app.py
```

**5. Abre en el navegador**

```
http://127.0.0.1:5000
```

> La base de datos `inventario.db` se crea automáticamente al iniciar la app.

---

## 🗄️ Base de Datos

Base de datos: `inventario.db` (SQLite)  
Tabla: `productos`

| Campo       | Tipo    | Descripción                      |
| ----------- | ------- | -------------------------------- |
| `id`        | INTEGER | Clave primaria, autoincrement    |
| `nombre`    | TEXT    | Nombre del producto (no nulo)    |
| `categoria` | TEXT    | Categoría del producto (no nulo) |
| `precio`    | REAL    | Precio en Bs. (no nulo)          |
| `stock`     | INTEGER | Cantidad en stock (no nulo)      |

---

## 🎨 Tecnologías Utilizadas

| Tecnología      | Uso                     |
| --------------- | ----------------------- |
| Python / Flask  | Backend y enrutamiento  |
| SQLite          | Base de datos local     |
| Jinja2          | Motor de plantillas     |
| Bootstrap 5     | Componentes UI y layout |
| Bootstrap Icons | Iconografía             |
| CSS custom      | Tema oscuro azulado     |
