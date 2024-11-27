# Motor Tutorial

## Schritt1
Nimm einen Motor und schließe ihn an Port #1 an. Schreibe einen Code, um die folgenden Aufgaben zu erfüllen:

1. Benutze den Knopf 'A' um Motor 1 mit der Geschwindigkeit 50 zu starten. Stoppe dann Motor 1 mit Knopf 'B'.
2. Benutze den Knopf 'A', um Motor 1 für 4 Umdrehungen laufen zu lassen. Benutzen Sie den Knopf 'B', um Motor 1 um 360 Grad zu drehen.
3. Benutzen Sie den Knopf 'A', um Motor 1 für 5 Sekunden laufen zu lassen.

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
ms_nezhaV2.oledClear()
ms_nezhaV2.oledShowNumber(1234, 1)
ms_nezhaV2.oledShowText("Hello!", 1)
 ms_nezhaV2.ledBrightness(PlanetX_Display.DigitalRJPin.J1, false)
input.onButtonPressed(Button.A, function () {  
})
input.onGesture(Gesture.Shake, function () {
})
ms_nezhaV2.onUltrasonicSensorTriggered(PlanetX_Display.DigitalRJPin.J1, 10, PlanetX_Basic.Distance_Unit_List.Distance_Unit_cm, function () {
})
ms_nezhaV2.onCrashSensorPressed(PlanetX_Display.DigitalRJPin.J1, function () {
})
```