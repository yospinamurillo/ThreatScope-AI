# ThreatScope AI

ThreatScope AI es una herramienta de auditoría de seguridad en navegador para analizar código fuente, configuraciones, logs, APIs y contextos de IAM con ayuda de modelos de IA. El objetivo es detectar vulnerabilidades, clasificarlas por severidad y sugerir remediaciones accionables sin requerir un backend complejo.

## ¿Qué hace?

- Analiza texto libre, código, configuraciones y logs
- Detecta potenciales vulnerabilidades comunes: inyección, XSS, secretos expuestos, permisos excesivos, configuración insegura y más
- Prioriza hallazgos por severidad: critical, high, medium, low e info
- Sugiere recomendaciones concretas para mitigar cada riesgo
- Está pensado como un prototipo funcional para uso local o demo

## Características principales

- Interfaz web estática en HTML/JavaScript
- Soporta varios tipos de análisis:
  - Código fuente
  - Configuración
  - Red / infraestructura
  - Logs del sistema
  - API / endpoints
  - IAM / permisos
- Integración con la API de Anthropic para análisis con IA
- Generación de hallazgos estructurados en formato JSON

## Requisitos

- Un navegador moderno (Chrome, Edge, Firefox o Safari)
- Una API key válida de Anthropic
- Acceso a Internet para consultar la API de Anthropic

## Inicio rápido

1. Clona el repositorio:

```bash
git clone https://github.com/yospinamurillo/ThreatScope-AI.git
cd ThreatScope-AI
```

2. Abre el archivo `threat_vulnerability_scanner.html` en tu navegador.

3. Ingresa tu `Anthropic API key` en el campo correspondiente.

4. Pega el código, log, configuración o descripción del sistema a analizar.

5. Selecciona el tipo de análisis y haz clic en `Iniciar análisis`.

## Uso

### Modo de uso recomendado

- Para código fuente: pega snippets o repositorios parciales
- Para configuraciones: añade YAML, JSON, .env, archivos de despliegue o políticas
- Para logs: incluye eventos, errores, entradas de auditoría o mensajes de servidor
- Para APIs: pega rutas, payloads, headers o ejemplos de llamadas
- Para IAM: describe permisos, políticas, roles o entidades de acceso

### Flujo típico

```text
1. Escribe el contexto o código a analizar
2. Elige el tipo de análisis
3. Genera un escaneo con IA
4. Revisa severidades y recomendaciones
5. Corrige los hallazgos antes de desplegar o compartir el artefacto
```

### Nota importante sobre la API key

Este proyecto usa la API de Anthropic directamente desde el navegador. Debes ingresar tu clave en el formulario para que la solicitud pueda autenticar correctamente. No se recomienda compartir tu clave en repositorios públicos ni almacenarla en archivos de configuración versionados.

## Estructura del proyecto

```text
ThreatScope-AI/
├── README.md
├── LICENSE
├── threat_vulnerability_scanner.html
├── CONTRIBUTING.md
├── SECURITY.md
└── ...
```

## Desarrollo y contribución

Consulta `CONTRIBUTING.md` para conocer el flujo de trabajo, estándares de calidad y recomendaciones para enviar cambios.

## Seguridad

Si encontraste una vulnerabilidad o un problema de seguridad, por favor revisa `SECURITY.md` antes de reportarlo.

## Licencia

Este proyecto se distribuye bajo la licencia MIT. Consulta el archivo `LICENSE` para ver el texto completo.

## Estado del proyecto

Este repositorio funciona como prototipo de evaluación de seguridad apoyado por IA. Puede adaptarse para escenarios internos, laboratorios, demos o análisis de seguridad manuales.

## Contacto

Si deseas colaborar o presentar una mejora, abre un issue en GitHub o contacta al propietario del repositorio.

---

ThreatScope AI is a browser-based security auditing tool designed to analyze source code, configurations, logs, APIs, and IAM contexts with AI assistance. The goal is to identify vulnerabilities, classify them by severity, and recommend actionable mitigations without requiring a full backend.
