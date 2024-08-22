# gogo7-br
Informações sobre a GoGo Board versão 7 para uso no Brasil

<img src="https://github.com/arnans/gogo7-sesi/blob/main/GoGo%207C.png" width="250">

Este repositório contém informações de fabricação e teste da Plataforma de Robótica Educacional GoGo Board. A GoGo Board foi criada em colaboração entre a Universidade de Chiang Mai na Tailândia e a Universidade de Columbia em Nova Iorque, EUA. A GoGo Board é uma plataforma de computação física que tem como pré-requisito pouca ou nenhuma experiência com programação/eletrônica, mas permite que crianças a partir dos 10 anos explorem ideias importantes em STEAM e Pensamento Computacional. Ela é adequada para trabalhos em áreas como Automação, Internet das Coisas (IoT), Análise de Dados e Inteligência Artificial (IA).

<img src="https://github.com/arnans/gogo7-sesi/blob/main/2024%20Sensor%20Set%207C/3D_PCB_GoGo%207C.png" width="500">

Sensor Set is a collection of useful sensors, actuators, and cable adapters that allows practical useage of the GoGo Board. The modules mainly uses the Grove and JST connectors. The set is manufactured as a panel to ease distribution. The individual modules can be broken off by hand upon first use. 

# Overview 

## The GoGo 7 Hardware

<img src="https://github.com/arnans/gogo7-sesi/blob/main/gogo%207%20diagram/GoGo%207C%20Top%201.jpg" width=640>

### Componentes conforme mostrado acima

- **Display Colorido**: Display de 1,8 polegadas. Permite o controle básico e a leitura de várias entradas e saídas.
- **D-Pad**: Um joystick para navegar na tela.
- **USB-C**: Usado para fornecer energia e se comunicar com a aplicação web de programação.
- **Chave On-Off**: Controla a energia fornecida à placa.
- **Entradas de Sensores**: 4 portas de entrada de sensores analógicos.
- **Portas de Saída**: 4 portas bidirecionais disponíveis usando um conector JST. Cada porta é capaz de conduzir 1A a 5V.
- **Portas para Servomotor & Relé**: 4 digital control ports. Can drive Servo Motors or Relays.
- **Portas de Extensão**: Isso inclui o Multi-dispositivo, Configurável, Extensão 1, 2 e o Barramento de Extensão de Saída.

<img src="https://github.com/arnans/gogo7-sesi/blob/main/gogo%207%20diagram/GoGo%207C%20Top%202.jpg" width=400>

### Componentes conforme mostrado acima

- **LEDs de Status**: Mostra o estado de execução/parada do código do usuário.
- **Sensors Integrados**: Microfone Digital (Intensidade de Som), IMU (Aceleração e Giro), Brilho, Proximidade.
- **Transmissor e Receptor Infravermelho**

<img src="https://github.com/arnans/gogo7-sesi/blob/main/gogo%207%20diagram/GoGo%207C%20Back.jpg" width=500>

### Componentes conforme mostrado acima

- **ESP32-S3**: CPU principal. Executa o sistema operacional da GoGo Board e o código do usuário.
- **ESP32-C3**: CPU auxiliar. Contém o firmware Tasmota por padrão. Este núcleo possui uma porta USB-C dedicada para atualizar o firmware.
- **Botões de Boot**: Usados para atualizar as CPUs correspondentes via porta USB-C.
- **Ponte-H Drivers, I2C Driver chip**: Usados para acionar as portas de saída. Eles são controlados via chip Driver I2C I/O.
- **Buzzer**: Um buzzer Piezo.
- **Limitador de Corrente**: Evita corrente de surto nos motores servo.
- **Pinos de Expansão de I/O**: Fornecem capacidades de expansão para a GoGo Board.
- **Divisor de 5 para 3,3 volts**: Interface ADC para a CPU.

## O Ambiente de Programação GoGo 7

<img src="https://github.com/arnans/gogo7-sesi/blob/main/gogo%207%20diagram/code.gogoboard.png" width=800>

Esta aplicação web possui as seguintes capacidades
- [Accesso via https://code.gogoboard.org](https://code.gogoboard.org)
- Conecta-se à GoGo Board usando USB, Wi-Fi ou laboratório remoto.
- Oferece uma programação moderna baseada em blocos.
- Contém cartões para monitorar e configurar várias funcionalidades.
- Armazenamento em nuvem. O código pode ser salvo e compartilhado na nuvem.
- Ferramentas de aprendizagem. Laboratório de Dados, Sala de Aula, Interface Web para controle remoto e mais.

# Informações de Fabricação

Esses arquivos são para a versão 7C da GoGo Board
- [Arquivos PCB Gerber](https://github.com/arnans/gogo7-sesi/blob/main/Gerber_PCB_GoGo_7C_2024-05-18.zip) - A GoGo Board 7 usa uma PCB de 4 camadas.
- [Arquivo Pick and Place](https://github.com/arnans/gogo7-sesi/blob/main/PickAndPlace_PCB_GoGo%207C_2024-05-18.xlsx)
- [Bill of Materials](https://github.com/arnans/gogo7-sesi/blob/main/BOM_GoGo%207_PCB_GoGo%207C_2024-05-18.xlsx)
- Renderização 3D [[Top](https://github.com/arnans/gogo7-sesi/blob/main/GoGo%207C%203D%20topview.png) | [Bottom](https://github.com/arnans/gogo7-sesi/blob/main/GoGo%207C%203D%20bottomview.png)]
- Fotos:foto da palca montada [[Superior](https://github.com/arnans/gogo7-sesi/blob/main/2024%2007%20GoGo%207C%20Photos/PXL_20240725_035141521.MP.jpg) | [Perspectiva Superior](https://github.com/arnans/gogo7-sesi/blob/main/2024%2007%20GoGo%207C%20Photos/PXL_20240725_035324777.MP.jpg) | [Inferior](https://github.com/arnans/gogo7-sesi/blob/main/2024%2007%20GoGo%207C%20Photos/PXL_20240725_035150818.MP.jpg) | [Perspectiva Inferior](https://github.com/arnans/gogo7-sesi/blob/main/2024%2007%20GoGo%207C%20Photos/PXL_20240725_035346049.MP.jpg)]
- Firmware: [Main CPU (ESP32-S3) and Tasmota Core (ESP32-C3)](https://github.com/arnans/gogo7-sesi/blob/main/firmware)
- [Procedimento de Teste e Controle de Qualidade](https://docs.google.com/document/d/1wkHplLRawxpCvvXY5K_7zhaUBPVLWB5iVyL8zbxunkI/edit#heading=h.g8lrajqe9t70)

# GoGo Sensor Set 7C

<img src="https://github.com/arnans/gogo7-sesi/blob/main/2024%20Sensor%20Set%207C/GoGo%20Sensor%20Set%207C%20Diagram.png" width="900">

There are a total of 14 different module types on the panel as follows:

- 2x Grove to Terminal Block Adapter
- 2x Grove to 3-pin Servo Motor Adapter
- 2x Grove to Grove Extension
- 2x JST to JST Extension
- 1x Rain Sensor
- 1x Joystick (5-ways)
- 1x Red/Blue LED pair
- 2x Whte LEDs
- 1x Digital Temperature and RH sensor
- 1x Potentiometer (Knob)
- 2x Limit Switches
- 1x Luminosity Sensor
- 2x IR Proximity Sensor

# Informações de Fabricação

- [PCB Gerber Files](https://github.com/arnans/gogo7-sesi/blob/main/2024%20Sensor%20Set%207C/Gerber_PCB_GoGo_7_-_Sensor_Set_7c_-_vcut_2024-05-31.zip)
- [Pick and Place File](https://github.com/arnans/gogo7-sesi/blob/main/2024%20Sensor%20Set%207C/PickAndPlace_PCB_GoGo%207%20-%20Sensor%20Set%207c%20-%20vcut_2024-05-31.xlsx)
- [Bill of Materials](https://github.com/arnans/gogo7-sesi/blob/main/2024%20Sensor%20Set%207C/BOM_GoGo%207%20-%20Sensor%20Set_PCB_GoGo%207%20-%20Sensor%20Set%207c%20-%20vcut_2024-05-31.xlsx)
- [3D Render of the board](https://github.com/arnans/gogo7-sesi/blob/main/2024%20Sensor%20Set%207C/Sensor%20Set%207C%203D%20Perspective.png)
- Photos of an assembled board [[Top](https://github.com/arnans/gogo7-sesi/blob/main/2024%20Sensor%20Set%207C/Photos/sensor%20set%207c%20top%20view.jpg) | [Bottom](https://github.com/arnans/gogo7-sesi/blob/main/2024%20Sensor%20Set%207C/Photos/sensor%20set%207c%20bottom%20view.jpg) | [Perspective](https://github.com/arnans/gogo7-sesi/blob/main/2024%20Sensor%20Set%207C/Photos/sensor%20set%207c%20perspective.jpg)]


# License

This work is licensed under a Creative Commons Attribution-NonCommercial (CC BY-NC) license. You are free to share, copy, and redistribute the material in any medium or format. However, any commercial use of this work is strictly prohibited without prior written consent from the author. Contact arnan.s@cmu.ac.th for more information.

<img src="https://mirrors.creativecommons.org/presskit/buttons/88x31/png/by-nc.png" width="100">

