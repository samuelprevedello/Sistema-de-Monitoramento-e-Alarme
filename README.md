# Sistema-de-Monitoramento-e-Alarme
Manual

Objetivo do Projeto: O objetivo deste projeto foi desenvolver um sistema de monitoramento e alarme para uma indústria, utilizando duas placas ESP32 (ESP1 e ESP2). A ESP1 foi responsável por monitorar a temperatura e umidade em dois ambientes, enquanto a ESP2 foi encarregada de receber alertas e controlar um alarme composto por um buzzer e um LED.

Implementação da ESP1:

Monitoramento Ambiental: A ESP1 foi configurada para monitorar a temperatura e umidade utilizando sensores DHT22. Quando a temperatura atingia 60°C, os servos motores abriam as comportas para ativar o sistema de ventilação.
Controle via Slide Switch: Um slide switch foi implementado para desativar o envio de mensagens para a ESP2 e resetar os servos para a posição inicial.
Desafios na Comunicação: Embora a lógica para enviar mensagens via ESP-NOW tenha sido implementada, dificuldades técnicas impediram a comunicação entre as ESPs.
Implementação da ESP2:

Simulação do Alarme: Como a comunicação via ESP-NOW não pôde ser finalizada, a ESP2 foi configurada para simular o recebimento de um alerta e ativar o buzzer.
Controle do Alarme: O buzzer foi configurado para ser ativado e desativado com base no estado de um slide switch, permitindo um controle manual do alarme.
Conclusão Geral: Este projeto proporcionou uma oportunidade valiosa para explorar e aplicar conceitos de IoT, comunicação sem fio (ESP-NOW), e controle de dispositivos em tempo real. Apesar das limitações encontradas na comunicação entre as ESPs, todos os outros aspectos do sistema foram implementados com sucesso, e as funcionalidades essenciais foram testadas e confirmadas.
