# Automatización: Lista de Espera Quirúrgica (Comunidad de Madrid)

## Contenido

- `lista_espera.py`: Script principal en Python
- `lista_espera.xlsx`: Archivo Excel donde se guardarán los datos
- Esta guía rápida (`README.md`)

## Requisitos

1. Tener Python 3 instalado.
2. Instalar las librerías necesarias:

```
pip install playwright openpyxl
playwright install
```

## Cómo usar

1. Abre `config.example.json` y cambia:
  "fecha_nacimiento": "DD/MM/AAAA", # fecha de nacimiento con este formato.
  "codigo": ["BLOQUE1", "BLOQUE2", "BLOQUE3", "BLOQUE4"], # 4 bloques de 5 dígitos
  "email": "tu_correo@gmail.com", # Cambiar por el tuyo
  "contrasena": "tu_contraseña_de_aplicacion", # Contraseña de aplicación
  "destinatario": "destino@gmail.com" # Destino del aviso

2. Ejecuta el script con:

```
python lista_espera.py
```

3. Se abrirá un navegador en segundo plano, iniciará sesión y extraerá el número.
4. El resultado se guardará en `lista_espera.xlsx`.

## Automatizar (opcional)

Puedes usar el Programador de Tareas de Windows o `cron` en Linux para ejecutarlo diariamente.
