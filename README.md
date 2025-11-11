https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Waterproof%20Temperature%20Sensor/%5B%20Multi%20%5D%20-%20Waterproof%20Temperature%20Sensor.jpg?raw=true

# Waterproof-Temperature-Sensor
**Waterproof Temperature Sensor** is a digital temperature sensor that provides accurate temperature readings in a compact and waterproof design. It communicates using the 1-Wire protocol, allowing multiple sensors to be connected on the same data line, each identified by a unique 64-bit serial code. It operates by detecting temperature through its internal circuit, converting the value into digital data, and then sending that data through the signal line to a microcontroller.

## **This sensor is suitable for:**
- Temperature monitoring system in aquariums
- Temperature control system in greenhouses or machinery

## **Specifications**
|Parameter|Value|
|-|-|
|**Model**|DS18B20|
|**Operating voltage (V)**|3.0 - 5.5 VDC|
|**Operating current (mA)**|~1.5 mA|
|**Adjustable Resolution**|9 - 12|
|**Operating Temperature Range**|-55°C to 125°C|
|**Accuracy**|±0.5°C|
|**Cable length**|100 cm|
|**Stainless Steel Tube Size**|6 × 45 mm|
|**Wiring connection**|Black wire - GND (Ground)|
||Red wire - VCC (Power supply +)|
||Yellow wire - DATA (Data Pin)| 

## Block Code Reference
|![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Waterproof%20Temperature%20Sensor/Water%20Temp%204.png?raw=true){{{width="150" height="auto"}}}| Use this block to set the sensor port (enter “1” if connected to port 1, or “2” for port 2)|
|-|-|
|![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Waterproof%20Temperature%20Sensor/Water%20Temp%205.png?raw=true){{{width="200" height="auto"}}}|**Use this block to read the temperature from the sensor in degrees Celsius (°C).**|

![Description](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Ultrasonic%20Sensor/Example%20code.png?raw=true){{{width="250" height="auto"}}} 
[**Download the working code here**](https://code.gogoboard.org/#/program/b906ff4a-7f70-4ad3-a25d-d040269c1430)

## **Required Equipment**
|Waterproof Temperature Sensor|![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/sensor/Temperature%20Sensor.png?raw=true){{{width="200" height="auto"}}}|
|-|-|
|**Pin-to-Grove Adapter (for use with GoGo Board)**|![Description](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Waterproof%20Temperature%20Sensor/water%20temp%20groove.png?raw=true){{{width="200" height="auto"}}}|
|**Grove cable**|![Description](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Ultrasonic%20Sensor/only%20grove%20(test).png?raw=true){{{width="200" height="auto"}}}|
|**Computer or Tablet**|![Description](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Ultrasonic%20Sensor/computer%20or%20tablet.png?raw=true){{{width="200" height="auto"}}}|
|**GoGo Board and USB-C cable**|![Description](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Ultrasonic%20Sensor/gogoboard%20and%20usb.png?raw=true){{{width="200" height="auto"}}}|

## **How to use**
**1. Connect the GoGo Board**
- Connect the GoGo Board to your computer or tablet via USB-C cable or Wi-Fi
![](https://github.com/thegogoboard/gogodoc/blob/main/Automation/Image%20(91).jpg?raw=true){{{width="500" height="auto"}}}

**2. Connect the Waterproof Temperature Sensor**
There are two ways to connect the sensor:
**Option 1:** Using a Grove Connector
- Connect the Waterproof Temperature Sensor to a Pin-to-Grove Adapter
- Plug the Grove cable into an configurable port on the GoGo Board

  ![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Waterproof%20Temperature%20Sensor/Water%20Temp.gif?raw=true){{{width="500" height="auto"}}}

**Option 2:** Using Jumper Wires (Dupont Wires)
- If you don’t have a Pin-to-Grove Adapter, you can use jumper wires to connect the sensor directly to the pins on the GoGo Board

![Description](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Waterproof%20Temperature%20Sensor/water%20temp%20with%20adapter.png?raw=true){{{width="500" height="auto"}}} ![Description](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Waterproof%20Temperature%20Sensor/water%20temp%20with%20board.png?raw=true){{{width="500" height="auto"}}}


## Getting Started with the Waterproof Temperature Sensor on GoGo Code 

**1. Visit the GoGo Code website:**
- Go to [GoGo Code](https://code.gogoboard.org/#/program) to start programming and controlling your device.

**2. Add the Waterproof Temperature Sensor extension:**
- Click on the **Add Extension** category

![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Waterproof%20Temperature%20Sensor/Water%20Temp%201.gif?raw=true){{{width="1000" height="auto"}}}

- Select **Official**, then click the **[ Multi ] - Waterproof Temperature Sensor** card. The system will automatically return to the main page.

![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Waterproof%20Temperature%20Sensor/Water%20Temp%202.gif?raw=true){{{width="1000" height="auto"}}}

**3. Add sensor command blocks:**
- Click on the **[ Multi ] - Waterproof Temperature Sensor** category. You will see two available blocks:

![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Waterproof%20Temperature%20Sensor/Water%20Temp%203.gif?raw=true){{{width="1000" height="auto"}}}

**4. Write a simple program to display sensor data:**
- Drag the **"Setup DS18820 Sensor with: input port..."** block into the start block.
- Go to the **Math** category and drag a number block into the  **input port** field.
- Use the **show number** block from the **Built-in Display** category.
- Insert the **"Temperature of DS18B20 (°C)"** block into the show number block.
- To display the value continuously, place everything inside the **"forever do each time wait..."** block from the **Loops** category.
![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Waterproof%20Temperature%20Sensor/Water%20Temp%206.png?raw=true){{{width="500" height="auto"}}}

**5. Download and test your code:**
- Click **Download**, then click **Run Code** to start running your program.
![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Waterproof%20Temperature%20Sensor/Water%20Temp%207.gif?raw=true){{{width="1000" height="auto"}}}
  
  **Cautions**
- Avoid modifying wires or connecting them incorrectly, as this may damage the device.
- Do not touch the sensor head while it is operating, as it may affect detection accuracy.
- If the sensor does not work, check the voltage and wiring connections.
:::
