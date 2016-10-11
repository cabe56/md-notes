
Goal: produce working software from problem definitions crafted by Product Managers

[Example mapping helps breakdown stories into specifications](https://cucumber.io/blog/2015/12/08/example-mapping-introduction)

## [Job Story](https://blog.intercom.com/using-job-stories-design-features-ui-ux/)
- Situation
- Motivation
- Expected Outcome

## Rules
- Jargon-y names: Acceptance Criteria, Conditions of Satisfaction
- State intent, not a solution
- Independent of implementation
  - Would be the same whether this story would be on web, mobile or a voice activated system.
- Ejemplos:
  - El facturador debe saber que pedidos le faltan por facturar
  - Los infaltables tienen mayor prioridad que productos normales
  - Solo puede haber una linea de pedido por producto

## Examples
- Jargon-y names: Scenarios, Edge cases
- Instance especifico de comportamiento del sistema
- Ejemplos:
  - 2 pedidos hoy, facturador ve 2 pedidos
  - 0 pedidos hoy, facturador no ve pedidos para hoy
  - 4 infaltables, 5 productos normales, facturador puede distinguir 4 de los 9
    - Permite que la implementacion determine si van primero o tienen un tag
  - Vendedor tenia 3 productos, cambio cantidad en uno, cart debe tener 3 lineas
  - Vendedor tenia 1 producto (caja) y un cart item, agrego mismo producto (unidad), solo hay un cart item

## Acceptance Tests
- Ejemplos traducidos a Scenarios de [Gherkin](https://github.com/cucumber/cucumber/wiki/Gherkin) (para test en Cucumber)
  - Given: preconditions
  - When: action
  - Then: testable outcome
- El PM ejecutaria estas acciones manualmente para verificar que se soluciono el problema.

## Referencias
- [Acceptance Criteria vs Scenarios](https://lizkeogh.com/2011/06/20/acceptance-criteria-vs-scenarios/)
- [Ejercicio que une todos los conceptos: Example mapping](https://cucumber.io/blog/2015/12/08/example-mapping-introduction)
