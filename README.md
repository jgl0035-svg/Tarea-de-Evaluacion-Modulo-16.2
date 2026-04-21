# Tarea-de-Evaluacion-Modulo-16.2
# 📝 Nota técnica sobre la ejecución de los tests

Durante la ejecución de los tests en Google Chrome aparece un aviso del Gestor de Contraseñas indicando que la contraseña utilizada en SauceDemo ha sido encontrada en una brecha de seguridad. Este popup bloquea temporalmente la interacción con la página, impidiendo que Selenium pueda hacer clic en los botones de “Add to cart”.

Este comportamiento no está relacionado con el código ni con Selenium, sino con la seguridad integrada del navegador. Cuando se cierra el aviso manualmente (pulsando “Aceptar”), los tests continúan y pasan correctamente en verde. Por tanto, el funcionamiento de las pruebas es correcto y el bloqueo se debe únicamente al popup del navegador.

A continuación incluyo una captura del aviso para que se entienda mejor el problema:

![popup](Captura de pantalla 2026-04-21 205548.png)

---

# 🧠 Apreciación y reflexión personal

En esta tarea he podido profundizar en el uso de Selenium y en la estructura Page Object Model, que hasta ahora solo había visto de forma más superficial. Me ha servido para entender mejor cómo separar la lógica de las páginas de la lógica de los tests, y cómo esto facilita muchísimo la organización del proyecto y la reutilización del código. También he aprendido a trabajar con localizadores más complejos, especialmente con XPath, y a comprender por qué algunos selectores funcionan en unas situaciones y en otras no.

Otro aspecto importante ha sido la gestión del ciclo de vida de los tests con JUnit: el uso de `@BeforeEach`, `@AfterEach` y la estructura de las pruebas me ha ayudado a tener una visión más clara de cómo se automatizan flujos completos dentro de una aplicación web. Además, he tenido que interpretar errores reales de Selenium, entender por qué fallaban los tests y aprender a diferenciar cuándo el problema viene del código y cuándo viene del propio navegador o del entorno.

En general, esta práctica me ha ayudado a acercarme más a un flujo de trabajo profesional, a entender mejor cómo se automatizan pruebas en aplicaciones reales y a ganar confianza en la depuración de problemas tanto de Selenium como del navegador. Siento que he avanzado bastante en la comprensión de la automatización de pruebas y en la organización de proyectos de testing.
