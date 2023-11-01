---
label: Add Input Binding
order: 59

icon: "/static/arrowi.png"
---
# Input Binging

Set up for keyboard and gamepad


# Setting

<style>
    .sample {
        text-align: center;
        color: #1956AF;
        border-radius: 10px;
        background-color: #ffb300;
        border: 1px solid #1956AF;
        padding-top: 20px;
        margin-bottom: 20px;
    }
</style>

:::sample
 Folder :  `Content/ModularMenu/Demo/ThirdPerson/Input/TestIMCS`
:::

:: Follow This Path

    Open [IMC_Default_Test]
    Open [Mappings] accordion section
    Open [IA_Jump] accordion section
    Add a control binding and bind key
    Open [Player Mappable Options] accordion section
    Set [Name] row any string
    Set [Display Name][!Unique!] the same string for the row where all action keys are located
    Set [Display Category] Keyboard or Gamepad
    Open your project directory and delete Saved folder

::

: Variables

`Name` -> Internal Name Of Input For Binding Can be same or different [AnyString]

`Display Name` -> Display Name Of Input All Action Keys Must Be Same [UniqueDisplayLabel]

`Display Category` -> Display Category Of Input [Gamepad] or [Keyboard] For Binding

:
