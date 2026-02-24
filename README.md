# 🚗 JulioDRIVE - Plataforma de Transporte Compartido

**JulioDRIVE** es una plataforma moderna de transporte compartido inspirada en IN Drive, diseñada para conectar pasajeros y conductores de manera segura, rápida y eficiente.

---

## 📋 Tabla de Contenidos

- [Características](#características)
- [Opciones Tecnológicas](#opciones-tecnológicas)
- [Estructura del Proyecto](#estructura-del-proyecto)
- [Requisitos Previos](#requisitos-previos)
- [Instalación](#instalación)
- [Configuración](#configuración)
- [Documentación](#documentación)
- [Seguridad](#seguridad)
- [Roadmap](#roadmap)
- [Contribución](#contribución)
- [Licencia](#licencia)

---

## ✨ Características

### Para Pasajeros
- ✅ Registro e identificación segura
- ✅ Solicitud de viajes en tiempo real
- ✅ Mapa interactivo con ubicación en vivo
- ✅ Sistema de calificación y reseñas
- ✅ Múltiples métodos de pago
- ✅ Historial de viajes
- ✅ Contacto de emergencia
- ✅ Chat con conductores

### Para Conductores
- ✅ Registro y verificación de documentos
- ✅ Aceptar/rechazar viajes
- ✅ Historial de ingresos
- ✅ Sistema de calificación
- ✅ Rutas optimizadas
- ✅ Soporte técnico prioritario
- ✅ Bonos y promociones

### Para Administradores
- ✅ Panel de control (Dashboard)
- ✅ Gestión de usuarios
- ✅ Monitoreo de viajes
- ✅ Análisis y reportes
- ✅ Gestión de pagos

---

## 🛠️ Opciones Tecnológicas

JulioDRIVE ofrece **3 opciones de implementación** según tus necesidades:

### **Opción 1: Web (React + Node.js + MongoDB)**
**Mejor para:** Sitio web de administración, MVP rápido

```
Stack:
├── Frontend: React.js, Redux, Mapbox/Google Maps
├── Backend: Node.js + Express.js
├── Base de Datos: MongoDB
├── Autenticación: JWT + OAuth2
├── Pagos: Stripe / MercadoPago
└── Hosting: Vercel (frontend), Heroku/Railway (backend)
```

**Ventajas:**
- Desarrollo rápido
- Comunidad grande
- Fácil mantenimiento
- Buena documentación

---

### **Opción 2: App Móvil Multiplataforma (React Native + Node.js + Firebase)**
**Mejor para:** Aplicación móvil iOS y Android, inicio rápido

```
Stack:
├── Frontend: React Native + Expo
├── Backend: Node.js + Express.js
├── Base de Datos: Firebase Firestore
├── Autenticación: Firebase Auth
├── Mapas: React Native Maps
├── Pagos: Stripe + Apple Pay
└── Notificaciones: Firebase Cloud Messaging
```

**Ventajas:**
- Una sola base de código para iOS y Android
- Desarrollo rápido
- Despliegue fácil con Expo
- Backend serverless con Firebase

---

### **Opción 3: App Móvil Nativa Profesional (Flutter + Python/Django + PostgreSQL)**
**Mejor para:** Aplicación profesional, alto rendimiento

```
Stack:
├── Frontend: Flutter (iOS y Android nativos)
├── Backend: Python + Django/FastAPI
├── Base de Datos: PostgreSQL
├── Cache: Redis
├── Autenticación: JWT + Social Login
├── Pagos: Stripe / Adyen
├── WebSockets: Django Channels
├── Hosting: AWS / Google Cloud
└── CI/CD: GitHub Actions / GitLab CI
```

**Ventajas:**
- Máximo rendimiento
- Experiencia nativa
- Escalabilidad profesional
- Mejor soporte comercial

---

## 📁 Estructura del Proyecto

```
JulioDRIVE/
│
├── README.md
├── .gitignore
├── LICENSE
│
├── 📂 option-1-web/
│   ├── frontend/
│   │   ├── src/
│   │   │   ├── components/
│   │   │   ├── pages/
│   │   │   ├── services/
│   │   │   └── App.jsx
│   │   └── package.json
│   │
│   └── backend/
│       ├── src/
│       │   ├── routes/
│       │   ├── controllers/
│       │   ├── models/
│       │   └── middleware/
│       └── package.json
│
├── 📂 option-2-mobile-react-native/
│   ├── app/
│   │   ├── screens/
│   │   ├── components/
│   │   ├── services/
│   │   └── app.json
│   │
│   └── backend/
│       ├── src/
│       │   ├── routes/
│       │   ├── controllers/
│       │   └── models/
│       └── package.json
│
├── 📂 option-3-mobile-flutter/
│   ├── flutter_app/
│   │   ├── lib/
│   │   │   ├── screens/
│   │   │   ├── models/
│   │   │   ├── services/
│   │   │   └── main.dart
│   │   └── pubspec.yaml
│   │
│   └── backend-python/
│       ├── app/
│       │   ├── routes/
│       │   ├── models/
│       │   └── settings.py
│       └── requirements.txt
│
├── 📂 shared/
│   ├── api-documentation/
│   │   └── API.md
│   ├── database-schema/
│   │   └── schema.sql
│   └── security/
│       └── SECURITY.md
│
└── 📂 docs/
    ├── SETUP.md
    ├── DEPLOYMENT.md
    └── CONTRIBUTING.md
```

---

## 📦 Requisitos Previos

### General
- Git
- Node.js 16+ (Opciones 1 y 2)
- Python 3.9+ (Opción 3)
- Docker (recomendado)

### Opción 1 (Web)
- npm o yarn
- Cuenta en MongoDB Atlas
- Cuenta en Stripe o MercadoPago

### Opción 2 (React Native)
- Expo CLI
- Xcode (Mac) o Android Studio
- Cuenta en Firebase

### Opción 3 (Flutter)
- Flutter SDK 3.0+
- Dart 3.0+
- PostgreSQL 12+
- Redis (opcional)

---

## 🚀 Instalación

### Opción 1: Web (React + Node.js)

```bash
# Clonar repositorio
git clone https://github.com/Catgato-star/JulioDRIVE.git
cd JulioDRIVE/option-1-web

# Backend
cd backend
npm install
cp .env.example .env
npm run dev

# Frontend (en otra terminal)
cd ../frontend
npm install
npm start
```

### Opción 2: React Native

```bash
# Clonar repositorio
git clone https://github.com/Catgato-star/JulioDRIVE.git
cd JulioDRIVE/option-2-mobile-react-native

# Backend
cd backend
npm install
npm run dev

# Mobile App
cd ../app
npm install
expo start
```

### Opción 3: Flutter

```bash
# Clonar repositorio
git clone https://github.com/Catgato-star/JulioDRIVE.git
cd JulioDRIVE/option-3-mobile-flutter

# Backend Python
cd backend-python
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
pip install -r requirements.txt
python manage.py runserver

# Flutter App
cd ../flutter_app
flutter pub get
flutter run
```

---

## ⚙️ Configuración

### Variables de Entorno

Cada opción requiere un archivo `.env`:

**Opción 1 & 2:**
```
MONGODB_URI=mongodb+srv://user:password@cluster.mongodb.net/juliodrive
STRIPE_SECRET_KEY=sk_test_xxxxx
JWT_SECRET=your_secret_key
GOOGLE_MAPS_API_KEY=xxxxx
FIREBASE_CONFIG=xxxxx
```

**Opción 3:**
```
DEBUG=False
SECRET_KEY=your_secret_key
DATABASE_URL=postgresql://user:password@localhost/juliodrive
REDIS_URL=redis://localhost:6379
STRIPE_SECRET_KEY=sk_test_xxxxx
```

---

## 📚 Documentación

- [API Documentation](./shared/api-documentation/API.md)
- [Setup Guide](./docs/SETUP.md)
- [Deployment Guide](./docs/DEPLOYMENT.md)
- [Security Policies](./shared/security/SECURITY.md)
- [Database Schema](./shared/database-schema/schema.sql)

---

## 🔒 Seguridad

JulioDRIVE implementa los siguientes estándares de seguridad:

- ✅ Autenticación con JWT y OAuth2
- ✅ Encriptación de datos sensibles (contraseñas, documentos)
- ✅ Validación de documentos de conductores
- ✅ HTTPS/TLS para todas las conexiones
- ✅ Protección contra CSRF, XSS, SQL Injection
- ✅ Rate limiting en APIs
- ✅ Logs de auditoría
- ✅ Cumplimiento con GDPR/CCPA

Ver [SECURITY.md](./shared/security/SECURITY.md) para más detalles.

---

## 🗓️ Roadmap

### Fase 1 (MVP - Meses 1-2)
- [ ] Autenticación de usuarios
- [ ] Sistema de solicitud de viajes
- [ ] Geolocalización en tiempo real
- [ ] Sistema de pagos básico
- [ ] Chat simple

### Fase 2 (Meses 3-4)
- [ ] Múltiples métodos de pago
- [ ] Sistema de calificación avanzado
- [ ] Soporte técnico
- [ ] Promociones y bonos
- [ ] Dashboard de administrador

### Fase 3 (Meses 5-6)
- [ ] Características de seguridad avanzadas
- [ ] Analytics y reportes
- [ ] Integración con terceros
- [ ] Optimización de rendimiento
- [ ] Internacionalización

### Fase 4 (Largo plazo)
- [ ] IA para recomendaciones
- [ ] Carpooling inteligente
- [ ] Integración de transporte público
- [ ] Expansión a nuevas ciudades

---

## 🤝 Contribución

¡Estamos abiertos a contribuciones! Por favor:

1. Fork el repositorio
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

Ver [CONTRIBUTING.md](./docs/CONTRIBUTING.md) para más detalles.

---

## 📄 Licencia

Este proyecto está bajo la licencia MIT. Ver [LICENSE](./LICENSE) para más detalles.

---

## 📞 Contacto y Soporte

- **Email:** support@juliodrive.com
- **Website:** https://www.juliodrive.com
- **Issues:** [GitHub Issues](https://github.com/Catgato-star/JulioDRIVE/issues)
- **Discussions:** [GitHub Discussions](https://github.com/Catgato-star/JulioDRIVE/discussions)

---

## 👥 Equipo

- **Proyecto:** JulioDRIVE
- **Desarrollador Principal:** [@Catgato-star](https://github.com/Catgato-star)
- **Versión:** 1.0.0
- **Última Actualización:** 2026-02-24

---

**¡Gracias por usar JulioDRIVE!** 🚗✨