### 1. **Asistente virtual de voz** (p. ej. Siri, Alexa o Google Assistant en un altavoz inteligente).

- **Performance:** Entendimiento del lenguaje natural, tiempo de respuesta despues de la pregunta, satisfaccion del usuario
- **Environment:** Parcialmente observable, determinista, secuencial, dinámico y continuo. El entorno depende de donde se encuentre el dispositivo, no es lo mismo que se encuentre en un recamara que en la cocina ya que tiene diferentes dispositivos y características.
- **Actuators:** Reproducir musica, encender o apagar dispositivos, responder preguntas, enviar mensajes, hacer llamadas.
- **Sensors:** Microfono, bocinas, camaras, sensores de temperatura, de movimiento, de humendad, conexion a internet.

### 2. **Robot aspirador doméstico** (p. ej. Roomba u otro robot que limpia pisos de un departamento).

- **Performance:** Tiempo de limpieza, calidad de limpieza, duracion de la bateria.
- **Environment:** Totalmente observable, estocastico, secuencial, dinámico y continuo. El entorno depende de la casa donde se encuentre el robot, ya que cada casa tiene diferentes habitaciones, muebles y obstáculos.
- **Actuators:** Movilidad hacia adelante, hacia atras, girar 360 grados, succion y trapear.
- **Sensors:** Deteccion de suciedad, de obstaculos, bateria, camara (como el LIDAR).

### 3. **Sistema de recomendación de streaming** (p. ej. Netflix o Spotify que sugiere películas o canciones).

- **Performance:** Tiempo de respuesta, cercania de las recomendaciones a los gustos del usuario, sugerencias de contenido nuevo.
- **Environment:** Parcialmente observable, estocastico, secuencial, dinámico y discreto. El entorno depende de los gustos del usuario, que pueden cambiar con el tiempo y con las tendencias.
- **Actuators:** Enumerar recomendaciones.
- **Sensors:** Historial del usuario, califiaciones de contenido, tiempo de retencion.

### 4. **Vehículo autónomo en ciudad** (conducción sin conductor en calles urbanas con tráfico y peatones).

- **Performance:** Tiempo de llegada para el usuario y destino final, seguridad del usuario y de los peatones, eficiencia en el consumo de combustible, ruta optima.
- **Environment:** Parcialmente observable, estocastico, secuencial, dinámico y continuo. El entorno depende de la ciudad donde se encuentre el vehiculo, ya que cada ciudad tiene diferentes calles, semaforos, peatones y trafico, no es lo miso una calle de latinoamerica que una calle de europa.
- **Actuators:** Acelerar, frenar, girar, encender o apagar luces, encender o apagar limpiaparabrisas.
- **Sensors:** Camaras, LIDAR, GPS, sensores de velocidad, sensores de proximidad, sensores de temperatura, sensores de lluvia, acceso a internet para obtener informacion del trafico y del clima.

### 5. **Agente de trading algorítmico en bolsa** (compra y venta automática de acciones en mercados financieros).

- **Performance:** Rentabilidad del portafolio, disminucion de riesgo, tiempo de respuesta de transaccion, cumplimiento de perfil de riesgo.
- **Environment:** Parcialmente observable, estocastico, secuencial, dinámico y continuo. El entorno depende del mercado financiero, dependiento de que activo se este operando y la plataforma que se utilice.
- **Actuators:** Comprar, vender, alertar al usuario, analisis de riesgo, analisis de rentabilidad, analisis de las compañias.
- **Sensors:** Datos del mercado, noticias, Estado de resultados de la coompañia, analisis tecnico y fundamental.

### 6. **Sistema de diagnóstico médico asistido por IA** (apoya a un médico a interpretar síntomas e imágenes clínicas).

- **Performance:** Entendimiento de los sintomas, tiempo de respuesta, precision del diagnostico, sugerencias de tratamiento, disminucion de errores medicos humanos.
- **Environment:** Parcialmente observable, estocastico, secuencial, dinámico y continuo. El entorno depende del paciente, ya que cada paciente tiene diferentes sintomas, antecedentes medicos y resultados de laboratorio, ademas depende del medico que este utilizando la herramienta, porque diferentes medicos pueden tener diferentes diagnosticos para el mismo caso.
- **Actuators:** Sugerir diagnosticos, sugerir tratamientos, alertar al medico de posibles errores, generar reportes medicos.
- **Sensors:** Resultados de laboratorio, sintomas del paciente, imagenes del paciente, antecedentes medicos del paciente.

### 7. **Dron de inspección de infraestructura** (revisa grietas, corrosión o fugas en puentes, tuberías o líneas eléctricas).

- **Performance:** Tiempo de inspeccion, precision de la inspeccion, seguridad del dron y del personal, deteccion de problemas en la infraestructura.
- **Environment:** Totalmente observable, estocastico, secuencial, dinámico y continuo. El entorno depende de la infraestructura que se este inspeccionando, ya que cada infraestructura tiene diferentes caracteristicas, ademas depende del clima y de la hora del dia.
- **Actuators:** Moverse en el espacio, girar, tomar fotos, grabar videos, enviar datos a la nube, diagnosticar problemas.
- **Sensors:** Camara, LIDAR, GPS, sensores de proximidad, sensores de temperatura, sensores de humedad, internet para enviar datos a la nube.

### 8. **Agente jugador de ajedrez** (programa que compite contra un humano u otro agente en partidas completas).

- **Performance:** Calidad de movimientos, tiempo de respuesta, tasa de victorias, capacidad de adaptacion a diferentes estilos de juego, mejora continua a traves del aprendizaje.
- **Environment:** Totalmente observable, determinista, secuencial, dinámico y discreto. Depende del jugador, ya que cada oponente tiene diferentes estilos de juego y estrategias.
- **Actuators:** Mover piezas, analizar el tablero, calcular jugadas futuras, aprender de partidas anteriores.
- **Sensors:** Tablero de ajedrez, movimientos del oponente, historial de partidas, reglas del juego.


