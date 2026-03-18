# DNS

<blockquote>
   $TTL 604800<br>
@   IN  SOA ns1.lab.local. admin.lab.local. (<br>
            2024010101  ; Serial<br>
            3600        ; Refresh<br>
            1800        ; Retry<br>
            604800      ; Expire<br>
            604800 )    ; Negative Cache TTL<br>
<br>
@   IN  NS  ns1.lab.local.<br>
<br>
ns1             IN  A   192.168.100.10<br>
ubuntu-server   IN  A   192.168.100.10<br>
windows-server  IN  A   192.168.100.20<br>
 </blockquote>
