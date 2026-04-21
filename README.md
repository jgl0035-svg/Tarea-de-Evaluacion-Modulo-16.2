# Tarea-de-Evaluacion-Modulo-16.2
# Aviso sobre los tests

Durante la ejecución de los tests en Google Chrome puede aparecer un aviso del Gestor de Contraseñas indicando que la contraseña utilizada en SauceDemo ha sido encontrada en una brecha de seguridad. Este popup bloquea temporalmente la interacción con la página, impidiendo que Selenium pueda hacer clic en los botones de “Add to cart”.

Esto no está relacionado con el código ni con Selenium, sino con la seguridad integrada del navegador. En caso de que le salga cierra el aviso rápidamente manualmente (pulsando “Aceptar”), los tests continúan y pasan correctamente en verde. Por tanto, el funcionamiento de las pruebas es correcto y el bloqueo se debe únicamente al popup del navegador.

Aquí pongo una captura del aviso para que se entienda mejor el problema:

<img width="605" height="382" alt="Captura de pantalla 2026-04-21 205548" src="https://github.com/user-attachments/assets/f961bafa-2814-4896-bdd2-dfac00d53636" />

---

# Reflexión personal

En esta tarea he podido saber más sobre el uso de Selenium y en la estructura Page Object Model. Me ha servido para entender mejor cómo separar la lógica de las páginas de la lógica de los tests, y cómo esto facilita muchísimo la organización del proyecto y la reutilización del código. También he aprendido a trabajar con localizadores más complejos, especialmente con XPath, y a comprender por qué algunos selectores funcionan en unas situaciones y en otras no.

Otro aspecto importante ha sido la gestión del ciclo de vida de los tests con JUnit: el uso de `@BeforeEach`, `@AfterEach` y la estructura de las pruebas me ha ayudado a tener una visión más clara de cómo se automatizan flujos completos dentro de una aplicación web. También, he entendido errores reales de Selenium, entender por qué fallaban los tests y aprender a diferenciar cuándo el problema viene del código y cuándo viene del propio navegador o de otra cosa.

En general, esta tarea me ha ayudado a acercarme más a un flujo de trabajo profesional, a entender mejor cómo se automatizan pruebas en aplicaciones reales y a ganar confianza en la depuración de problemas tanto de Selenium como del navegador.
