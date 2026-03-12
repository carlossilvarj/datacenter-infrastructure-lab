# Investigação de Saturação de CPU em Linux

## Objetivo

Demonstrar como investigar situações onde um servidor Linux apresenta uso elevado de CPU.

## Cenário

Servidor em produção apresentando lentidão causada por alto consumo de CPU.

## Ferramentas utilizadas

top  
uptime  
htop  
pidstat  
ps  

## Passo 1 — Verificar carga do sistema

uptime

Analise o **load average**.

---

## Passo 2 — Identificar processos que consomem CPU

top

---

## Passo 3 — Listar processos ordenados por uso de CPU

ps -eo pid,comm,%cpu --sort=-%cpu | head

---

## Passo 4 — Analisar uso de CPU por processo

pidstat 1

---

## Conclusão

A análise estruturada permite identificar rapidamente a origem do consumo de CPU em ambientes de produção.
Add CPU saturation investigation lab
