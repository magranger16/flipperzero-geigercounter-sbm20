# flipperzero-geigercounter
A geiger counter application for the Flipper Zero

<img src="https://github.com/nmrr/flipperzero-geigercounter/blob/main/img/logo.jpg" width=30% height=30%>

You need a **geiger counter** board to run this application. This board can be used : https://aliexpress.com/item/1005004074447209.html

The geiger counter board can be powered with +5V power pin of the **Flipper Zero** 

Output pin for measure on arduino cannot be used on the **Flipper Zero** because output voltage is too low. You can use jack out port instead. This port must be connected on **A7** GPIO.

## Build the program

Assuming the toolchain is already installed, copy **flipper_geiger** directory to **applications_user**

Plug your **Flipper Zero** and build the geiger counter :
```
./fbt launch_app APPSRC=applications_user/flipper_geiger
```

The program will automatically be launched after compilation

<img src="https://github.com/nmrr/flipperzero-geigercounter/blob/main/img/flipper1.png" width=25% height=25%>

## Use cases

Ambient radioactivity :

<img src="https://github.com/nmrr/flipperzero-geigercounter/blob/main/img/flipper2.png" width=25% height=25%>

Measure of uranium ore piece inside a lead container :

<img src="https://github.com/nmrr/flipperzero-geigercounter/blob/main/img/flipper3.png" width=25% height=25%>

Measure of uranium ore in contact with the geiger tube :

<img src="https://github.com/nmrr/flipperzero-geigercounter/blob/main/img/flipper4.png" width=25% height=25%>

All previous measures in a row (the scale of the graph is automatically adjusted) :

<img src="https://github.com/nmrr/flipperzero-geigercounter/blob/main/img/flipper5.png" width=25% height=25%>
