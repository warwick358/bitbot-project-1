# project-1 BitBot lights and sound

## step 1 buzzer on
First we will get the "select bitbit modle" block from the "select bitbit modle" tab
and place it in the "on start" block.
Then we will get the "turn buzzer" block from "inputs and outputs" tab and place it under the "select bitbit modle" block
switch stur buzzer to "on"

```blocks
bitbot.select_model(BBModel.Classic)
bitbot.buzz(true)
```

## step 2 pause and buzzer off.
The next thing we need to do is put in a pause for the length of time we want the buzzer to be on.
Go to the "basic"tab and get the "pause" block and placce it under the "turn buzzer" block
Chamge the number in the block to 100
hen we will get the "turn buzzer" block from "inputs and outputs" tab and place it under the "select bitbit modle" block
switch stur buzzer to "off"
The go to the "basic"tab and get the "pause" block and placce it under the "turn buzzer" block
Chamge the number in the block to 200

```blocks
bitbot.select_model(BBModel.Classic)
bitbot.buzz(true)
basic.pause(100)
bitbot.buzz(false)
basic.pause(200)
```
## step 3 LED's
now we will use the onboard LED's 
go to the "bitbot" then the "fire led's" tab and ge the "set all LED's to" block.
place this under the last pause block and select a colour.

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
check the code and download to the microbit and connet to the bitbot.

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

