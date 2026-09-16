# ProyectoCita-JavaEmpresarial

-- Crear una superclase de persona, donde dependera paciente y medico
-- Crear clases de citas, citapresencial, domiciliar y virtual
-- Expediente
-- Distribucion medica, y tambien el rango hora
-- Tipo Cita, Estado Cita
-- Subservicio, Modalidad, Institucion
-- Crear las excepciones sobre cupos, paciente y medico no repetible, expediente unico, fecha no valida, cambiocita no permitido, cita vencida


Super Clase Persona
Atributos: idPersona, nombre, apellido, fechaNacimiento, documento, telefono, correo, direccion, condicion

Clase Paciente
hereda de Persona
Atributos: idPaciente, numeroExpediente, tipoSangre

Clase PersonalMedico
heresa de Persona
Atributos: numeroJunta, poseeEspecialidad, cargo, horarioAtencion, documento
    SubClase Medico : 
        SubClase MedicoGeneral : 
        SubClase MedicoEspecializado : + especialidades
    SubClase Enfermera : 
    SubClase Licenciado : 
    

Clase Expediente
Atributos: numero, fecha_creacion, estado

Clase Cita
Atributos: fecha, distribucion, estado, reprogramada
    SubClase CitaPresencial: + fechaHora
    SubClase CitaDomiciliar: + direccion
    SubClase CitaVirtual: + url

Clase Distribucion
Atributos: medico, rangohora, especialidad


Excepciones:
    TelefonoInvalido
    CorreoElectronicoInvalido

    PersonaInexistente
    PersonaFallecida
    DocumentoPacienteNoDisponible
    ExpedienteNoDisponible
    FechaNacimientoInvalida

    MedicoNoDisponible
    MedicoInexistente
    DocumentoMedicoNoDisponible
    NumeroJuntaNoDisponible
    EspecialidadInexistente

    CitaVencida
    CitaCancelada
    CitaReprogramada
    UrlInvalida
    HorarioNoValido
    HorarioNoDisponible

    CargoNoDisonible





















