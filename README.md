# LAB05
# Integrantes:

1. Ahumada Soles Carlos
   
2. Calluchi Patiño Eduardo

3. Principe Huamanchumo Luis

4. Sandoval Vargas Robert

5. Correa Asencio Damer

# instrucciones
1. Posicionarse en la carpeta del proyecto Ansible:

```bash
cd ansible
```

2. Verificar el inventario:

```bash
ansible-inventory -i inventory.ini --list
```
3. Probar conectividad con los nodos:

```bash
ansible all -i inventory.ini -m ping
```

4. Ejecutar el playbook del balanceador de carga:

```bash
ansible-playbook -i inventory.ini playbook.yaml
```

5. Una vez desplegado, probar acceso al balanceador desde el host:

```bash
curl http://localhost:5010
```
