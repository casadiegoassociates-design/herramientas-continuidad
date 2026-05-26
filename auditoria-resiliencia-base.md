# Checklist: Auditoria de Resiliencia Tecnologica
**Desarrollado por:** Casadiego & Asociates  
**Estándar de Referencia:** ISO 22301 / ITIL v4

---

## 1. Resiliencia Energetica

> **Enfoque:** Mitigacion de cortes de energia prolongados (Blackouts) e inestabilidad de voltaje.

- [ ] **Topologia UPS:** Validar equipos Online de Doble Conversion (0 ms de transferencia en carga critica).
- [ ] **Autonomia Baterias:** Verificar soporte de carga por un minimo de 15 minutos (ventana de arranque secundario).
- [ ] **Conmutacion ATS:** Confirmar transferencia automatica a planta diesel en menos de 10 segundos.
- [ ] **Combustible Planta:** Verificar stock in-situ para un minimo de 48 horas de autonomia continua a plena carga.
- [ ] **Pruebas Black-Start:** Validar ejecuciones de pruebas con corte real de energia en los ultimos 90 dias.

---

## 2. Proteccion de Datos y Backups

> **Enfoque:** Blindaje de informacion contra fallos fisicos, logicos o ataques de Ransomware.

- [ ] **Regla 3-2-1 (Copias):** Verificar la existencia de 3 copias de datos (1 produccion, 2 respaldos).
- [ ] **Regla 3-2-1 (Medios):** Confirmar el uso de al menos 2 tipos de almacenamiento distintos (NAS, Cintas, Discos).
- [ ] **Regla 3-2-1 (Off-site):** Validar minimo 1 copia externa fuera de la planta principal (Aislamiento Cloud).
- [ ] **Inmutabilidad:** Verificar politicas WORM o Air-Gap logico activos en el repositorio secundario de backups.
- [ ] **Ventana RPO:** Confirmar que la frecuencia de respaldo de la base de datos se alinea con el limite de perdida tolerable.
- [ ] **Ventana RTO:** Verificar simulacros de restauracion critica en entornos aislados en los ultimos 30 dias.

---

## 3. Redundancia de Red

> **Enfoque:** Alta disponibilidad de conectividad y eliminacion de puntos unicos de fallo (SPOF).

- [ ] **Enlaces ISP:** Confirmar minimo 2 proveedores de internet con rutas e infraestructura fisica de ultima milla separadas.
- [ ] **Failover SD-WAN:** Verificar conmutacion por error automatica en menos de 5 segundos ante caidas de linea.
- [ ] **Core HA:** Validar configuraciones de alta disponibilidad (Active-Passive) en switches y firewalls principales.

---

## 4. Seguridad y Gobierno (IAM)

> **Enfoque:** Control estricto de accesos y privilegios durante ventanas de contingencia u operacion degradada.

- [ ] **Minimo Privilegio:** Verificar que los accesos a las consolas criticas de infraestructura esten limitados estrictamente por rol.
- [ ] **MFA Activo:** Validar autenticacion multifactor en el 100% de los accesos remotos (VPNs) y consolas de nube.
- [ ] **Centralizacion Logs:** Confirmar almacenamiento inmutable de bitacoras de eventos para auditorias forenses.

---

## 📊 Solicitud de Evaluacion Formal

Si al ejecutar este checklist autogestionado su equipo detecta mas de un **[ ]** sin marcar, su operacion se encuentra en una brecha critica de continuidad operativa.

Para coordinar una auditoria formal respaldada por ingenieros seniors y recibir un informe ejecutivo de impacto financiero ($C_down), genere una orden de servicio con nuestra firma:

* 🌐 **Sitio Web:** [casadiego.associates.com](https://casadiego.associates.com)
* 💬 **WhatsApp Corporativo:** [+58 412-8453912](https://wa.me/584128453912)
