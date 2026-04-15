# EXAMEN_PRACTICO_2
Descripcion del Proyecto
Sistema en C++ de consola que gestiona pacientes y atenciones de una clinica, con modulo integrado de Ahorcado de dominio clinico.

Metodologia seguida
1.	Fase 1 - Analisis: Se identificaron actores (Paciente, Atencion), variables clave, reglas de negocio (cobertura segun seguro, recargos, prioridad) y casos criticos.
2.	Fase 2 - Diseño: Se definieron las clases Paciente y Atencion con encapsulamiento completo y constructores. Se diseño el menu principal integrador y el sub-menu del Ahorcado.
3.	Fase 3 - Construccion incremental: Primero estructura base, luego registros y validaciones, despues reportes y recursividad, finalmente el modulo Ahorcado.
4.	Fase 4 - Pruebas y depuracion: Se corrigio el fragmento defectuoso calcularPago(), se probaron casos normales y casos limite (cobertura mayor al costo, cedula invalida, etc.).
5.	Fase 5 - Versionamiento: Proyecto gestionado con GitHub Desktop para Windows.
6.	Fase 6 - Cierre: Codigo funcional, README y defensa tecnica lista.

Partes implementadas
Sistema Clinico
•	Registro de pacientes con cedula, edad, sexo, tipo de seguro y antecedente de riesgo
•	Registro de atenciones con especialidad, prioridad, costo, examenes y tiempo de espera
•	Calculo de cobertura segun tipo de seguro (IESS 80%, Privado 60%, Ninguno 0%)
•	Recargo por examenes (20%) y por paciente de riesgo (10%)
•	Busqueda por cedula y por especialidad (manual)
•	Ordenamiento manual por prioridad y por tiempo de espera (algoritmo burbuja)
•	Deteccion de inconsistencias en atenciones criticas
•	Emision de factura detallada con IVA
•	Funcion recursiva: totalAtencionesPaciente() suma costos de manera recursiva
•	Depuracion justificada: funcion calcularPago() corregida con prueba minima
Modulo Ahorcado Clinico
•	Menu propio con 4 opciones
•	Modo 1 vs 1 con multiple rondas y marcador
•	Modo vs CPU
•	Historial de partidas
•	Dos niveles de dificultad (facil y dificil)
•	Palabras del dominio clinico (especialidades, diagnosticos)
•	Validacion de letras, prevencion de repeticion
•	Dibujo ASCII del ahorcado con 6 estados
•	Puntaje acumulado y ganador final

Clases implementadas
•	Paciente: cedula, nombre, edad, sexo, tipoSeguro, riesgo — con constructor, getters y setters
•	Atencion: cedulaPaciente, especialidad, prioridad, costoBase, tieneExamenes, tiempoEspera, estado — con constructor, getters y setters
•	Ahorcado: manejo del juego, historial, niveles de dificultad, dibujo ASCII


Correcion del codigo
Se depuro el codigo y se justifico
