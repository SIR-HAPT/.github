# SIR-HAPT

**Sistema Inmersivo con Retroalimentación Háptica para Terapia**

SIR-HAPT es una herramienta terapéutica para rehabilitación física de miembro superior que integra realidad mixta (Meta Quest 3), retroalimentación háptica (bHaptics TactGlove DK2 y Tactosy for Hands) y un serious game desarrollado en Unity/C# con mecánicas de trayectoria en spline. El sistema incluye además una aplicación de escritorio para la gestión terapéutica desarrollada en Python con KivyMD, respaldada por Firebase Firestore y Authentication.

El sistema fue implementado y evaluado en **ADACEA (Alicante, España)** en colaboración con el grupo **Human Robotics (HuRo Lab)** de la Universidad de Alicante.

Proyecto de Evaluación Final — Licenciatura en Ingeniería Biomédica  
**Universidad de Monterrey (UDEM)** · Vicerrectoría de Ciencias de la Salud

---

## Repositorios

| Componente | Tecnología | Repositorio |
|---|---|---|
| Serious game de realidad mixta | Unity / C# / Meta Quest 3 / bHaptics SDK2 / Firebase | [SIR-HAPT_PEF](https://github.com/SIR-HAPT/SIR-HAPT_PEF) |
| Aplicación de gestión terapéutica | Python / KivyMD / Firebase Firestore & Authentication | [SIR-HAPT_App_PEFII](https://github.com/SIR-HAPT/SIR-HAPT_App_PEFII) |

---

## Arquitectura general

El sistema se compone de dos módulos independientes que se comunican a través de Firebase:

- **Serious game (Meta Quest 3):** el paciente interactúa con trayectorias tridimensionales en un entorno de realidad aumentada, recibiendo retroalimentación visual, auditiva y háptica en tiempo real mediante los guantes bHaptics.
- **Aplicación terapéutica (escritorio):** el terapeuta registra pacientes, configura sesiones y trayectorias, y visualiza las métricas de desempeño obtenidas durante cada sesión.
- **Firebase:** actúa como backend compartido, gestionando autenticación, almacenamiento de trayectorias y registro de sesiones terapéuticas.

---

## Créditos

**Autora:** Alma Cristina Villanueva Guzmán  
**Asesora:** Dra. Irma Nayeli Angulo Sherman (UDEM)  
**Colaboradores:** Dr. Gabriel J. García · Dr. Andrés Úbeda Castellanos — Human Robotics Lab, Universidad de Alicante
