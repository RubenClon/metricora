# Metricora 📊 • Kotlin Multiplatform (KMP)

[![Kotlin](https://img.shields.io/badge/Kotlin-2.3.0-purple.svg)](https://kotlinlang.org/)
[![Compose Multiplatform](https://img.shields.io/badge/Compose%20Multiplatform-1.10.0-blue.svg)](https://jetbrains.com/lp/compose-multiplatform/)
[![AGP](https://img.shields.io/badge/AGP-8.11.2-green.svg)](https://developer.android.com/studio/releases/gradle-plugin)
[![Koin](https://img.shields.io/badge/Koin-4.2.0-blueviolet.svg)](https://insert-koin.io/)

**Metricora** es una aplicación comercial multiplataforma nativa diseñada para gestionar la contabilidad e impuestos (IVA, IRPF y liquidaciones trimestrales) de autónomos bajo el modelo fiscal español. 

A diferencia de las soluciones híbridas tradicionales, Metricora comparte el **100% de la lógica de negocio, reglas fiscales y persistencia** mediante **Kotlin Multiplatform (KMP)**, compilando a código nativo en **5 plataformas**: Android, iOS, Windows, macOS y Linux.

---

## 📸 Capturas de Pantalla e Interfaz Adaptativa

El sistema implementa una interfaz completamente responsiva controlada mediante un gestor de clases de ventana (`rememberWindowClass()`). La navegación se adapta dinámicamente según la densidad y tamaño de la pantalla del dispositivo.

| 📱 Modo Compacto (Android / iOS) | 💻 Modo Expandido (Windows / macOS / Linux) |
|:---:|:---:|
| <img src="screenshots/mobile_dashboard.png" width="260" alt="Dashboard Móvil"/> | <img src="screenshots/desktop_analytics.png" width="520" alt="Analytics Desktop"/> |
| *Navegación inferior táctil (`K34BottomNav`)* | *Panel de navegación lateral estirado (`K34SideNav`)* |

### 🌗 Experiencia Visual Completa
| Modo Oscuro Integrado | Seguridad y APIs Nativas |
|:---:|:---:|
| <img src="screenshots/dark_mode.png" width="260" alt="Modo Oscuro"/> | <img src="screenshots/biometric_prompt.png" width="260" alt="Biometría"/> |
| *Soporte nativo para temas claro, oscuro y automático* | *Pantalla de bloqueo con autenticación biométrica* |

---

## 🏗️ Arquitectura del Proyecto

El proyecto está diseñado bajo los principios de **Clean Architecture** combinados con el patrón de presentación **MVVM (Model-View-ViewModel)**. El código fuente está rigurosamente modularizado para maximizar la reutilización:
