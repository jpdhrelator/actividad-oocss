# Actividad: El Sistema de Alertas


## Escenario 
Estás construyendo un dashboard administrativo. Tienes dos tipos de mensajes para el usuario: "Éxito" (cuando guarda un dato) y "Error" (cuando falla la conexión).


Actualmente, el código CSS está duplicado y es difícil de mantener.

```css

/* --- CÓDIGO MALO (SIN OOCSS) --- */

.mensaje-exito {
  /* Estructura (Repetido) */
  padding: 15px;
  margin-bottom: 20px;
  border: 1px solid transparent;
  border-radius: 4px;
  font-family: sans-serif;
  /* Apariencia (Único) */
  color: #155724;
  background-color: #d4edda;
  border-color: #c3e6cb;
}

.mensaje-error {
  /* Estructura (Repetido) */
  padding: 15px;
  margin-bottom: 20px;
  border: 1px solid transparent;
  border-radius: 4px;
  font-family: sans-serif;
  /* Apariencia (Único) */
  color: #721c24;
  background-color: #f8d7da;
  border-color: #f5c6cb;
}
````


###  Tu Misión (Instrucciones)

Tu tarea es reescribir ese CSS aplicando OOCSS en tu editor de código o mentalmente:

1. Crea una clase base llamada .alert que contenga solo la estructura (las propiedades que se repiten en ambos). Piensa en esto como tu "Clase Padre" o "Abstract Class" en Java.

2. Crea dos clases modificadoras llamadas .alert-success y .alert-error que contengan solo la apariencia (colores).

Escribe cómo quedaría el HTML para mostrar un mensaje de error usando tus nuevas clases.