[PROCESO DE DESARROLLO]
1.- Si el desarrollo se llevará a un workpspace de producción, instalar ahí la versión beta(vtex release patch beta)

[DESPLIGUE][THEME O COMPONENTS]
** Si es un desplige major

1.- Definir bien el ticket de Jira. Los requerimientos, RFC, cambios hechos... (basarse en el ejemplo).

2.- Hacer la revisión del código en los PR, revisando que todo esté en orden, siguiendo las mejores practicas.

3.- ** Revisar que el checkout ui custom que se haya migrado correctamente

4.- vtex release patch stable(el manifest ya incluye el "vtex publish")

5.- vtex install

6.- vtex deploy (este comando propaga los cambios a todos los workspaces, por lo tanto antes de ejecutarlo, asegurate que la versión publicada de tu app funcione correctamente, esto en un workspace de producción).

6.5.- Si fue el release de una versión major, asegurarse que esté bien el workspace de producción.

7.- vtex promote(si es un workspace de producción)

https://developers.vtex.com/docs/guides/vtex-io-documentation-making-your-new-app-version-publicly-available

[DESPLIGUE][CHECKOUT UI CUSTOM]

1.- Revisión de código en el PR

2.- Una vez aprobado el PR, el desarrollardor lleva el código al checkout ui custom de vtex(así cómo el css si se hicieron cambios) al workspace master o productivo.