<div align="center">

# 📄 Whitepaper: Data Sovereignty in Digital Psychotherapy
## El Imperativo Ético del Edge-AI en Salud Mental

**Author / Autor:** Jhon Andry, B.S.  
**Date / Fecha:** 2026-08-12  
**Version / Versión:** 1.0-draft

</div>

---

## 📌 Executive Summary / Resumen Ejecutivo

**[EN]** Digital psychotherapy is at an ethical crossroads. Current tools —telepsychology platforms, mental health apps, generative AI assistants— operate under a model that treats patient data as remote computational resource. Therapy session audio, children's projective drawings, voice patterns of a person in crisis: all travel to servers the therapist does not control, in unknown jurisdictions, under privacy policies that change without notice.

**[ES]** La psicoterapia digital está en una encrucijada ética. Las herramientas actuales —plataformas de telepsicología, apps de salud mental, asistentes de IA generativa— operan bajo un modelo que trata los datos del paciente como recurso computacional remoto. El audio de una sesión de terapia, los dibujos proyectivos de un niño, los patrones de voz de una persona en crisis: todo viaja a servidores que el terapeuta no controla, en jurisdicciones desconocidas, bajo políticas de privacidad que cambian sin aviso.

**[EN]** This whitepaper argues that **data sovereignty in psychotherapy is not a technical problem solved by better encryption.** It is an ethical problem demanding a different architecture: local processing, device sovereignty, auditable code transparency.

**[ES]** Este whitepaper argumenta que **la soberanía de datos en psicoterapia no es un problema técnico que se resuelve con mejor cifrado.** Es un problema ético que exige una arquitectura diferente: procesamiento local, soberanía del dispositivo, transparencia auditable del código.

**Cortex-Protocol** and **Neuro-Synapse Core** are a concrete proposal.  
**Cortex-Protocol** y **Neuro-Synapse Core** son una propuesta concreta.

---

## 1️⃣ The Problem / El Problema

### 1.1 The Illusion of Consent / La Ilusión del Consentimiento

**[EN]** When a therapist uses a commercial platform, the patient "accepts" terms nobody reads. But professional secrecy is not negotiable by contract. A psychologist cannot delegate patient confidentiality to a corporation's service clause.

**[ES]** Cuando un terapeuta usa una plataforma comercial, el paciente "acepta" términos que nadie lee. Pero el secreto profesional no es negociable por contrato. Un psicólogo no puede delegar la confidencialidad del paciente a una cláusula de servicio.

### 1.2 Business Model as Conflict of Interest / Modelo de Negocio como Conflicto

**[EN]** Mental health platforms monetize data. Even when they say "we don't sell your data," model training, contextual advertising, and aggregated insights are indirect monetization. The economic incentive is against privacy.

**[ES]** Las plataformas de salud mental monetizan datos. Incluso cuando dicen "no vendemos tus datos", el entrenamiento de modelos, la publicidad contextual y los insights agregados son monetización indirecta. El incentivo económico está en contra de la privacidad.

### 1.3 Legal Vulnerability / Vulnerabilidad Jurídica

**[EN]** A court order in the server's country can compel the company to hand over therapy session data. The therapist, who swore to protect the patient, has no control.

**[ES]** Una orden judicial en el país del servidor puede obligar a la empresa a entregar datos de sesiones terapéuticas. El terapeuta, que juró proteger al paciente, no tiene control.

---

## 2️⃣ The Proposal / La Propuesta

### 2.1 Principles / Principios

| # | Principle / Principio |
|---|----------------------|
| 1 | **Data never leaves the professional's device.** / Los datos nunca salen del dispositivo del profesional. |
| 2 | **AI runs locally.** / La IA corre localmente. |
| 3 | **Code is auditable.** / El código es auditable. |
| 4 | **Therapist has absolute control.** / El terapeuta tiene control absoluto. |
| 5 | **Cryptography is the boundary, not policy.** / La criptografía es el límite, no la política. |

### 2.2 Architecture / Arquitectura

```
┌─────────────────────────────────────────────────────────────┐
│  THERAPIST'S DEVICE (Edge) / DISPOSITIVO DEL TERAPEUTA      │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────────────┐ │
│  │ Local Audio │  │ Local Camera│  │ Encrypted History   │ │
│  │ (Prosody)   │  │ (HTP/Visual)│  │ (SQLCipher + TPM)   │ │
│  └──────┬──────┘  └──────┬──────┘  └─────────────────────┘ │
│         │                │                                   │
│  ┌──────▼────────────────▼───────────────────────────────┐  │
│  │           Local LLM (Llama 3.2 1B/3B)                │  │
│  │           Clinical assistance, NOT diagnosis         │  │
│  └──────────────────────────────────────────────────────┘  │
│                          │                                  │
│  ┌───────────────────────▼───────────────────────────────┐  │
│  │           Therapist UI (Total Control)                │  │
│  └───────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────┘
        [NO INTERNET REQUIRED / SIN INTERNET REQUERIDA]
        [NO EXTERNAL SERVERS / SIN SERVIDORES EXTERNOS]
```

---

## 3️⃣ Clinical Practice Implications / Implicaciones Clínicas

### 3.1 Therapist as Guardian / Terapeuta como Guardián

**[EN]** In the traditional model, the therapist is a "user" of a platform. In the Cortex model, the therapist is the **sovereign guardian** of patient data. Technology is their tool, not intermediary.

**[ES]** En el modelo tradicional, el terapeuta es "usuario" de una plataforma. En el modelo Cortex, es el **guardián soberano** de los datos del paciente. La tecnología es su herramienta, no su intermediario.

### 3.2 AI as Assistant / La IA como Asistente

**[EN]** Local AI suggests interpretations based on biomarkers. Therapist validates, corrects, or discards. The system learns therapist preferences, not a global "all patients" model.

**[ES]** La IA local sugiere interpretaciones basadas en biomarcadores. El terapeuta valida, corrige o descarta. El sistema aprende las preferencias del terapeuta, no un modelo global de "todos los pacientes".

### 3.3 Research Without Exploitation / Investigación Sin Explotación

**[EN]** Therapists can voluntarily export anonymized data. This is an **active opt-in**, not a terms-of-use condition. Research is not built on exploiting patient vulnerability.

**[ES]** Los terapeutas pueden exportar datos anonimizados voluntariamente. Esto es una **opción activa**, no una condición de uso. La investigación no se construye sobre la explotación de la vulnerabilidad del paciente.

---

## 📢 Call to Action / Llamado a la Acción

**[EN]**
- **Psychologists:** Demand tools that demonstrably respect professional secrecy.
- **Developers:** Join open standards for ethical digital mental health.
- **Regulators:** Privacy in mental health requires architectures, not just policies.
- **Patients:** Ask your therapist where your data ends up. You have the right to know.

**[ES]**
- **Psicólogos:** Exijan herramientas que respeten el secreto profesional de forma demostrable.
- **Desarrolladores:** Únanse a estándares abiertos para salud mental digital ética.
- **Reguladores:** La privacidad en salud mental requiere arquitecturas, no solo políticas.
- **Pacientes:** Pregunten a su terapeuta dónde terminan sus datos. Tienen derecho a saber.

---

## 📚 References / Referencias

- APA. (2017). *Ethical Principles of Psychologists and Code of Conduct.*
- EU. (2016). *GDPR, Art. 9.*
- Cavoukian, A. (2009). *Privacy by Design.*
- Mittelstadt, B. D., et al. (2016). The ethics of algorithms. *Big Data & Society.*

---

<div align="center">

**[EN]** Open draft. Comments welcome via GitHub Issues.  
**[ES]** Borrador abierto. Comentarios bienvenidos vía GitHub Issues.

*"Technology must serve human biology — not the other way around."*  
*"La tecnología debe servir a la biología humana — no al revés."*

</div>
