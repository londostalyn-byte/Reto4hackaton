# 🚨 Emergencia-Sync
Sistema de Alerta Temprana de Ingresos a Emergencias - Reto 4 HackIAthon Viamatica

## 📋 Descripción
Plataforma que procesa emergencias médicas en tiempo real, validando pólizas de seguros y notificando automáticamente a hospitales y gestores de casos mediante un agente IA.

## 🏗️ Estructura
```
reto4hackaton/
├── emergencia-frontend/     # Frontend Next.js
├── emergencia-backend/      # Backend FastAPI
└── README.md
```

## 🚀 Quick Start

### Backend
```bash
cd emergencia-backend
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python app/main.py
```

### Frontend
```bash
cd emergencia-frontend
npm install
npm run dev
```

## 📊 Stack
- **Backend:** FastAPI
- **Frontend:** Next.js
- **Database:** PostgreSQL (Railway)


## 🔐 Características
✅ Validación de pólizas en tiempo real
✅ Agente IA para decisiones
✅ Notificaciones automáticas
✅ Auditoría completa

## 🖼️ Capturas

### Formulario de Ingreso de Paciente

<img width="867" height="666" alt="fronted agente ia" src="https://github.com/user-attachments/assets/cf198a96-bc65-4ba8-9126-1b7cdd7b22f8" />

### Envio de Correo 

<img width="1349" height="267" alt="mails " src="https://github.com/user-attachments/assets/0daf2738-f0ad-43be-970e-983ece597bb6" />

### Notificación de Correo Enviada

<!-- ARRASTRA AQUÍ LA IMAGEN DEL CORREO RECIBIDO -->
<img width="1043" height="509" alt="notificacion back" src="https://github.com/user-attachments/assets/c3f3663b-be68-4e97-938d-cff49f951694" />
<img width="877" height="503" alt="emergencia bac" src="https://github.com/user-attachments/assets/b13e0b5c-5218-4445-9351-b59f24ffd89e" />

## 🚀 Deploy
Ambos servicios en Railway (automático desde GitHub)

---

## 📋 Datos de Prueba — Cómo llenar el formulario

### Campos del formulario

| Campo | Descripción |
|---|---|
| **Cédula del Paciente** | 10 dígitos del paciente registrado |
| **ID del Hospital** | Identificador del hospital (ej: HOSP-001) |
| **Nombre del Hospital** | Nombre completo del hospital |
| **Correo del Hospital** | Email del departamento de admisiones |
| **Correo Gestor de Seguros** | Email del gestor de casos de la aseguradora |
| **Fecha y Hora de Ingreso** | Se llena automáticamente con la fecha actual |

---

### 🏥 Hospitales disponibles

| ID Hospital | Nombre | Correo Hospital |
|---|---|---|
| `HOSP-001` | Hospital General San Juan | `admisiones@sanjuan.com` |

---

### 👤 Pacientes de prueba

#### ✅ Caso APROBADO — Póliza activa
```
Cédula:                  1234567890
ID del Hospital:         HOSP-001
Nombre del Hospital:     Hospital General San Juan
Correo del Hospital:     admisiones@sanjuan.com
Correo Gestor Seguros:   casos@segurosecuador.com
```

#### ✅ Caso APROBADO — Póliza activa
```
Cédula:                  1234567891
ID del Hospital:         HOSP-001
Nombre del Hospital:     Hospital General San Juan
Correo del Hospital:     admisiones@sanjuan.com
Correo Gestor Seguros:   casos@segurosamerica.com
```

#### ❌ Caso DENEGADO — Póliza suspendida
```
Cédula:                  1234567892
ID del Hospital:         HOSP-001
Nombre del Hospital:     Hospital General San Juan
Correo del Hospital:     admisiones@sanjuan.com
Correo Gestor Seguros:   casos@segurosecuador.com
```

#### ✅ Caso APROBADO — Póliza activa (plan básico)
```
Cédula:                  1234567893
ID del Hospital:         HOSP-001
Nombre del Hospital:     Hospital General San Juan
Correo del Hospital:     admisiones@sanjuan.com
Correo Gestor Seguros:   casos@segurosVida.com
```

#### ❌ Caso DENEGADO — Póliza expirada
```
Cédula:                  1234567894
ID del Hospital:         HOSP-001
Nombre del Hospital:     Hospital General San Juan
Correo del Hospital:     admisiones@sanjuan.com
Correo Gestor Seguros:   casos@segurosamerica.com
```

---

## 🎯 Reto
Reto 4 HackIAthon Viamatica
