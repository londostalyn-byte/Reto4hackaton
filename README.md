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
- **Database:** SQLite (desarrollo)

## 🔐 Características

✅ Validación de pólizas en tiempo real  
✅ Agente IA para decisiones  
✅ Notificaciones automáticas  
✅ Auditoría completa  


## 🚀 Deploy

Ambos servicios en Railway (automático desde GitHub)

## 📋 Datos de Prueba

- `1234567890` → ACTIVA ✅
- `1234567891` → ACTIVA ✅
- `1234567892` → SUSPENDIDA ❌
- `1234567894` → EXPIRADA ❌

## 🎯 Reto

Reto 4 HackIAthon Viamatica
