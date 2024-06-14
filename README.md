markdown
Copiar código
```mermaid
%%{init: {'theme': 'base', 'themeVariables': { 'primaryColor': '#ffcc00', 'edgeLabelBackground':'#ffffee', 'secondaryColor':'#ff9900', 'tertiaryColor':'#ffcc00', 'lineColor':'#ff9900'}}}%%
actor Profesor
actor Administrador
actor SistemaDeAutenticacion
actor Impresora

SistemaDeAutenticacion --|> Profesor : Identificación del Profesor

Profesor --> (Completar Acta con Notas)
Profesor --> (Añadir/Borrar Alumno en Acta)
Profesor --> (Integrar Actas de Grupos)
Profesor --> (Consultar Información del Alumno)
Profesor --> (Generar Estadísticas de Calificaciones)
Profesor --> (Consultar Porcentajes de Presentados y No Presentados)
Profesor --> (Visualizar Gráfico de Calificaciones)
Profesor --> (Calculadora para Notas)
Profesor --> (Importar/Exportar Lista de Alumnos y Calificaciones)
Profesor --> Impresora : Imprimir Actas y Listas Provisionales

Administrador --> (Gestionar Alumnos)
Administrador --> (Gestionar Asignaturas)
Administrador --> (Gestionar Titulaciones)
Administrador --> (Gestionar Grupos)
Administrador --> (Consultar Alumnos No Matriculables)
Administrador --> (Consultar Historial Académico del Alumno)
