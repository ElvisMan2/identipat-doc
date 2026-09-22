# Servicio de desarrollo de una herramienta de inteligencia artificial

## Identificación de activos de propiedad intelectual en el Perú

La herramienta estará basada en procesamiento de lenguaje natural.

## Objetivo del servicio

El objetivo de la consultoría es contratar los servicios especializados de una empresa para el desarrollo de una herramienta de inteligencia artificial basada en procesamiento de lenguaje natural para la identificación de activos de propiedad intelectual en el Perú, que incorpora funcionalidades técnicas, operativas y visuales.

## Requisitos funcionales

Los requisitos funcionales del servicio establecidos en los Términos de Referencia son los siguientes:

### RF-01: Acceso a la plataforma

El sistema deberá permitir el acceso de los usuarios a la plataforma desde el portal institucional [www.patenta.pe](https://www.patenta.pe/), alojado en un servidor independiente. Asimismo, deberá mostrar de forma destacada información general sobre la herramienta, sus propósitos, el funcionamiento básico de sus algoritmos y el tipo de datos que se procesan, brindando pautas claras para su uso ético y consciente. Adicionalmente, el portal incluirá de manera visible los términos, condiciones y políticas de privacidad aplicables a su utilización.

### RF-02: Registro de información del usuario

El sistema deberá permitir registrar a los usuarios nuevos, almacenando información general como nombres, apellidos, correo electrónico y perfil del usuario. Asimismo, deberá reconocer a los usuarios previamente registrados mediante un identificador válido (DNI o Carné de Extranjería) para evitar la duplicidad de registros. El sistema integrará un mecanismo digital (casilla de verificación o equivalente) para capturar el consentimiento explícito, previo, libre e informado del usuario para el tratamiento de sus datos personales, conforme a la Ley N° 29733, impidiendo el avance en la plataforma si este no es otorgado.

### RF-03: Ingreso de descripción del activo

El sistema deberá permitir al usuario ingresar la descripción de su creación mediante lenguaje natural, a través de texto, voz o documentos en formato PDF. Asimismo, deberá exigir una longitud mínima de caracteres en la descripción, con el fin de garantizar un contexto suficiente para su procesamiento y análisis.

### RF-04: Procesamiento de lenguaje natural

El sistema deberá aplicar técnicas de procesamiento de lenguaje natural (PLN) y aprendizaje automático para preprocesar, transformar y analizar la descripción ingresada por el usuario, con el fin de obtener la información necesaria para su clasificación.

### RF-05: Identificación de materia patentable

El sistema deberá utilizar un servicio de IA generativa para analizar la descripción ingresada por el usuario y determinar si la creación descrita contiene materia susceptible de protección mediante patente, de acuerdo con los criterios establecidos en los artículos 15 y 20 de la Decisión 486 de la Comunidad Andina.

El servicio de IA generativa deberá ser compatible con el utilizado actualmente por el Indecopi en sus soluciones de inteligencia artificial (1). Asimismo, deberá incluir la capacidad de consumo necesaria para garantizar el funcionamiento del sistema durante un periodo mínimo de un (01) año, contado desde su puesta en producción.

La solución deberá diseñarse e implementarse bajo un enfoque agnóstico respecto del proveedor y de la tecnología de IA generativa. En ese sentido, no deberá incorporar dependencias innecesarias de componentes propietarios de una marca específica y deberá consumir el servicio mediante mecanismos de integración estandarizados, tales como API. Este enfoque deberá permitir la evolución de la solución y facilitar, de ser necesario, la sustitución del servicio o proveedor de IA generativa sin requerir modificaciones sustanciales en los demás componentes del sistema.

### RF-06: Clasificación de materia protegible

Cuando la creación contenga materia susceptible de protección mediante propiedad intelectual, el sistema deberá identificar y recomendar la modalidad de protección más probable, considerando, entre otras, las siguientes categorías: patente de invención, modelo de utilidad, diseño industrial, signos distintivos y derechos de autor, así como otras modalidades que sean identificadas durante la etapa de análisis.

### RF-07: Emisión de reportes de diagnóstico

El sistema deberá generar un reporte automatizado que indique el potencial de registro de la creación, proporcionando orientación práctica y recomendaciones sobre las modalidades de protección de propiedad intelectual aplicables. El reporte estará disponible para su visualización en el navegador web y descarga en formato PDF. El reporte generado deberá incluir de manera obligatoria y visible una cláusula de exención de responsabilidad jurídica (*disclaimer*), la cual especificará que los resultados constituyen una guía complementaria basada en IA y no reemplazan bajo ninguna circunstancia el juicio técnico, la evaluación experta ni las decisiones oficiales del personal examinador de la Entidad, salvaguardando el principio de supervisión humana.

### RF-08: Orientación complementaria y ruta de registro

El sistema deberá proporcionar información específica sobre cada modalidad de protección identificada, incluyendo los requisitos aplicables, pasos para su trámite, formatos de apoyo, tutoriales y/o enlaces a los servicios oficiales de asesoría correspondientes.
