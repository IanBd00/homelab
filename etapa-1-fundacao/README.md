# Etapa 1: Fundação

Topologia da rede:

!(topologia/Topologia.png)

Versões usadas: 

• VirtualBox 7.2.6<br>
• Ubuntu Server 24.04<br>
• Windows Server 2022

Configuração de Rede:

•IPs<br>
•Adaptadores NAT<br>
•Rede Interna

Comandos usados para configurar o netplan:

•sudo nano /etc/netplan/00-installer-config.yaml<br>
•sudo chmod 600 /etc/netplan/00-installer-config.yaml<br>
•sudo netplan apply<br>
•ip addr show

YAML de rede:

<blockquote>

```yaml
network:
  version: 2
  ethernets:
    enp0s3:
      dhcp4: true
    enp0s8:
      dhcp4: no
      addresses:
        - 192.168.100.10/24
    enp0s9:
      dhcp4: no
      addresses:
        - 192.168.56.10/24
```
</blockquote>

Acertos e falhas:

•Utilização do ssh-keygen de forma corrreta e sem erros<br>
•Facilidade no entendimentos dos comandos<br>
•Problemas da aplicação da chave pública por meio do ssh-copy-id (Necessidade de criar uma Host-Only)


