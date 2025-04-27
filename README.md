# Infraestructura moderna con Podman y Traefik

Este repositorio contiene la configuración y los despliegues utilizados para construir una infraestructura moderna, segura y rootless basada en **Podman** y **Traefik**.

Todo el proceso está documentado en una serie de entradas en mi blog.

---

## 🛠️ Tecnologías utilizadas

- **Podman** (Contenedores rootless)
- **Podman Compose** (Orquestación estilo Docker Compose)
- **Traefik** (Proxy inverso dinámico)
- **Debian** como sistema base

---

## 📚 Serie de posts en el blog

- [Introducción a la infraestructura con Podman y Traefik](https://TU_DOMINIO.COM/infraestructura-moderna-podman-traefik)
- [Primeros pasos: Montando Traefik como Reverse Proxy](https://TU_DOMINIO.COM/primeros-pasos-traefik-podman-compose)

*(El listado se irá actualizando a medida que avance la serie)*

---

## 📂 Estructura del proyecto

infraestructura/ 
└── traefik/ 
├── podman-compose.yml 
├── .gitignore 
└── README.md


---

## 🚀 Primeros pasos

1. Clona el repositorio:
   ```bash
   git clone https://github.com/cristotodev/infraestructura-podman-traefik.git
   ```

2. Entra en la carpeta
    ```bash
    cd infraestructura/traefik
    ```

3. Levanta los servicios
    ```bash
    podman-compose up -d
    ```

## 🛡️ Notas importantes

-   Actualmente estamos utilizando el puerto `8081` en lugar del `80` por limitaciones de usuarios rootless.
    
-   El dashboard de Traefik está habilitado de forma insegura por ahora para facilitar pruebas iniciales.
    
-   Próximamente se implementará autenticación básica y configuración de HTTPS automático.
## 📜 Licencia

Este proyecto se publica bajo la licencia MIT.
