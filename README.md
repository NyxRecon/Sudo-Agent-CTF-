![Nmap](screenshots/agent_sudo_capa.png)
# Sudo-Agent-CTF 🛸
Write-up do Sudo Agent CTF (TryHackMe), com enumeração, exploração web, esteganografia, SSH e privilege escalation via CVE-2019-14287.

## 📌 Informações da Máquina

| Item        | Informação                                      |
| ----------- | ----------------------------------------------- |
| Plataforma  | TryHackMe                                       |
| Sistema     | Linux                                           |
| Dificuldade | Easy                                            |
| Objetivo    | Web exploitation, FTP,SSH, esteganografia e privilege escalation |
| CVE         | CVE-2019-14287                                  |
| Status      | Completed ✅                                    |

## 🛠️ Ferramentas utilizadas

```text
Nmap
Hydra
User-Agent Switcher
FTP
Binwalk
John the Ripper
7-Zip
Steghide
SSH
Linux Commands
Browser
```

# Reconhecimento

## Scan de portas:
O primeiro passo da etapa de reconhecimento foi identificar as portas abertas.
Realizei o scan de portas com nmap:
```bash
nmap -sV -sC sudoagent
```
## Portas abertas:
```bash
21/tcp open  ftp     
22/tcp open  ssh
80/tcp open  http
```
# Enumeração Web

Realizando a análise da aplicação web, me deparei com a seguinte mensagem:


