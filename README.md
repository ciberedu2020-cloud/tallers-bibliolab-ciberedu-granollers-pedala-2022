# De la dada al núvol · Tallers participatius del 2022

Materials dels tallers amb què va començar el projecte de sensors de qualitat de l'aire de
**CiberEdu**, fets el 2022 amb Bibliolabs i Granollers Pedala. Expliquen per què mesurem les
partícules de l'aire, com es van construir els dispositius i com es connectaven al WiFi.

Es guarden **tal com es van fer**, com a document històric. Algunes coses han canviat des de
llavors: mira l'apartat «Què ha canviat» abans de fer-los servir per muntar o connectar un sensor.

## Els documents

| Fitxer | Què és |
| --- | --- |
| [1-bibliolabs-granollers-pedala.pdf](1-bibliolabs-granollers-pedala.pdf) | Presentació del taller: per què és important l'aire que respirem, què són les partícules (PM), dades de Granollers i el pla del dia (construir els nous models, més econòmics). |
| [2-anem-a-construir.pdf](2-anem-a-construir.pdf) | Com es munta el sensor: components (placa ESP8266, pantalla 1602 LCD, semàfor, sensor ZH03B, protoboard i capsa impresa en 3D) i com es connecta cada peça a la placa. |
| [3-anem-a-connectar.pdf](3-anem-a-connectar.pdf) | Com s'instal·lava el semàfor en un lloc i com es connectava al WiFi amb el mòbil. |

El programa original de les plaques és públic a
[github.com/Dracvar06/environmental_pollution](https://github.com/Dracvar06/environmental_pollution)
(«A maker project to learn about environmental pollution»).

## Què ha canviat des del 2022

- **Servidor.** Les dades anaven a un servidor de FAGOM, que ja no funciona. Des del 2026 els
  sensors envien a un servei al núvol (flespi), una Raspberry Pi les guarda i es poden veure a la
  pàgina pública del projecte.
- **Programa.** Totes les plaques porten un programa nou (2026). El WiFi es configura igual, amb
  el mòbil, però la xarxa del sensor ara es diu **CIBEREDU-Sensor** i no té contrasenya
  (els passos i la contrasenya de «Anem a connectar» ja no serveixen).
- **Connexió del sensor.** «Anem a construir» connecta el sensor a **RX i TX** (fil groc a RX,
  fil verd a TX). Algunes capses es van muntar més endavant amb el sensor a **D7 i D8** (fil groc
  a D7, fil verd a D8). El programa del 2026 prova tots dos muntatges i es queda amb el que
  funciona, però si muntes o revises una capsa, comprova a quins pins va cada fil.
- **Pantalla i semàfor** es connecten igual que al document: pantalla a D1/D2, semàfor a D5
  (vermell), D4 (groc) i D3 (verd).

## Contacte

CiberEdu · ciberedu2020@gmail.com
