# Hospedagem-Container

Este é um repositório criado auxiliar no desenvolvimento e controle de um novo projeto pessoal. O projeto consiste em desenvolver um ambiente usando containers para hospedagem de aplicações web feitas em php.

## **Funcionamento básico**
Preciso declarar as variáveis para que a construção dos containeres aconteça de forma mais dinâmica. Todavia, atualmente, os comandos básicos são:
```
docker build -t basico .
docker-compose up -d
```
O primeiro cria o container da imagem e o segundo sobe os containeres do docker-compose

```
docker exec -it infraptans_mariazinha_1 sh -c "service php7.2-fpm start && nginx"
docker exec -it infraptans_joaozinho_1 sh -c "service php7.2-fpm start && nginx"
```

Estes comandos servem para iniciar o php e o nginx dentro dos containeres

### **Gerando certificados**

```
touch <path do acme>/acme.json
sudo chmod 600 <path do acme>/acme.json
```
