# Instalar y configurar Obsidian paso a paso

Esta guía te acompaña desde la instalación hasta tu primera nota conectada. Está pensada para seguir el mini curso en un ordenador con Windows, macOS o Linux.

**Resultado:** un vault abierto, notas organizadas, enlaces funcionando y plantillas y diario preparados para practicar.

Esta guía forma parte del vault **00-empieza-aqui**. Desde [Home](Home.md) puedes recorrer la [estructura de carpetas y sus ejemplos](01-ESTRUCTURA-DEL-VAULT.md). Los ajustes básicos, las plantillas y las notas de ejemplo ya están incluidos; los pasos siguientes te enseñan a revisarlos y reproducirlos en tu propio vault.

## 1. Instala Obsidian

1. Entra en la [descarga oficial de Obsidian](https://obsidian.md/download).
2. Elige tu sistema operativo:
   - **Windows:** descarga el instalador, ejecútalo y sigue el asistente.
   - **macOS:** descarga y abre el archivo `.dmg`; arrastra Obsidian a Aplicaciones.
   - **Linux:** elige uno de los paquetes disponibles y sigue las instrucciones para ese formato en la [guía oficial de instalación](https://obsidian.md/help/install).
3. Abre la aplicación.

## 2. Descarga el material del curso

Desde la página del repositorio en GitHub:

1. Pulsa **Code → Download ZIP**.
2. Extrae el ZIP completamente.
3. Guarda la carpeta extraída en un lugar fácil de encontrar, por ejemplo `Documentos/Cursos/Obsidian`.

Si ya usas Git, puedes clonar el repositorio con la URL que muestra **Code**. Ambas opciones sirven para seguir el curso.

Dentro encontrarás varias carpetas numeradas. **Cada carpeta es un vault independiente.** Para comenzar, utiliza `00-empieza-aqui`.

## 3. Abre el primer vault

Un **vault** o **bóveda** es una carpeta que contiene tus notas y la configuración de Obsidian.

1. En la pantalla inicial, busca **Abrir carpeta como bóveda / Open folder as vault**.
2. Pulsa **Abrir / Open**.
3. Selecciona la carpeta `00-empieza-aqui` que acabas de extraer.
4. Confirma y comprueba que aparecen `00 Inbox`, `04 Knowledge` y `Home` en el explorador lateral.
5. Abre la nota **00-INSTALAR-Y-CONFIGURAR-OBSIDIAN** para continuar esta guía dentro de Obsidian.

Si ya tienes otra bóveda abierta, utiliza el selector de bóvedas de la esquina inferior izquierda y entra en **Manage Vaults…**, o busca **Open another vault** en la paleta de comandos.

**Selecciona la carpeta numerada, no la carpeta que contiene todo el repositorio.** Así, los enlaces se resuelven dentro del ejemplo del módulo y no se mezclan notas con el mismo nombre de otros vaults. En el segundo ejemplo, selecciona la carpeta exterior `02-linked-knowledge`, que contiene `README.md` y `04 Knowledge`.

Consulta: [gestión de bóvedas](https://obsidian.md/help/manage-vaults).

## 4. Ajusta idioma y editor

Los nombres de los menús pueden variar ligeramente según la versión y el idioma. Incluimos referencias en inglés para encontrarlos.

1. Abre **Ajustes / Settings** con el icono de engranaje.
2. En **General → Language**, selecciona **Español**. Reinicia si la aplicación lo solicita.
3. En **Editor**, elige **Live Preview / Vista previa en vivo** como modo de edición predeterminado.
4. En **Apariencia / Appearance**, ajusta el tema claro u oscuro y el tamaño del texto a tu gusto.

## 5. Configura dónde se guardan las notas

En el explorador de Obsidian, crea estas carpetas con **Nueva carpeta** si todavía no existen:

```text
00 Inbox
03 Resources
  Attachments
Templates
Daily Notes
```

En **Ajustes → Archivos y enlaces / Files and links**:

| Opción | Valor para practicar |
| --- | --- |
| Ubicación predeterminada de notas nuevas | En la carpeta especificada: `00 Inbox` |
| Ubicación predeterminada de adjuntos nuevos | En la carpeta especificada: `03 Resources/Attachments` |
| Actualizar enlaces internos automáticamente | Activado |
| Usar Wikilinks | Activado, para escribir enlaces como `[[Nombre de nota]]` |

Los ajustes del vault se guardan en su carpeta `.obsidian`; configura cada bóveda que utilices. Referencias: [ajustes](https://obsidian.md/help/settings) y [carpeta de configuración](https://obsidian.md/help/configuration-folder).

## 6. Activa las funciones del curso

En **Ajustes → Complementos principales / Core plugins**, comprueba que están activos:

- Explorador de archivos y búsqueda.
- Selector rápido y paleta de comandos.
- Enlaces entrantes / Backlinks y vista de grafo / Graph view.
- Plantillas / Templates y notas diarias / Daily notes.

Estos ejercicios usan funciones incluidas en Obsidian. Puedes mantener el **modo restringido** de los complementos de la comunidad. Consulta los [ajustes de complementos](https://obsidian.md/help/settings).

## 7. Crea dos notas y conéctalas

1. Crea una nota llamada **Prueba de instalación** con el botón de nueva nota del explorador. Comprueba que queda en `00 Inbox`.
2. Escribe este contenido:

```markdown
# Prueba de instalación

Estoy preparando mi sistema de notas para el curso.

- [x] Abrir el vault
- [ ] Practicar los enlaces

Mi siguiente paso es [[Mi objetivo con Obsidian]].

#practica
```

3. Abre el enlace `Mi objetivo con Obsidian` desde la vista de lectura. Si la nota todavía no existe, Obsidian la creará. Escribe qué te gustaría organizar con esta herramienta.
4. Con esa segunda nota abierta, muestra el panel **Backlinks**. Debe aparecer una referencia desde `Prueba de instalación`.
5. Abre **Graph view** desde la paleta de comandos y localiza ambas notas conectadas.

La paleta se abre con `Ctrl+P` en Windows/Linux o `Cmd+P` en macOS. Busca el nombre de la función; los comandos se muestran en el idioma de tu aplicación.

Referencia: [cómo consultar los backlinks](https://obsidian.md/help/Plugins/Backlinks) y [vista de grafo](https://obsidian.md/help/Plugins/Graph+view).

## 8. Prepara una plantilla

1. En **Ajustes → Templates**, selecciona `Templates` como carpeta de plantillas.
2. Configura fecha `YYYY-MM-DD` y hora `HH:mm`.
3. Dentro de `Templates`, abre **Nota de aprendizaje**, ya incluida en este vault. Si estás configurando otra bóveda, créala con este contenido:

```markdown
# {{title}}

Fecha: {{date:YYYY-MM-DD}}

## Qué aprendí

## Cómo lo voy a aplicar

## Próximo paso

- [ ] Probarlo en un ejemplo
```

4. Crea una nota vacía llamada **Aprendiendo Obsidian**.
5. Con el cursor en el cuerpo de esa nota, abre la paleta y ejecuta **Templates: Insert template** o su equivalente en español.
6. Selecciona **Nota de aprendizaje**. Comprueba que el título y la fecha sustituyen a las variables.

Los vaults `03-developer-workflow` y `05-final-demo-vault` ya incluyen `Research Note` y `Feature Note`: puedes insertarlas del mismo modo.

Referencia: [plantillas de Obsidian](https://obsidian.md/help/Plugins/Templates).

## 9. Configura las notas diarias

1. Dentro de `Templates`, crea **Daily Note** si no existe:

```markdown
# {{date:YYYY-MM-DD}}

## Hoy quiero avanzar en

- [ ]

## Lo que aprendí

## Ideas para retomar
```

2. En **Ajustes → Daily notes**, configura:
   - **Date format:** `YYYY-MM-DD`.
   - **New file location:** `Daily Notes`.
   - **Template file location:** selecciona `Templates/Daily Note`.
3. Ejecuta **Open today's daily note** desde la paleta, o pulsa el icono del calendario.
4. Comprueba que la nota está en `Daily Notes` y anota una tarea.

Si la nota de hoy ya existía, se abrirá con su contenido anterior: la plantilla solo se aplica al crear una nota diaria nueva. Puedes insertarla manualmente con el comando de plantillas.

En `06-second-brain-sdd` estos ajustes ya vienen configurados y la plantilla `Templates/Daily Note` está incluida: no hace falta crear nada.

Referencia: [notas diarias](https://obsidian.md/help/Plugins/Daily+notes).

## 10. Continúa con el curso

Abre otra carpeta numerada como bóveda cuando cambies de módulo. Para volver a consultar esta guía, abre de nuevo `00-empieza-aqui` desde el selector de bóvedas.

| Carpeta | Uso |
| --- | --- |
| `00-empieza-aqui` | Esta guía, ajustes básicos y estructura de ejemplo |
| `01-obsidian-basics` | Primeras notas, Markdown y organización |
| `02-linked-knowledge` | Enlaces, backlinks y grafo |
| `03-developer-workflow` | Captura de ideas, plantillas y diario |
| `04-obsidian-sdd` | Conocimiento, especificaciones y decisiones |
| `05-final-demo-vault` | Ejemplo integrado para el cierre |
| `06-second-brain-sdd` | Segundo cerebro completo: SDD, agentic harness, ADRs, specs y plantillas. Empieza por `Home` |

## Si algo no funciona

| Síntoma | Qué comprobar |
| --- | --- |
| No aparecen las notas del curso | Extrae el ZIP y abre la carpeta numerada que contiene los archivos `.md`. |
| Veo varias notas iguales | Comprueba que abriste un solo vault y no la raíz del repositorio. |
| Un enlace abre una nota vacía | El destino aún no existe o su nombre no coincide. En las plantillas, `[[nota]]` es un marcador para sustituir. |
| No encuentro Templates o Daily notes | Activa el complemento principal correspondiente. |
| La lista de plantillas está vacía | Selecciona `Templates` en los ajustes y crea una nota dentro de esa carpeta. |
| Las variables siguen apareciendo como `{{title}}` | Inserta la plantilla mediante el comando; copiar y pegar su texto no sustituye las variables. |
| La nota diaria está vacía | Revisa la plantilla seleccionada y si la nota ya existía antes de configurarla. |
| No encuentro una carpeta vacía al descargar el repo | Git no conserva carpetas vacías; créala desde el explorador de Obsidian. |

## Comprobación final

- [ ] Abro un vault del curso y encuentro esta guía dentro de Obsidian.
- [ ] Las notas nuevas se guardan en `00 Inbox`.
- [ ] Puedo conectar dos notas y ver su backlink.
- [ ] Puedo insertar una plantilla con título y fecha.
- [ ] Puedo abrir mi nota diaria en `Daily Notes`.

Guía revisada el 10 de septiembre de 2026 con la documentación oficial enlazada en cada apartado.
