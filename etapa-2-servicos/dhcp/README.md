# Etapa 2 : Serviços

<h3>🌐 Configuração de DHCP</h3>

<blockquote>

subnet 192.168.100.0 netmask 255.255.255.0 {<br>
  range 192.168.100.50 192.168.100.100;<br>
  option routers 192.168.100.1;<br>
  option domain-name-servers 192.168.100.10;<br>
}



  </blockquote>
