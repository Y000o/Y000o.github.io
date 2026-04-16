# _Y000!_ — Hacker Portfolio  ![](https://komarev.com/ghpvc/?username=Y000o&color=00ff41&style=flat-square&label=PROFILE+VIEWS)
### Luis Alberto Gastelum Madero · Security Researcher · Bug Hunter · ISO 27001 Auditor

> **🔗 Live → [y000o.github.io](https://y000o.github.io)**

---

## ¿Qué es esto?

Un portfolio de ciberseguridad construido como una **PWA de un solo archivo** — `index.html` — en vanilla HTML, CSS y JavaScript puro. Sin frameworks. Sin dependencias. Sin build steps. Instalable como app nativa en Android, iOS y Desktop.

Diseñado para funcionar como herramienta operativa real: no es solo un portfolio estático, es un entorno de trabajo con terminal, toolkit de reconocimiento, base de datos de payloads, calculadoras y desafíos CTF embebidos.

---

## 🖥 Terminal Emulator

Terminal interactiva en el navegador que simula una sesión Bash en Kali Linux (`y000@kali:/home/y000$`).

**Comandos disponibles:**

| Comando | Descripción |
|---|---|
| `help` | Lista todos los comandos disponibles |
| `whoami` | Muestra perfil completo: rol, HOF, certificaciones |
| `ls` / `cd` / `cat` | Navegación de directorio virtual con archivos ficticios |
| `skills` | Nivel de habilidades (SQLi 95%, XSS 93%, Web Pentest 92%...) |
| `certs` | Lista de certificaciones (Cisco, ISO 27001, CEH, TOEFL...) |
| `repos` | Repositorios principales con estrellas |
| `hof` | Hall of Fame completo (ONU ×3, Harvard) |
| `nmap` | Simula escaneo Nmap con output realista |
| `sqlmap` | Simula explotación SQLi con flags reales |
| `xss` | Generador de payloads XSS en terminal |
| `payload` | Payloads por categoría (xss, sqli, lfi, rce, ssti) |
| `dork` | Google Dorks por tipo de target |
| `dns` | Resolución DNS real vía Google DNS API |
| `ip` | Geolocalización de IP vía ipapi.co |
| `ssl` | Verificación de certificado SSL de un dominio |
| `myip` | Muestra tu IP pública actual |
| `hash` | Calcula hash (md5, sha1, sha256) de un string |
| `encode` / `decode` | Base64 en terminal |
| `man` | Manual de comandos individuales |
| `uptime` | Tiempo transcurrido desde que empecé a hackear |
| `matrix` | Intensifica el rain de Matrix por 10 segundos |
| `y000` | Comando oculto... 👀 |
| `konami` | Easter egg especial |
| `clear` / `exit` | Lo que esperas (o no) |

Historial de comandos navegable con ↑↓. Autocompletado en `Tab`.

---

## 🚩 CTF Challenges — 6 Flags · 1,500 pts

Seis desafíos Capture The Flag embebidos directamente en la página. Barra de progreso y marcador de puntos en tiempo real. Score persistente en `localStorage`.

| # | Nombre | Dificultad | Puntos | Descripción |
|---|---|---|---|---|
| 1 | **XSS ARCHIVE** | 🟢 EASY | 100 | Relacionado con el historial de disclosures XSS |
| 2 | **LOG RECON** | 🟢 EASY | 150 | Reconocimiento en los logs del sitio |
| 3 | **WAF BYPASS** | 🟡 MEDIUM | 200 | Evasión de filtros WAF |
| 4 | **SQL HUNTER** | 🟡 MEDIUM | 250 | Cacería de inyección SQL |
| 5 | **HIDDEN COMMAND** | 🔴 HARD | 300 | Comando oculto en la terminal |
| 6 | **KONAMI CODE** | ⚫ EXPERT | 500 | ↑↑↓↓←→←→BA — tú ya sabes |

> Score actual del sitio: **0/1,500** — nadie lo ha resuelto todo aún.

---

## 🛡 Cyber Toolkit — 28 Herramientas Integradas

Toolkit de seguridad ofensiva completamente funcional en el navegador, organizado en 5 categorías. Búsqueda global de herramientas incluida.

### 🔍 Reconocimiento

**🎯 TARGET PROFILER**  
Orquestador completo de reconocimiento. Ejecuta 5 fases en paralelo con checkboxes configurables:
- Fase 1 — Resolución DNS
- Fase 2 — Infraestructura (Shodan/InternetDB)
- Fase 3 — Superficie de ataque (subdominios, puertos)
- Fase 4 — Threat Intel (OTX, MalwareBazaar)
- Fase 5 — OSINT pasivo
Genera **PDF Técnico**, **PDF Ejecutivo** y exporta en **JSON**.

**🔍 RECON (Unificado)**  
Todo-en-uno para dominio o IP. Módulos independientes: DNS · Ports/CVEs · WHOIS · Subdomains · SSL/Certs · BGP/ASN · Dir Fuzz · Headers · Geoloc · Propagación. Botón ▶ RECON ejecuta todos en paralelo. Export TXT.

**🔭 SHODAN EXPLORER**  
Búsquedas avanzadas con filtros, exploits asociados, DNS inverso y perfil de organización. Soporte de API Key opcional para upgrade de InternetDB a API completa con más datos.

**🌀 DNS RECON**  
Consulta completa de registros DNS: A · AAAA · MX · NS · TXT · SOA · CNAME · SRV · AXFR.

**📜 CRT.SH**  
Búsqueda de subdominios en logs públicos de Certificate Transparency. Modos: subdominios, certificados completos, expirados.

**🌐 ASN LOOKUP**  
Lookup de número ASN, dominio o IP. Devuelve prefijos anunciados, organización, país y BGP peers.

**📍 IP INFO**  
Geolocalización de IP con ASN, ISP, ciudad, país y reverse DNS.

**🗺 GEO MAP**  
Mapa interactivo de geolocalización + simulación de traceroute visual con saltos.

**🕰 WAYBACK MACHINE**  
Consulta CDX API de Internet Archive — historial de capturas, URLs indexadas por fecha y estado HTTP.

**🪣 S3 FINDER**  
Buscador de buckets expuestos en Amazon S3, Azure Blob y GCP Storage con permutaciones automáticas del nombre del target.

**🔍 PORT SCANNER**  
Escaneo de puertos vía Shodan como Nmap — banners, versiones de servicio y CVEs asociados por puerto.

---

### ☣ Threat Intelligence

**☣ THREAT INTEL**  
Análisis multi-motor de amenazas para IPs, URLs, dominios y hashes de archivos.  
Motores: MalwareBazaar · AlienVault OTX · Cloudflare · Spamhaus · Shodan · ipapi.co  
Soporta **bulk scan** (múltiples targets a la vez) y **drag & drop de archivos** para análisis de hash.

**🐛 CVE DATABASE**  
Búsqueda de CVEs por tecnología, nombre o número. Muestra CVSS score, descripción y referencias. Fuentes: CIRCL + NVD.

**💥 EXPLOIT SEARCH**  
Búsqueda de exploits públicos en Exploit-DB, CIRCL, GitHub PoC y PacketStorm.

**💰 BUG BOUNTY CHECKER**  
Verifica si un dominio está dentro del scope de programas en HackerOne, Bugcrowd e Intigriti.

**🔎 GITHUB SECRETS**  
Scanner de secretos expuestos en repositorios públicos de GitHub (tokens, API keys, credentials).

**⚛ NUCLEI TEMPLATES**  
Búsqueda de templates de Nuclei por CVE, tecnología, severidad o tag. Links directos al repositorio.

**🔭 INTEL HUB**  
Hub centralizado que conecta con: Robtex · ThreatFox · URLhaus · GreyNoise · Censys · ZoomEye — todo desde una sola interfaz.

---

### 🌐 Web Testing

**🛡 WAF FINGERPRINT + BYPASS**  
Detecta el WAF activo en el target y su tipo. Incluye técnicas de bypass para los WAFs más comunes.

**💣 PAYLOAD GENERATOR**  
Generador visual de payloads para XSS, SQLi, LFI, SSTI y RCE. Seleccionable por tipo y variante.

**🌐 CORS TESTER**  
Prueba de misconfiguraciones Cross-Origin Resource Sharing en el target.

**📋 HTTP HEADERS ANALYZER**  
Análisis de headers de seguridad HTTP: HSTS · CSP · X-Frame-Options · CORS · Fingerprinting de servidor.

**🎭 PAYLOAD OBFUSCATOR**  
Ofuscador de payloads XSS y SQLi para evasión de WAFs y filtros de entrada.

**📡 HTTP HACKBAR**  
Constructor de requests HTTP con URL parser, payload injector, encoder, soporte multi-proxy y exportación de request completo.

**⬡ GRAPHQL SECURITY**  
Detección de endpoints GraphQL, instrospección y queries de ataque predefinidas.

**🔬 PARAMETER DISCOVERY**  
Descubrimiento de parámetros ocultos — más de 200 parámetros comunes, detecta respuestas diferentes (arjun-lite en el browser).

---

### 🔐 Crypto & Encoding

**🔐 HASH CALCULATOR**  
Cálculo de hashes MD5, SHA1, SHA256, SHA512 y HMAC. Comparación de hashes.

**🔑 JWT INSPECTOR**  
Decodificación, inspección y verificación de firma de tokens JWT. Detección de algoritmo none y weak secrets.

**🔄 ENCODER / DECODER**  
Conversión entre: Base64 · URL encoding · HTML entities · Hex · ROT13 · Unicode. Bidireccional.

---

### 📚 Referencia y Documentación

**✅ OWASP CHECKLIST**  
OWASP Testing Guide v4.2 completo como checklist interactiva. Checkboxes persistentes por sesión.

**📝 PENTESTING REPORT BUILDER**  
Constructor de reportes de pentesting profesional — vuln por vuln, con correlación automática OWASP y **exportación a PDF profesional**.

**⚡ CVSS 3.1 CALCULATOR**  
Calculadora interactiva del CVSS Base Score v3.1 con todos los vectores (AV/AC/PR/UI/S/C/I/A) y generación automática del vector string.

**🔍 GOOGLE DORK GENERATOR**  
Generador de Google Dorks para OSINT, asset discovery y reconocimiento pasivo. Categorizado por tipo de target.

**🗂 PORT REFERENCE DB**  
Base de datos de puertos con servicios, protocolos y vectores de ataque comunes. Buscable y filtrable por categoría.

**📝 WORDLIST GENERATOR**  
Generación de wordlists de fuzzing por tecnología detectada — soporta 15 frameworks/stacks diferentes.

**🔎 REGEX TESTER**  
Tester de expresiones regulares con highlight en tiempo real y librería de patrones comunes para security research.

**📐 CIDR / SUBNET CALCULATOR**  
Calculadora de rangos IPv4, número de hosts, broadcast, máscaras de red y subnets.

**🔀 HTTP RESPONSE DIFFER**  
Compara dos respuestas HTTP side-by-side y resalta las diferencias — útil para detección de auth bypass y blind injection.

**🔒 PASSWORD AUDIT**  
Generador de one-liners para Hashcat y John The Ripper. Identificación de tipo de hash y wordlists recomendadas.

**🎲 UTILS**  
Caja de herramientas miscelánea: generador de UUID/tokens, cálculo de Favicon Hash (Shodan), Password Strength Meter y User-Agent randomizer.

---

## 💣 Payload Arsenal (Base de Datos de Payloads)

Base de datos filtrable de payloads ofensivos con búsqueda por texto y filtros por categoría y etiqueta. One-click copy para cada entrada.

**Categorías disponibles:**

| Tipo | Variantes incluidas |
|---|---|
| **XSS** | Classic, DOM-based, Blind XSS, Polyglot, Framework-specific |
| **SQLi** | Union-Based, Error-Based, Boolean Blind, Time-Based, OOB, Stacked queries |
| **SSTI** | Jinja2, Twig, Freemarker, Velocity |
| **SSRF** | Internal services, cloud metadata, bypass |
| **XXE** | External entity, Blind XXE |
| **WAF Bypass** | Encoding tricks, HTTP pollution, Unicode bypass |
| **Auth Bypass** | SQL-based, JWT manipulation, default creds |
| **Google Dorks** | Admin panels, sensitive files, login pages, config exposure |
| **Cloud** | AWS, Azure, GCP misconfigurations |
| **Custom** | Payloads propios desarrollados en engagements reales |

---

## 🗺 Vulnerability Map

Mapa interactivo construido con **Leaflet.js** que visualiza los targets de responsible disclosure en el mapa mundial. Cada marcador incluye:
- Nombre de la organización
- Tipo de vulnerabilidad reportada
- Referencia al HOF o CVE
- País/región de la organización

---

## 📡 Attack Methodology Graph

SVG interactivo que representa el kill chain completo de una evaluación de seguridad web. Cada nodo es clickable y muestra información adicional + enlace a GitHub repos relacionados:
TARGET → RECON → SCAN → ENUM → EXPLOIT → REPORT
↓
[SQLi] [XSS] [LFI] [API] [WAF BYPASS]

Nodos vinculados a:
- `github.com/Y000o/Dorking` (RECON)
- `github.com/Y000o/Nmap` (SCAN)
- `github.com/Y000o/sql_injection_basic` (SQLi — 58★)
- `github.com/Y000o/Payloads_xss_sql_bypass` (XSS/WAF — 183★)

---

## 🏆 Hall of Fame

Reconocimientos verificados de responsible disclosure:

| Organización | Reconocimiento | Detalle |
|---|---|---|
| **ONU / CEPAL** | Hall of Fame ×3 | unite.un.org/ict-security/hall-fame — SQL Injection Critical, XSS, phpinfo exposure |
| **Harvard University** | Thank You Letter del CISO | Christian Hamer, CISO, HUIT Information Security — XSS — Feb 2021 |
| **OpenBugBounty** | Researcher Activo | Perfil `_Y000_` — universidades y gobiernos |
| **HackerOne** | Bug Hunter | Programas activos — web apps y APIs |

> *"Thank you for taking the time to report this vulnerability to us responsibly. We appreciate your effort in helping keep Harvard and its community safe."*  
> — Christian Hamer, CISO, Harvard University, Feb 23 2021

---

## 📊 Skills Radar & Bars

Canvas animado con radar chart de 8 ejes (Web Pentesting · OSINT · Network Security · Malware Analysis · Social Engineering · Scripting · Forensics · Criptografía) más barras individuales de habilidades:
- SQLi: 95%
- XSS: 93%
- Web Pentesting: 92%
- Google Dorking: 90%
- Nmap/Recon: 88%
- ISO 27001: 85%
- SIEM/SOC: 82%

---

## ⏱ Timeline

Timeline cronológica de carrera: desde los primeros CTFs, primeros reports en OpenBugBounty, HOF ONU, HOF Harvard, certificaciones, cargo en Gobierno de Querétaro y actividad actual en bug bounty.

---

## ✍️ Write-ups & Findings

**Casos reales documentados con expansión ▼:**

1. **CEPAL / ONU — SQL Injection Crítico**  
   - Tipo: Error-based + Union-based SQLi
   - Impacto: acceso a base de datos completa
   - Estado: Reportado responsablemente, HOF confirmado

2. **Vulnerabilidades XSS en aplicaciones gubernamentales**  
   - DOM-based XSS con prueba de concepto
   - Detalles técnicos de explotación y mitigación

3. **Exposición de phpinfo() en servidor ONU**  
   - Información de sistema expuesta públicamente
   - Vector de escalada para reconocimiento adicional

**Feed en vivo de Medium** — carga automática de los últimos artículos publicados vía RSS.

---

## 📁 Repositorios (GitHub Live)

Tabla de repositorios con búsqueda, filtro por lenguaje, ordenamiento y carga en vivo desde `api.github.com/users/Y000o`.

| Repo | Descripción | Stars |
|---|---|---|
| `Payloads_xss_sql_bypass` | Colección de payloads XSS, HTML, CSS y SQL — mayormente creados/modificados por _Y000!_ | ⭐ 183 |
| `Nmap` | Scripts y comandos Nmap para recon, OS fingerprinting y NSE personalizado | ⭐ 118 |
| `sql_injection_basic` | Guía práctica de SQL Injection — conceptos, payloads, extracción y evasión | ⭐ 58 |
| `Sql_injection_medium-advanced` | Técnicas avanzadas: Union, Error, Blind Boolean, Time-Based | ⭐ 18 |
| `Inyeccion-sql-automatizada-con-sqlmap` | Automatización con SQLMap — extracción de tablas y credenciales | ⭐ 23 |
| `Dorking` | Google Dorks para Bug Bounty y OSINT — paneles expuestos, archivos sensibles | ⭐ 10 |
| `MX-OSINT` | OSINT para México — consultas a bases de datos gubernamentales vía CURP | ⭐ 4 |
| `Y000SINT` | Dashboard OSINT terminal — Shodan + vecert.io (en desarrollo activo) | ⭐ 2 |
| `y000o.github.io` | Este mismo sitio — portfolio hacker con terminal y toolkit | — |

---

## 🎓 Certificaciones

Cards con categorización visual por emisor:

- **Cisco** — Intro to Cybersecurity, Cybersecurity Essentials, Linux Essentials
- **ISO 27001:2022** — Auditor Lead certificado
- **Diplomado** — Seguridad Informática Ágil
- **CEH** — Certified Ethical Hacker
- **CCNA** — Cisco Networking
- **Idiomas** — TOEFL 460 pts · Inglés B1+

---

## 🎨 Diseño & Efectos Visuales

- **Matrix rain** en canvas con modo intenso activable desde terminal (`matrix`)
- **Partículas flotantes** en canvas con física de movimiento
- **CRT scan-line overlay** animado sobre toda la página
- **Glitch animation** en nombre del hero con RGB shift
- **Custom crosshair cursor** con punto central y líneas cruzadas
- **ALERT MODE** — botón en navbar que vira toda la UI de verde a rojo (simulación de amenaza activa)
- **Boot sequence** — animación de arranque de sistema en la primera carga
- Totalmente responsive, mobile-first (probado en Android con Termux)
- Fuentes: **Orbitron** (headers) · **Share Tech Mono** (texto) · **VT323** (accents)

---

## 🥚 Easter Eggs

- **Konami Code** `↑↑↓↓←→←→BA` — activa un overlay oculto y desbloquea el CTF #6
- **Comentario en source code** — mensaje directo para quien hace recon del HTML
- **Comando `y000`** en terminal — desbloquea el CTF #5
- **Comando `sudo su`** — 3 intentos fallidos con mensaje personalizado
- **Comando `exit`** — "No puedes salir. Estás adentro. 😈"
- Prueba: `curl -s https://y000o.github.io | grep -E 'password|secret|key|token'` 😉

---

## 🌐 PWA (Progressive Web App)

- Instalable en Android, iOS y Desktop como app nativa
- `manifest.json` con nombre, íconos y colores del tema
- Theme color: `#00ff41` (verde terminal)
- Funciona offline (assets cacheados)

---

## 📬 Contacto

| Plataforma | Link |
|---|---|
| 🔗 Portfolio | [y000o.github.io](https://y000o.github.io) |
| 💻 GitHub | [github.com/Y000o](https://github.com/Y000o) |
| 🐦 X (Twitter) | [@_Y000_](https://x.com/_Y000_) |
| 💼 LinkedIn | [Luis Gastelum](https://linkedin.com/in/luis-madero-b4933516a) |
| 🐛 OpenBugBounty | [/researchers/_Y000_/](https://openbugbounty.org/researchers/_Y000_/) |
| 🎯 HackerOne | Perfil activo |
| ✉️ Email | luis_gastelum_11@hotmail.com |

---


