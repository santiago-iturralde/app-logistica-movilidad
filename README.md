# 🚖 App Móvil de Logística y Transporte Urbano

> **Ecosistema móvil multiplataforma (Android/iOS) para la conexión en tiempo real entre pasajeros y conductores.**

![Project Status](https://img.shields.io/badge/Status-Production%20%28Private%29-blue)
![Tech Stack](https://img.shields.io/badge/Stack-Flutter%20%7C%20Firebase%20%7C%20Google%20Maps-02569B)
![Platform](https://img.shields.io/badge/Platform-Android%20%26%20iOS-green)
![License](https://img.shields.io/badge/License-Proprietary-red)

## 📖 El Desafío
Desarrollar una solución tecnológica integral para modernizar una agencia de remises, reemplazando la asignación manual por radio con un sistema automatizado. El objetivo principal fue optimizar la logística de despacho, reducir los tiempos de espera y aumentar la seguridad tanto de conductores como de pasajeros.

**⚠️ Nota:** *Este software fue desarrollado para un cliente privado. El código fuente no está disponible públicamente por acuerdos de confidencialidad.*

## 🛠️ Solución Técnica

El sistema consta de tres componentes principales:
1.  **Driver App:** Para conductores (recepción de viajes, navegación).
2.  **Passenger App:** Para clientes (solicitud, seguimiento, pagos).
3.  **Admin Dashboard:** Panel web para control de flota y despacho manual.

### Stack Tecnológico
| Componente | Tecnología | Uso |
|:---:|:---:|:---|
| **Mobile Core** | **Flutter (Dart)** | Desarrollo híbrido para mantener una única base de código para Android e iOS. |
| **Backend / DB** | **Firebase** | Firestore (NoSQL) para base de datos en tiempo real y Auth para gestión de sesiones. |
| **Logic** | **Cloud Functions** | Lógica de negocio segura (cálculo de tarifas) ejecutada en el servidor (Serverless). |
| **Maps** | **Google Maps API** | Servicios de Geocoding, Places Autocomplete y Directions API para rutas óptimas. |

## ⚡ Características Clave Implementadas

### 📍 Tracking en Tiempo Real & Geofencing
Implementación de listeners de Firestore para actualizar la posición del conductor en el mapa del pasajero con latencia mínima (<500ms). Uso de Geofencing para detectar llegadas automáticas.

### 💰 Cálculo de Tarifas Dinámico
Algoritmo híbrido que combina **distancia** (obtenida via API) y **tiempo estimado**, con soporte para zonas de recargo y tarifas nocturnas configurables desde el backend.

### 📶 Modo Offline-First
Arquitectura robusta que permite a la app seguir funcionando (consultar historial, ver estado actual) incluso en zonas de baja cobertura, sincronizando los datos automáticamente al recuperar conexión.

## 📱 Galería de Pantallas (UI/UX)

> *Diseño centrado en la usabilidad rápida para conductores en movimiento.*

| Introduccion/Informacion | 
|:---:|:---:|:---:|
| <img width="389" height="874" alt="1_remis" src="https://github.com/user-attachments/assets/1ddb0c6e-198a-4f03-a7ae-138ea3c1a79c" /> |
| <img width="386" height="852" alt="2_remis" src="https://github.com/user-attachments/assets/3a09e589-86f9-4336-ba3d-30af72e8bd4c" /> |

| Login / Inicio | Solicitud de Viaje | 
|:---:|:---:|:---:|
| <img width="392" height="878" alt="3_remis" src="https://github.com/user-attachments/assets/266bccec-8209-4ea8-8d93-de54cff5fbf2" /> 
| ![4_remis](https://github.com/user-attachments/assets/52815bb3-173b-426f-beca-546af68ee64f) |

|Menu|
|:---:|:---:|:---:|
| ![5_remis](https://github.com/user-attachments/assets/f6c018d2-7550-404f-b33e-6234efbe8877)|

---
### 👨‍💻 Santiago Iturralde - Mobile & Backend Developer
[Ver Portafolio Completo](https://portafolio-kappa-kohl.vercel.app/)
