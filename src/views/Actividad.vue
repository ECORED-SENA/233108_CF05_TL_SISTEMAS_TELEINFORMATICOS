<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
      // Para cuestionario usar: <ActividadController :cuestionario="cuestionario"/>
      // Para parrafo usar: <ActividadController :parrafo="parrafo"/>
      #Actividad                
      <ActividadController :cuestionario="cuestionario"/>

</template>

<script>
import ActividadController from '@ecored-sena/boulder-kit/plugin/components/actividad/ActividadController.vue'

export default {
  name: 'ActividadDidactica',
  components: {
    ActividadController,
  },
  data: () => ({
    cuestionario: {
      tema: 'Cuestionario conceptual',
      titulo: 'Cuestionario',
      introduccion:
        '<b>Objetivo:</b> evaluar el nivel de comprensión y aplicabilidad de las estrategias de recursos para determinar la gestión de las redes de datos en las organizaciones.',
      barajarPreguntas: false,
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO',
      preguntas: [
        {
          id: 1,
          texto: '¿En qué consiste HTTP?',
          imagen: '@/assets/actividad/imagen1.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Permite la solicitud y transferencia de documentos web.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto:
                'Permite la transferencia de mensajes de correo electrónico.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Permite la transferencia de archivos entre dos sistemas finales.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Permite tener un sistema de nombres de dominio.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto:
            'Lo sentimos, su respuesta no es la correcta. <em>Board</em> del <em>software</em> EAGLE.',
        },
        {
          id: 2,
          texto: '¿En qué consiste SMTP?',
          imagen: '@/assets/actividad/imagen2.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Permite la solicitud y transferencia de documentos web.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Permite la transferencia de mensajes de correo electrónico.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto:
                'Permite la transferencia de archivos entre dos sistemas finales.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Permite tener un sistema de nombres de dominio.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 3,
          texto: '¿En qué consiste FTP?',
          imagen: '@/assets/actividad/imagen3.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Permite la solicitud y transferencia de documentos web.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Permite la transferencia de mensajes de correo electrónico.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Permite la transferencia de archivos entre dos sistemas finales.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Permite tener un sistema de nombres de dominio.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 4,
          texto: '¿En qué consiste DNS?',
          imagen: '@/assets/actividad/imagen4.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Permite la solicitud y transferencia de documentos web.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Permite la transferencia de mensajes de correo electrónico.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Permite la transferencia de archivos entre dos sistemas finales.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Permite tener un sistema de nombres de dominio.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 5,
          texto: '¿Qué es Retraso de procesamiento?',
          imagen: '@/assets/actividad/imagen1.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'El tiempo necesario para examinar la cabecera del paquete y determinar a dónde dirigirlo.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Espera ser transmitido al enlace.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Sólo puede transmitirse después de que se hayan transmitido todos los paquetes.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Tiempo necesario para propagarse desde el principio del enlace hasta el router de destino.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
