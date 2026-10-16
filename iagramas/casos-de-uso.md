flowchart LR
  V[Visitante] --> C((Consultar animales))
  S[Solicitante / Adoptante] --> C
  S --> A((Enviar solicitud de adopción))
  S --> E((Consultar estado de solicitud))
  O[Operador] --> R((Registrar reporte de riesgo))
  CO[Coordinador] --> AS((Asignar caso de rescate))
  CO --> ES((Supervisar estado del caso))
  RE[Rescatista] --> DR((Registrar rescate))
  VE[Veterinario] --> HV((Registrar evaluación veterinaria))
  AD[Encargado de adopciones] --> RV((Revisar solicitud))
  AD --> DA((Registrar entrega))
  ADM[Administrador] --> GU((Gestionar usuarios y roles))
  R --> AS
  AS --> DR
  DR --> HV
  HV --> C
  A --> RV
  RV --> DA
