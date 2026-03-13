# Linux Datacenter Infrastructure Lab

Laboratório prático de troubleshooting e diagnóstico de infraestrutura Linux.

Este repositório contém laboratórios que simulam problemas reais encontrados em ambientes de produção.

---

## Laboratórios disponíveis

- [Diagnóstico de Desempenho do Linux](labs/linux-performance-diagnostics)
- [Investigação de Saturação de CPU](labs/cpu-saturacao)
- Análise de Pressão de Memória (em breve)
- Incidente de Disco Cheio (em breve)
- Investigação de Gargalo de IO (em breve)

---

## Fluxo profissional de diagnóstico

CPU → Memória → IO → Disco → Rede → Aplicação

---

## Fluxo de investigação
+------+
| CPU  |
+------+
    ↓
+------+
| RAM  |
+------+
    ↓
+------+
| IO   |
+------+
    ↓
+------+
| Disk |
+------+
    ↓
+------+
| Net  |
+------+
    ↓
+------+
| App  |
+------+

---

## Estrutura do repositório

```
labs/
 ├─ linux-performance-diagnostics
 │   └─ README.md
 ├─ cpu-saturacao
 │   └─ README.md
```

Cada pasta contém um laboratório baseado em cenários reais de troubleshooting em servidores Linux.
