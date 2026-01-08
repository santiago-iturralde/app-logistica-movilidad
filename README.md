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

| Login / Inicio | Solicitud de Viaje | Seguimiento en Vivo |
|:---:|:---:|:---:|
| <img src="images/1_remis.png" width="200" alt="Login Screen"> | <img src="images/2_remis.png" width="200" alt="Booking Screen"> | <img src="images/3_remis.png" width="200" alt="Live Tracking"> |

| Perfil de Usuario | Historial de Viajes | Chat In-App |
|:---:|:---:|:---:|
| <img src="images/4_remis.png" width="200" alt="User Profile"> | <img src="images/5_remis.png" width="200" alt="Trip History"> | <img src="images/chat_screen.png" width="200" alt="Chat Support"> |

---
### 👨‍💻 Santiago Iturralde - Mobile & Backend Developer
[Ver Portafolio Completo](https://portafolio-kappa-kohl.vercel.app/)
