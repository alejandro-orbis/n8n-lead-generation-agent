# 🤖 Agente Autónomo de Generación de Leads B2B (n8n + Apify + IA)

Sistema de automatización que extrae, enriquece y organiza clientes potenciales desde Google Maps. Ideal para equipos de ventas y marketing que necesitan leads cualificados 24/7.

---

## 📊 Arquitectura del Sistema

[Schedule Trigger] → [Google Sheets (Leer Consultas)] → [Apify (Scraping Google Places)] → [Firecrawl (Web Scraping)] → [JavaScript (Extracción con IA)] → [Google Sheets (Guardar Resultados)]

---

## 🚀 ¿Qué hace este sistema?

| Paso | Descripción |
|:---|:---|
| **1** | Lee consultas desde un Google Sheet (ej: "clínicas dentales Madrid") |
| **2** | Lanza un job en Apify para buscar negocios en Google Places |
| **3** | Espera a que el job termine y obtiene los resultados |
| **4** | Para cada negocio con sitio web, extrae el HTML completo |
| **5** | Usa JavaScript y expresiones regulares para extraer: emails, LinkedIn, Facebook, Instagram, Twitter |
| **6** | Guarda los datos enriquecidos en Google Sheets |
| **7** | Marca la consulta como procesada y pasa a la siguiente |

---

## 🛠️ Tecnologías utilizadas

| Tecnología | Propósito |
|:---|:---|
| **n8n** | Orquestación del flujo completo |
| **Apify** | Scraping de Google Places |
| **Firecrawl** | Extracción de HTML de sitios web |
| **JavaScript (Regex)** | Extracción de emails y redes sociales |
| **Google Sheets API** | Almacenamiento de leads y gestión de consultas |

---

## 📈 Resultados clave

- ✅ **Procesamiento por lotes** para evitar saturar APIs
- ✅ **Extracción de emails** con filtrado de falsos positivos
- ✅ **Detección de redes sociales**: LinkedIn, Facebook, Instagram, Twitter
- ✅ **Escalable** a miles de consultas sin intervención manual
- ✅ **Autónomo**: se ejecuta programado o manualmente

---

## 🎯 Caso de uso real

Una empresa de marketing necesita 500 leads cualificados para una campaña. En lugar de buscar manualmente, este sistema procesa las consultas automáticamente y entrega los datos en una hoja de cálculo lista para usar.

---

## 📦 Instalación y configuración

1. Clona este repositorio
2. Importa el workflow JSON en tu n8n
3. Configura las credenciales:
   - Apify API Key
   - Firecrawl API Key
   - Google Sheets OAuth2
4. Prepara tu Google Sheet con las consultas (columnas: Query, Location)
5. Activa el workflow y ejecuta

---

## 👨‍💻 Autor

**Alejandro Peralta**  
Especialista en Automatización de Procesos  
[GitHub](https://github.com/alejandro-orbis) | [LinkedIn](https://linkedin.com/in/alejandro-orbis) | [Email](mailto:alejandro@orbisautomations.com)

---

## ⭐ Si te ha gustado este proyecto, ¡dale una estrella!
