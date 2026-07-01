STorM32 BGC
===========

<strong>STM32 32-bit microcontroller based 3-axis brushless gimbal controller board</strong>

schemes and designs by OlliW (except of STorM32 v4.1)<br>
v0.17: layout by Martinez and OlliW<br>
v4.1: design by KrattWorks

latest board version: v3.3, v4.1, v6.2

The STorM32 BGC boards and all other hardware published here are open source hardware, under the terms of the TAPR Open Hardware License as published by the Free Hardware Foundation, see http://www.tapr.org/ohl.html.

The firmwares are free and the GUI is open source, for the details of the terms of usage/licenses see <a href="http://www.olliw.eu/2013/storm32bgc">here</a>.

<strong>Further resources:</strong><br>- project web page http://www.olliw.eu/2013/storm32bgc (out-dated)<br>- thread at rcgroups http://www.rcgroups.com/forums/showthread.php?t=2055844<br>- wiki for the documentation http://www.olliw.eu/storm32bgc-wiki

## STorM32 v6.2 Board

General purpose boards specifically made for NT and TSTorM32 setups. STM32H7 based.

## STorM32 v4.1 Board

General purpose board, like v3.3 but with on-board motor drivers.

## STorM32 v3.3 Boards

General purpose boards specifically made for NT and TSTorM32 setups.

### STorM32 Micro Series

Series of stackable boards with 20x20 mm hole pattern: Main board, NT Motor-Encoder module, NT Triple Motor module, NT Logger module. 

<strong>changes in v3.3:</strong><br>- board specifically designed for NT and T-STorM32<br>- no motor drivers on board<br>- 3 NT plugs to make it easy to connect several NT modules<br>- NT-X plug carrying also the battery voltage<br>- 5 V power rail on the NT bus, with sufficient "juice"<br>- Rx&Tx on NT bus swapped, to avoid cable crossing to connect with NT modules<br>- support of stacking with a "high-power" extension board<br>- MPU9250 on board, spi (no i2c anymore!)<br>- firmware update procedure via USB<br>- ESP8266 port for WIFI connectability<br>- CAN bus port<br>- no BOOT0 button, smaller RESET button<br>- 0402 size parts<br>- board size as small as I could get it with a 2 layer design: 40 x 25 mm<br>- mounting holes, 3 mm diameter, 35 mm apart

## v1.x Boards

These boards will be phased out.

