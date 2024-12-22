# ¿Qué es y cómo funciona el modelo HTTP?

HTTP (Hypertext Transfer Protocol) es un protocolo de comunicación que define cómo los navegadores (clientes) y los servidores intercambian información en la web. Este modelo sigue un esquema de solicitud y respuesta, lo que lo convierte en la base del funcionamiento de Internet.

## Partes esenciales del modelo HTTP

1. **Cliente y Servidor**  
   - **Cliente:** El navegador u otra aplicación que realiza solicitudes.  
   - **Servidor:** El sistema que recibe la solicitud y devuelve una respuesta, como una página HTML o un archivo.

2. **Métodos HTTP**  
   Son acciones que indican lo que el cliente desea hacer. Los principales son:  
   - `GET`: Solicita recursos (como una página web).  
   - `POST`: Envía datos al servidor.  
   - `PUT`: Actualiza recursos existentes.  
   - `DELETE`: Elimina recursos.  

3. **Mensajes HTTP**  
   - **Solicitud (Request):** Enviada por el cliente, incluye un método, una URL y opcionalmente datos adicionales.  
   - **Respuesta (Response):** Enviada por el servidor, incluye un código de estado (p. ej., 200 OK) y el contenido solicitado.

4. **Códigos de estado**  

   Informan sobre el resultado de la solicitud:  
   - `200`: Éxito.  
   - `404`: Recurso no encontrado.  
   - `500`: Error del servidor.

## Resumen del proceso HTTP

1. El cliente envía una solicitud al servidor utilizando un método HTTP.  
2. El servidor procesa la solicitud y envía una respuesta con el contenido y un código de estado.  
3. El cliente interpreta y muestra la información al usuario.
