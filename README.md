# filament-dryer
A simple filament dryer for drying 1 kg spools of filament. It's based around an Ender 3 heater and fan, combined with a PCB and another sensor. All controlled via Klipper. More information on CAD, firmware and the PCB is available in the folders.

<img width="294" height="379" alt="CAD model" src="https://github.com/user-attachments/assets/55805f72-6afa-4847-a3d5-faa922712fb1" />


## CAD
The filament is made for 3D printing and it will use about 350g of ABS/ASA. I deigned it in onshape, here is the [link](https://cad.onshape.com/documents/1bd024d5b7959acafc85207a/w/bc3f431890b8dcf2703dc2b2/e/cdbebe0165cb72dab1a66bad?configuration=open%3Dfalse&renderMode=0&uiState=6928c6e1034c4c312e27572e) if you want to see it yourself. Here are some more pictures from onshape:

<img width="119" height="300" alt="electronics" src="https://github.com/user-attachments/assets/6792c361-c955-457a-98a5-e498e4220d36" />
<img width="297" height="300" alt="side view" src="https://github.com/user-attachments/assets/b7215e63-8d3f-4dc1-a69e-65c53ee3de6b" />
<img width="209" height="300" alt="open" src="https://github.com/user-attachments/assets/ad07b4ce-cb2b-43a2-b5f6-fb68491db2a7" />


## PCB
It uses a custom 2 layer pcb, that's designed to be hand soldered. Most of the components are through hole and the one that isn't is pretty zasy to do yourself. Here are some pictures of the pcb:

<img width="300" height="300" alt="PCB 3D model" src="https://github.com/user-attachments/assets/bc2cf122-7300-4535-aa65-13ea3a191364" />
<img width="300" height="300" alt="PCB" src="https://github.com/user-attachments/assets/37c5080a-ef45-43cb-86f8-a145892d301d" />
<img width="424" height="300" alt="schematic" src="https://github.com/user-attachments/assets/9a250340-53d7-49de-a472-8f1badb93c04" />


## BOM
In the BOM it uses a pico W because that is the only one LCSC has. You could also use a normal pico, but then you will need to get it from somewhere else.

| Category | Item | Quantity | Minimum Order Quantity | Unit Price | Total Price | URL | Running Total |
| ---: | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| PCB Components | Capacitor 10µF | 1 | 1 |  $ 0.3996  | $0.40 | https://www.lcsc.com/product-detail/C531341.html |  $ 0.40  |
| PCB Components | Capacitor 22µF | 1 | 1 |  $ 1.2269  | $1.23 | https://www.lcsc.com/product-detail/C531341.html |  $ 1.63  |
| PCB Components | JST XH connector | 5 | 10 |  $ 0.0482  | $0.48 | https://www.lcsc.com/product-detail/C378939.html |  $ 2.11  |
| PCB Components | Screw Terminal | 2 | 5 |  $ 0.1102  | $0.55 | https://www.lcsc.com/product-detail/C8465.html |  $ 2.66  |
| PCB Components | Mosfet | 2 | 1 |  $ 0.8775  | $1.76 | https://www.lcsc.com/product-detail/C38774.html |  $ 4.41  |
| PCB Components | Resistor 100Ω | 2 | 50 |  $ 0.0110  | $0.55 | https://www.lcsc.com/product-detail/C120214.html |  $ 4.96  |
| PCB Components | Resistor 100KΩ | 2 | 20 |  $ 0.0242  | $0.48 | https://www.lcsc.com/product-detail/C119444.html |  $ 5.45  |
| PCB Components | Resistor 120Ω | 1 | 20 |  $ 0.0122  | $0.24 | https://www.lcsc.com/product-detail/C359996.html |  $ 5.69  |
| PCB Components | Resistor 7KΩ | 1 | 20 |  $ 0.0229  | $0.46 | https://www.lcsc.com/product-detail/C119429.html |  $ 6.15  |
| PCB Components | CAN Transceiver | 1 | 1 |  $ 2.6161  | $2.62 | https://www.lcsc.com/product-detail/C16468.html |  $ 8.77  |
| PCB Components | Voltage Regulator | 1 | 1 |  $ 3.5895  | $3.59 | https://www.lcsc.com/product-detail/C22371890.html |  $ 12.36  |
| PCB Components | Jumper | 1 | 5 |  $ 0.0880  | $0.44 | https://www.lcsc.com/product-detail/C265313.html |  $ 12.80  |
| PCB Components | AHT21 Sensor | 1 | 1 |  $ 1.5105  | $1.51 | https://www.lcsc.com/product-detail/C3012624.html |  $ 14.31  |
| PCB Components | Pico W | 1 | 1 |  $ 10.7204  | $10.72 | https://www.lcsc.com/product-detail/C7203003.html |  $ 25.03  |
| PCB Components | 1x20 Pin Header | 2 | 5 |  $ 0.0566  | $0.28 | https://www.lcsc.com/product-detail/C42431804.html |  $ 25.31  |
| PCB Components | LCSC Shipping | 1 |  |  $ 10.88  | $10.88 |  |  $ 36.19  |
| PCB | PCB (incl. shipping) | 1 | 1 |  $ 4.24  | $4.24 | https://jlcpcb.com/ |  $ 40.43  |
| Parts | Heater | 1 |  | (from Ender 3) |  |  |  $ 40.43  |
| Parts | 4010 Blower Fan | 1 |  | (from Ender 3) |  |  |  $ 40.43  |
| Case | Printed Parts | 350g |  |  (I already own)  |  |  |  $ 40.43  |
| Case | Screws M3x12 | 4 |  |  (I already own)  |  |  |  $ 40.43  |
| Case | Screws M3x8 | 2 |  |  (I already own)  |  |  |  $ 40.43  |
| Case | Screws M3x16 | 2 |  |  (I already own)  |  |  |  $ 40.43  |
| Case | M3 Nuts | 6 |  |  (I already own)  |  |  |  $ 40.43  |
| Case | voron inserts | 2 |  |  (I already own)  |  |  |  $ 40.43  |
