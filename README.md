# Libertad · Libro de mantenimiento

Panel de mantenimiento del velero **Libertad** (Bénéteau Océanis 393, motor Volvo Penta D2-55). Es una página web en un único archivo (`index.html`) y no necesita servidor, base de datos ni dependencias.

## Funciones

- Semáforo de revisiones periódicas: vencidas, próximas (aviso a 30, 60 o 90 días), al día y sin fecha.
- Alertas de vencimientos y de arreglos de prioridad alta.
- Registro de revisiones hechas: calcula la próxima fecha según la periodicidad y, si se indica un coste, lo añade a Gastos.
- Arreglos pendientes con prioridad y estado (pendiente, a revisar, hecho).
- Gastos por año con gráfico.
- Lista de compras.
- Ficha técnica del motor.

## Publicar en GitHub Pages

1. Crea un repositorio y sube `index.html` (y este README) a la raíz.
2. Ve a **Settings → Pages → Build and deployment** y en *Source* elige `Deploy from a branch`.
3. Selecciona la rama `main` y la carpeta `/ (root)`, y guarda.
4. En uno o dos minutos la página estará en `https://<usuario>.github.io/<repositorio>/`.

## Dónde se guardan los datos

- Los datos iniciales van incluidos en `index.html` y proceden de `0_MANTENIMIENTO_INVENTARIO_GASTOS LIBERTAD.xlsx` (17-10-2026).
- Los cambios se guardan en el navegador (`localStorage`) del dispositivo que uses. No se sincronizan entre el ordenador y el móvil.
- Para pasar los cambios a otro dispositivo, o para tener copia de seguridad, usa **Exportar copia (JSON)** e **Importar copia** al pie de la página.
- **Restaurar datos del Excel** vuelve a los datos iniciales incluidos en el archivo.

## Privacidad

Si el repositorio es público, cualquiera puede leer los datos incluidos en `index.html`: gastos, proveedores y notas. En la cuenta gratuita de GitHub, Pages solo funciona con repositorios públicos. Para mantenerlo privado hace falta un plan de pago, o bien usar el archivo en local o subirlo sin datos personales.

---
Diego Estévez García · ADENDA
