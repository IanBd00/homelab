# 🌐 Etapa 2 - Serviços de Rede (DHCP, DNS e Nginx)

Nesta etapa do homelab, implementei serviços essenciais de rede, simulando um ambiente corporativo básico.

## 📡 DHCP (Dynamic Host Configuration Protocol)

O DHCP foi configurado para distribuir automaticamente endereços IP na rede.

### 🔄 Funcionamento (DORA)

O processo de obtenção de IP ocorre em 4 etapas:

1. **Discover** – cliente procura um servidor DHCP<br>
2. **Offer** – servidor oferece um IP disponível<br>
3. **Request** – cliente solicita o IP oferecido<br>
4. **Acknowledge** – servidor confirma a atribuição

---

## 🌍 DNS (Domain Name System)

O DNS foi configurado para resolver nomes dentro da rede local.

### 🔧 Arquivos utilizados:

- `named.conf.local` → define as zonas<br>
- `db.lab.local` → contém os registros DNS

### 🧪 Testes

```bash
dig lab.local
nslookup lab.local
