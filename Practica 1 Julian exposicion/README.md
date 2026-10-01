# Práctica 1 - Aplicación Base en Angular

## 1. Descripción del Proyecto
Este proyecto corresponde a la **Práctica 1** desarrollada en clase de *Desarrollo de interfaces*. Consiste en una aplicación web frontend creada con el framework **Angular**, estructurada mediante componentes reutilizables y enrutamiento modular.

---

## 2. Tecnologías Empleadas
Para consultar más información sobre la plataforma base, puedes visitar la [Documentación Oficial de Angular](https://angular.dev).

| Herramienta | Versión / Tipo | Función principal |
| :--- | :--- | :--- |
| **Angular CLI** | Versión reciente | Creación de componentes y gestión del proyecto |
| **TypeScript** | Lenguaje tipado | Lógica de negocio y definición de clases |
| **HTML5 & CSS3** | Vistas y maquetación | Estructura visual y estilos de interfaz |
| **Vite / Node.js** | Servidor local | Compilación rápida y desarrollo |

---

## 3. Tareas y Objetivos Realizados
Estado de los hitos completados durante la práctica:

- [x] Instalación del entorno con Node.js y Angular CLI.
- [x] Inicialización del proyecto `practica1`.
- [x] Configuración del componente principal (`app.component`).
- [x] Comprobación de arranque en servidor de desarrollo.
- [ ] Conectar con un backend externo mediante HttpClient.

---

## 4. Captura de la Aplicación
A continuación se muestra una captura de pantalla del proyecto funcionando en el navegador:

![Vista de la aplicación](https://angular.dev/assets/images/press-kit/angular_wordmark_gradient.png)

---

## 5. Código Destacado del Proyecto

Para levantar el servidor de desarrollo y visualizar la app en `http://localhost:4200/` se ejecuta:
`ng serve`

### Componente Principal (`src/app/app.component.ts`)
```typescript
import { Component } from '@angular/core';
import { RouterOutlet } from '@angular/router';

@Component({
  selector: 'app-root',
  standalone: true,
  imports: [RouterOutlet],
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  title = 'practica1';
}