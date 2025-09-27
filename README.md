LAB05

Ahumada Soles Carlos
Calluchi Patiño Eduardo
Principe Huamanchumo Luis
Sandoval Vargas Robert
Asencio Correa Damer

instrucciones
1. Posicionarse en la carpeta del proyecto Ansible:

bash
cd ansible


2. Verificar el inventario:

bash
ansible-inventory -i inventory.ini --list


3. Probar conectividad con los nodos:

bash
ansible all -i inventory.ini -m ping


4. Ejecutar el playbook del balanceador de carga:

bash
ansible-playbook -i inventory.ini playbook.yaml


5. Una vez desplegado, probar acceso al balanceador desde el host:

bash
curl http://localhost:5010
