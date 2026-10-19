# DAW Project Hub

Pequeña página web para practicar un flujo profesional de trabajo con Git y GitHub.

## Seguridad y archivos ignorados

### 1. ¿Por qué .env.example puede publicarse?

Porque contiene únicamente los nombres de las variables que necesita la aplicación, pero no contiene valores sensibles o secretos reales. Sirve como ejemplo para saber qué información debe configurarse.

### 2. ¿Por qué .env debe ignorarse?

Porque el archivo .env puede contener contraseñas, tokens, claves u otros datos privados. Si se subiera a GitHub, esa información podría quedar expuesta.

### 3. ¿Qué habría que hacer si una contraseña o un token reales se hubieran publicado en GitHub?

Habría que considerar esa información comprometida, revocar o cambiar inmediatamente la contraseña o el token y eliminar el secreto del repositorio y de su historial si fuera necesario.

### 4. ¿Bastaría con eliminar el archivo en un commit posterior?

No. Aunque se elimine posteriormente, el archivo y su contenido pueden seguir estando disponibles en el historial de Git. Por eso habría que cambiar o revocar el secreto y, si fuera necesario, eliminarlo también del historial.