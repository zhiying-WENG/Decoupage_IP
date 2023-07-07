# Decoupage_IP  

### **Symétrique:**  
  
maximun est 50 équipements dans 4 groups --> 2^6 = 64 >= 50+2, 32-6 = 26  


|   | L'adresse réseau | L'adresse de broadcast |  Adresse de début de plage | Adresse de fin de plage |
| :----- | :----: | :----: | :----: | :----:  |
| Le Pôle informatique: | 172.16.1.0/26  | 172.16.1.63 |  172.16.1.1  |  172.16.1.62 |
| Le Pôle développement: | 172.16.1.64/26 | 172.16.1.127 | 172.16.1.65 |  172.16.1.126      |
| Le Pôle Administratif | 172.16.1.128/26 | 172.16.1.191      |   172.16.1.129     |  172.16.1.190      |
| Le Pôle Technicien | 172.16.1.192/26 | 172.16.1.255      |   172.16.1.193     |  172.16.1.254      |  
_ _ _   
### **Asymétrique:**  
  
Le Pôle informatique (6 bureaux, environ 50 équipements au total) --> 2^6 = 64 >= 50+2, 32-6 = 26  

Le Pôle développement (6 bureaux, environ 12 équipements au total) --> 2^4 = 16 >= 12+2, 32-4 = 28  

Le Pôle Administratif (4 bureaux, environ 20 équipements au total) --> 2^5 = 32 >= 20+2, 32-5 = 27

Le Pôle Technicien (4 bureaux, environ 15 équipements au total) --> 2^5 = 32 >= 15+2, 32-5 = 27  

|   | L'adresse réseau | L'adresse de broadcast |  Adresse de début de plage | Adresse de fin de plage |
| :----- | :----: | :----: | :----: | :----:  |
| Le Pôle informatique: | 172.16.1.0/26  | 172.16.1.63 |  172.16.1.1  |  172.16.1.62 |
| Le Pôle développement: | 172.16.1.64/28 | 172.16.1.79 | 172.16.1.65 |  172.16.1.78 |
| Le Pôle Administratif | 172.16.1.80/27 | 172.16.1.111|   172.16.1.81 |  172.16.1.110 |
| Le Pôle Technicien | 172.16.1.112/27 | 172.16.1.143 | 172.16.1.113 |  172.16.1.142 |