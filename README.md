# ProyectoCita-JavaEmpresarial

-- Crear una superclase de persona, donde dependera paciente y medico
-- Crear clases de citas, citapresencial, domiciliar y virtual
-- Expediente
-- Distribucion medica, y tambien el rango hora
-- Tipo Cita, Estado Cita
-- Subservicio, Modalidad, Institucion
-- Crear las excepciones sobre cupos, paciente y medico no repetible, expediente unico, fecha no valida, cambiocita no permitido, cita vencida


Super Clase Persona
Atributos: idPersona, nombre, apellido, fechaNacimiento, dui, telefono, correo, direccion

Clase Paciente
hereda de Persona
Atributos: idPaciente, numeroExpediente, tipoSangre

Clase Medico
heresa de Persona
Atributos: idMedico, numeroJunta, poseeEspecialidad, cargo, horarioAtencion
