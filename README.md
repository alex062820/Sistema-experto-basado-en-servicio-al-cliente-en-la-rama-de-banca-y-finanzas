# Sistema-experto-basado-en-servicio-al-cliente-en-la-rama-de-banca-y-finanzas
Representación del Conocimiento Programa - Sistema Experto 

// Simulación de un sistema de servicio al cliente en banca y finanzas

// Función para restablecer la contraseña
function restablecerContrasena(email) {
    console.log(`Se ha enviado un enlace para restablecer la contraseña a ${email}.`);
}

// Función para consultar saldo
function consultarSaldo() {
    console.log("Redirigiendo a la sección de consulta de saldo en la plataforma de banca en línea.");
}

// Función para iniciar un proceso de reclamo por transacción no reconocida
function iniciarReclamo() {
    console.log("Iniciando el proceso de reclamo y notificando al departamento de riesgo operacional.");
}

// Función para proporcionar detalles de una transferencia
function detallesTransferencia() {
    console.log("Proporcionando información sobre los requisitos y detalles del beneficiario para la transferencia.");
}

// Función para guiar al proceso de apertura de cuenta digital
function abrirCuentaDigital() {
    console.log("Guiando al cliente al proceso de apertura de cuenta en línea.");
}

// Función principal para gestionar las solicitudes del cliente
function gestionarSolicitud(solicitud, datos) {
    switch (solicitud) {
        case 'olvidarContrasena':
            restablecerContrasena(datos.email);
            break;
        case 'consultarSaldo':
            consultarSaldo();
            break;
        case 'transaccionNoReconocida':
            iniciarReclamo();
            break;
        case 'solicitarTransferencia':
            detallesTransferencia();
            break;
        case 'abrirCuentaDigital':
            abrirCuentaDigital();
            break;
        default:
            console.log("Solicitud no reconocida. Por favor, elija una opción válida.");
            break;
    }
}

// Ejemplo de uso del programa
let solicitudCliente = 'olvidarContrasena'; // Solicitud del cliente (puede ser 'consultarSaldo', 'transaccionNoReconocida', 'solicitarTransferencia', 'abrirCuentaDigital')
let datosCliente = { email: 'cliente@ejemplo.com' }; // Datos necesarios para la solicitud

// Gestionar la solicitud del cliente
gestionarSolicitud(solicitudCliente, datosCliente);

