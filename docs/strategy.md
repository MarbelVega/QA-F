# Estrategia de Quality Engineering

## Principios
1. Pruebas tempranas y continuas.
2. Priorización basada en riesgo y criticidad.
3. Trazabilidad entre requisito, riesgo, prueba, defecto y evidencia.
4. Automatización en la capa adecuada, no automatizar por porcentaje.
5. Quality gates explícitos, excepciones con vencimiento y retest.
6. Pruebas en producción controladas: canary, sintéticos y observabilidad.

## Modelo recomendado
- **Componente:** reglas y lógica aislada, rápidas y deterministas.
- **Integración/contrato:** API, BD, eventos, terceros y compatibilidad.
- **Sistema/E2E:** journeys críticos, pocos pero representativos.
- **No funcionales:** seguridad, rendimiento, accesibilidad, resiliencia y recuperación.
- **Aceptación/operación:** smoke, rollback, monitoreo, SLO y DR.

## Definition of Ready
Riesgo identificado, aceptación verificable, datos/ambiente definidos, dependencias disponibles, observabilidad prevista y requisitos de seguridad/privacidad incluidos.

## Definition of Done
Pruebas aprobadas, evidencia adjunta, defectos tratados, automatización integrada, sin hallazgos bloqueantes, rollback probado, monitoreo activo y documentación actualizada.

## Métricas útiles
- Escape rate y defectos por severidad.
- Cobertura de riesgos y journeys, no solo líneas de código.
- Flaky test rate objetivo < 2%.
- Tiempo de feedback de pull request objetivo < 15 min para gates rápidos.
- Change failure rate, deployment frequency, lead time y MTTR.
- p95/p99, error rate y throughput contra SLO.
- Hallazgos críticos/altos abiertos, edad y tasa de retest.
