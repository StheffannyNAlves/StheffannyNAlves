<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0d1117&height=200&section=header&text=Stheffanny&fontSize=70&fontColor=ffffff&fontAlign=50&fontAlignY=35&animation=twinkling&desc=Embedded%20Security%20and%20Digital%20Forensics&descSize=20&descAlign=50&descAlignY=60" width="100%"/>
</div>

<div align="center">
  
  <img src="https://img.shields.io/badge/C-Bare--Metal-00599C?style=for-the-badge&logo=c&logoColor=white" />
  <img src="https://img.shields.io/badge/Assembly-ARM-red?style=for-the-badge&logo=arm&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-Forensics-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Hardware-Security-black?style=for-the-badge&logo=hack-the-box&logoColor=white" />
  <br/>
  <img src="https://img.shields.io/badge/MCU-%20%7C%20RP2040-blue?style=for-the-badge&logo=stmicroelectronics&logoColor=white" />
  <img src="https://img.shields.io/badge/Tools-GDB%20%7C%20OpenOCD-green?style=for-the-badge&logo=gnu&logoColor=white" />

</div>

<br/>

## Sobre Mim

Graduanda em Eng. de Computação(UEFS). 

Meu estudo atual foca em **Embedded Cybersecurity** e **Low-Level Forensics**, auditando a segurança de microcontroladores e desenvolvendo métodos de extração de evidências que eliminam abstrações de software.

Atuo investigando a integridade física e lógica de sistemas embarcados, com ênfase em:

* 🕵️‍♀️ **Forensics:** Extração direta de memória (SWD/MMIO) e análise de *dump* de firmware.
* 🛡️ **Defensive:** Implementação de Secure Boot, MPU Hardening e TrustZones.
* ⚔️ **Offensive:** Learning Fault Injection.

---

### Foco de Estudo e Desenvolvimento

| Categoria | Stack |
| :--- | :--- |
| **Linguagens** | C (Bare-Metal), Assembly (ARM Thumb-2), Python (Scripting & Analysis)|
| **Hardware Alvo** |  Dual-Core Cortex-M0+ (RP2040)|
| **Protocolos** | UART, SPI, I2C (Low-level implementation & Sniffing) |
| **Engenharia Reversa** | Ghidra, GDB, Binwalk, Wireshark |

---

## Projetos

### 🔬 Projeto Dolos — Forensic SWD Probe
> Bare-metal firmware extractor for RP2040 via SWD — no RTOS, no abstractions.

Dolos é uma ferramenta forense que extrai firmware de microcontroladores via SWD
usando um RP2040 como probe, sem depender de OpenOCD ou abstrações de SO.
Projetado para cenários onde a integridade da evidência não pode ser comprometida
por camadas de software intermediárias.

**Decisões arquiteturais:**
- **Multicore split** — Core 1 dedicado ao bit-banging SWD para garantir
  determinismo temporal; Core 0 gerencia USB CDC e logging
- **Static LUT error policy** — substituiu FSM simples, cada código de falha
  mapeia diretamente para uma política de resposta sem overhead de estado
- **Circular log buffer com chain-of-custody** — garante rastreabilidade
  mesmo sob condições de falha
- **Pico SDK intencional** — usado como camada de abstração de hardware
  controlada, não como atalho; decisão documentada e justificada

**Stack:** C bare-metal · RP2040 · SWD · USB CDC · TinyUSB

[→ Repositório](https://github.com/StheffannyNAlves/swd-forensic-extractor)




---

### Contato

> Estudante de Engenharia de Computação buscando oportunidades em suporte técnico
e infraestrutura de TI enquanto desenvolvo pesquisa em segurança embarcada.

---
<div align="center">
  <img height="180" src="https://github-readme-stats-virid-six-52.vercel.app/api?username=StheffannyNAlves&show_icons=true&theme=dracula&hide_border=true&cache_bust=12345" alt="Sthe Stats" />
  <img height="180" src="https://github-readme-stats-virid-six-52.vercel.app/api/top-langs/?username=StheffannyNAlves&layout=compact&theme=dracula&hide_border=true&cache_bust=12345" alt="Sthe Languages" />
</div>





<div align="center">
  <h3>🗺️ Mapa de Contribuição</h3>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/StheffannyNAlves/StheffannyNAlves/output/github-contribution-grid-snake-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/StheffannyNAlves/StheffannyNAlves/output/github-contribution-grid-snake.svg">
    <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/StheffannyNAlves/StheffannyNAlves/output/github-contribution-grid-snake.svg">
  </picture>
</div>
