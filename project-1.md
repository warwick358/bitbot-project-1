# project-1 BitBot lights and sound

## step 1 
Buzzer On

First we will get the "select bitbit model" block from the "select bitbit model" tab and place it in the "on start" block.
Then we will get the "turn buzzer" block from "inputs and outputs" tab and place it under the "select bitbit model" block switch buzzer to "on".

```blocks
bitbot.select_model(BBModel.Classic)
bitbot.buzz(true)
```

## step 2 
Pause and Buzzer Off.

The next thing we need to do is put in a pause for the length of time we want the buzzer to be on.
Go to the "basic" tab and get the "pause" block and place it under the "turn buzzer" block
Change the number in the block to 100.
Then we will get the "turn buzzer" block from "inputs and outputs" tab and place it under the "select bitbit model" block switch the buzzer to "off"
The go to the "basic" tab and get the "pause" block and place it under the "turn buzzer" block
Change the number in the block to 200

```blocks
bitbot.select_model(BBModel.Classic)
bitbot.buzz(true)
basic.pause(100)
bitbot.buzz(false)
basic.pause(200)
```
## step 3 
LED's

Now we will use the onboard LED's 
Go to the "bitbot" then the "fire led's" tab and get the "set all LED's to" block.
Place this under the last pause block and select a colour.

```block
bitbot.select_model(BBModel.Classic)
bitbot.buzz(true)
basic.pause(100)
bitbot.buzz(false)
basic.pause(200)
bitbot.setLedColor(0xFF0000)
basic.forever(function () {
```
## step 4 Connect to bitbot
Check the code and download to the microbit and connect to the bitbot.

```block

bitbot.select_model(BBModel.Classic)
bitbot.buzz(true)
basic.pause(100)
bitbot.buzz(false)
basic.pause(200)
bitbot.setLedColor(0xFF0000)
basic.forever(function () {
    
})
```


