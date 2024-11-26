# Motor Tutorial
### @hideIteration true
```package
ms_nezhaV2=github:MINTspark/pxt-mintspark-ikv2
```
```blocks
basic.showNumber(0)
basic.pause(100)
basic.showLeds(`
    . . . . .
    . . . . .
    . . . . .
    . . . . .
    . . . . .
    `)
basic.showIcon(IconNames.Heart)
basic.showString("Hello!")
basic.clearScreen()
basic.forever(function () { 
})
music.play(music.tonePlayable(262, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
ms_nezhaV2.runMotor(MotorConnector.M1, 20)
ms_nezhaV2.stopMotor(MotorConnector.M1)
ms_nezhaV2.runMotorFor(MotorConnector.M1, 20, 1, MotorMovementMode.Turns)
input.onButtonPressed(Button.A, function () {  
})
input.onGesture(Gesture.Shake, function () {
})
```
## Step1
Take a Motor and connect it to port #1. Write code to complete the following tasks:

1. Use button 'A' to start motor 1 with speed 50. Then stop motor 1 with button 'B'.
2. Use button 'A' to run motor 1 for 4 revolutions. Use button 'B' to run motor 1 for 360 degrees.
3. Use button 'A' to run motor 1 for 5 seconds.