# Linux Performance Diagnostics Lab

## Objetivo

Demonstrar um fluxo profissional de diagnóstico de lentidão em servidores Linux.

## Cenário

Servidor Linux apresentando lentidão em ambiente de produção.

O objetivo é identificar rapidamente o gargalo seguindo um fluxo estruturado de análise.

## Ferramentas utilizadas

top  
uptime  
vmstat  
iostat  
df  
ss  
sar  

## Fluxo profissional de diagnóstico

1. CPU
2. Memória
3. IO
4. Disco
5. Rede
6. Aplicação

## Verificando CPU
top
uptime
ps -eo pid,comm,%cpu --sort=-%cpu


## Verificando memória


free -h
vmstat 1


## Verificando IO


iostat -xz 1


Observe:

- await
- %util
- fila de disco

## Verificando disco


df -h
du -sh /var/*


Discos acima de 85% podem gerar impacto imediato.

## Verificando rede


ss -tulpn
sar -n DEV 1 3


## Conclusão

Diagnóstico estruturado economiza tempo e evita decisões erradas em produção.

Fluxo recomendado:

CPU → RAM → IO → Disco → Rede → Aplicação 
