# YetAnotherRuggedMeshtasticEUD
A huge thanks to anvlmedia. This build is based off of his initial design for a rugged Meshtastic enclosure. Our modifications externalize the LoRa and GPS antennas. Additionally, we also make use of a weather resistant USB-C adapter in place of the original Fischer connector to increase accessibility.
 
## Assembly

### Parts List
- 1x [Lid](https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/Mechanical/STLs/Lid.stl)
- 1x [Main Body](https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/Mechanical/STLs/Main%20Body.stl)
- 1x [Gasket](https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/Mechanical/STLs/Gasket.stl)
- 1x [Knob](https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/Mechanical/STLs/Knob.stl)
- 1x [56D36-01-2-AJN Rotary Switch](https://www.digikey.com/en/products/detail/grayhill-inc/56D36-01-2-AJN/98655?s=N4IgTCBcDaIKwDYAiBmBBaADARnWdAggFIByIAugL5A) or [56SDP36-01-2-AJN Rotary Switch](https://www.digikey.com/en/products/detail/grayhill-inc/56SDP36-01-2-AJN/2678565)
- 1x [USB-C Adapter](https://www.aliexpress.us/item/3256804440339698.html?spm=a2g0o.order_list.order_list_main.69.551b1802ttIMoC&gatewayAdapt=glo2usa)
- 1x [USB-C Adapter Cap](https://www.aliexpress.us/item/3256805936943547.html?spm=a2g0o.order_list.order_list_main.74.551b1802ttIMoC&gatewayAdapt=glo2usa)
- 2x [SMA Connector](https://www.digikey.com/en/products/detail/gct/cab412rf-0100-a-1-e/22251137)
- 3x [Light Pipe](https://www.digikey.com/en/products/detail/visual-communications-company-vcc/LMC-080-CTP/4515531?so=90373260&content=productdetail_US&mkt_tok=MDI4LVNYSy01MDcAAAGX0MQASlnBdqnk_A_6-qsaQpySAVFtRW1V2aL_yuqiJkK8GdLw7qbNu7k92KyTDxIo68lhwqGd2r5rppqj1dw4OAeHWfHPXsyYTJiT8VoO)
- 6x [M3 Brass Insert](https://www.mcmaster.com/94180A331/)
- 6x [M3 x 30mm Screws](https://www.mcmaster.com/91294A141/)
- 1x [RAK19007](https://store.rakwireless.com/products/rak19007-wisblock-base-board-2nd-gen)
- 1x [Wisblock GPS Module](https://store.rakwireless.com/products/wisblock-gnss-location-module-rak12500)
- 1x RAK Core Module
- 1x [2.0 JST Connector](https://www.amazon.com/dp/B07NWD5NTN?ref_=ppx_hzsearch_conn_dt_b_fed_asin_title_1)
- 1x 3.7v 504050 LiPo Battery

### Assembly of components

#### Rotary Switch
1. Install the end stop pins that came with your switch in the positions shown in the following image where one is placed between `9` and `10`, and the other is placed between `1` and `2`.
    - *Note: Before installing the pins, ensure the flat side of the rotary switch shaft is at position `5` or `6`*
      <p align="left"><img alt="Switch Pins" src="https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/images/switch_pins.jpg" width="500"></p>

3. Solder the black wires of your male and female JST cables together
4. Solder the red wire of the male JST cable to the "6-10" center pin of the rotary switch
5. Solder the red wire of the female JST cable to the `6` pin
    - *Note: Your wiring should look like the following image*
      <p align="left"><img alt="Wiring" src="https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/images/switch_wiring.jpg" width="500"></p>

6. Install all of your bulkhead components including SMA connectors, rotary switch, and USB connector
    - *Note: The USB connector can only be installed one way*
    - *Note: The rotary switch must be installed to that postitions `5` and `6` are facting up*
      <p align="left"><img alt="Bulkhead" src="https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/images/bulkhead.jpg" width="500"></p>

#### Main Board
1. Install the Wisblock GPS module on the RAK19007 board using the included small screw
      <p align="left"><img alt="GPS" src="https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/images/gps_module.jpg" width="500"></p>
      
3. Insert the USB-C plug of the USB-C adapter into your RAK19007 board
    - *Note: Route the cable so that it tucks under the SMA pigtails and rotary switch*
      <p align="left"><img alt="USB Cable" src="https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/images/usb_cable.jpg" width="500"></p>

4. Install the main board into the main enclosure body using the RAK included screws
5. Connect the pigtail cables to their respective IPEX connectors including the BLE antenna that came with your RAK device
6. Press fit the BLE antenna in the small slot next to the main board
      <p align="left"><img alt="BLE Antenna" src="https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/images/ble_antenna.jpg" width="500"></p>

#### Enclosure
1. Install six M3 brass inserts in the back of the enclosure main body
      <p align="left"><img alt="Brass" src="https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/images/threads.jpg" width="500"></p>
      
2. Install three light pipes in the `C`, `H`, and `U` positions on your enclosure lid
      <p align="left"><img alt="Light Pipes" src="https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/images/light_pipe.jpg" width="500"></p>

3. Using double-sided tape, attach your LiPo pack to the inside of the enclosure lid
      <p align="left"><img alt="Battery" src="https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/images/battery_placement.jpg" width="500"></p>

4. Place the gasket and lid onto the enclosure main body so that the gasket is between the lid and main body
      <p align="left"><img alt="Gasket" src="https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/images/gasket.jpg" width="500"></p>

5. Using six M3x30mm screws, fasten the enclosure shut
6. Install the power switch knob onto the rotary switch
      <p align="left"><img alt="Gasket" src="https://github.com/justcallmekoko/YetAnotherRuggedMeshtasticEUD/blob/main/images/switch_cover.jpg" width="500"></p>

## Usage
- **The design is not intended to be waterproof.** It is simply meant to be water and dust resistant
- To power the unit on, place the switch in the `I` position
- To power the unit off, place the switch in the `O` position
- Charge and program the device through the USB-C power mounted to the enclosure bulkhead
- When connected to USB-C power, the device will only charge the battery when the switch is in the `I` position
- When connected to USB-C power, the device will power on even if the switch is in the `O` position
- Connect a GPS antenna to the SMA connector labeled `G`
- Connect a LoRa antenna to the SMA connector labeled `L`
- Use the side grid panel for indentification markings

## Extra Printed Components
- There are extra files located in the "STL" folder if you wish to print your own light pipes and USB passthrough.
  
  <a href="https://github.com/workshop35/YARM_EUD_stuff/blob/06f0664fd07bfb7e5f15abcb8ad2165e72d469b8/Mechanical/STLs/mainBodyEdit.3mf">Case</a>
  
  <a href="https://github.com/workshop35/YARM_EUD_stuff/blob/06f0664fd07bfb7e5f15abcb8ad2165e72d469b8/Mechanical/STLs/usbPassthrough.3mf">USB Passthrough</a>

  <a href="https://github.com/workshop35/YARM_EUD_stuff/blob/0d7214ca557dbc08e7389d28ac9c6c2bc0039537/Mechanical/STLs/usbNut.3mf">Nut</a>
  
  <a href="https://github.com/workshop35/YARM_EUD_stuff/blob/06f0664fd07bfb7e5f15abcb8ad2165e72d469b8/Mechanical/STLs/usbCap.3mf">Dust Cap</a>
  
  <a href="https://github.com/workshop35/YARM_EUD_stuff/blob/06f0664fd07bfb7e5f15abcb8ad2165e72d469b8/Mechanical/STLs/capLanyard.3mf">Cap Lanyard</a>

  <a href="https://github.com/workshop35/YARM_EUD_stuff/blob/0d7214ca557dbc08e7389d28ac9c6c2bc0039537/Mechanical/STLs/lightPipe.3mf">Light Pipe</a>

- Extra Purchase
  [USB-C Breakout Boards](https://a.co/d/73ktVuH)

   https://github.com/user-attachments/assets/33cab01c-ab12-4689-82cd-6a3599bcc097


- The case is modified to remove the lanyard opening, the antenna mounting flange thickness is reduced, the the USB passthrough opening was altered.
  <p align="left"><img alt="Case" src="https://github.com/workshop35/YARM_EUD_stuff/blob/28bed2836d53fdf2c32b75fd225b185d3f1ab35f/images/caseEdit.png" width="500"></p>
  
- The lightpipe is printed in clear PETG. **The "Arachne" wall generator was used in OrcaSlicer.** Insert a pipe into each opening and fix with an adhesive.
  <p align="left"><img alt="Light Pipe" src="https://github.com/workshop35/YARM_EUD_stuff/blob/28bed2836d53fdf2c32b75fd225b185d3f1ab35f/images/petgLightPipe.png" width="500"></p>

- The USB passthrough is four parts: USB-C holder, retention nut, cap, and lanyard. The lanyard was printed in TPU.
  <p align="left"><img alt="Components" src="https://github.com/workshop35/YARM_EUD_stuff/blob/28bed2836d53fdf2c32b75fd225b185d3f1ab35f/images/usbPassthrough.png" width="500"></p>

- Press-fit the female USB breakout board into the holder. This is a very tight fit and may require adjustments to the print depending on your printer.
  <p align="left"><img alt="USB Pressed-In" src="https://github.com/workshop35/YARM_EUD_stuff/blob/1ecce05b40116ae93a889a9c6f5ca5a717c85e53/images/usb_pressed.jpg" width="500"></p>

- Cut roughly two inches of a four-conductor ribbon cable (four individual wires also work). Solder one end to the female USB breakout in the holder from the previous step. Solder the other to a male USB breakout. The connections are straight through without crossover. Use 3/8" or equivalent shrink tube to insulate the connections.
   <p align="left"><img alt="USB Cable" src="https://github.com/workshop35/YARM_EUD_stuff/blob/afdc7702d2fe8f17967b4ad596d43a6f0784559c/images/usb_cable_complete.jpg" width="500"></p>

- Install the male end of the cable into the RAK19007 board. You may have to loosen the board for it to fit. **This will not fit into the original case, you must use the modified version linked above**.
  <p align="left"><img alt="Cable Install" src="https://github.com/workshop35/YARM_EUD_stuff/blob/afdc7702d2fe8f17967b4ad596d43a6f0784559c/images/usb_installed.jpg" width="500"></p>

- Verify functionality by connecting a USB power source.
  <p align="left"><img alt="Ops Check" src="https://github.com/workshop35/YARM_EUD_stuff/blob/afdc7702d2fe8f17967b4ad596d43a6f0784559c/images/usb_charging.jpg" width="500"></p>  
