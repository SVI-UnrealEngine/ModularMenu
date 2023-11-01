---
label: Add Input Context
order: 58
icon: "/static/arrowi.png"
---
# New Input Context

Add a IMC structure for input binding

# Setting

:: Creation Path

    Create [IMC_Default_{customname}]
    Open [Mappings] accordion section
    Add [IA_youraction] accordion section
    Add a control binding and bind a key
    Open [Player Mappable Options] accordion section
    Set [Name] row any string
    Set [Display Name]-[Unique]- the same string for the row where all action keys are located
    Set [Display Category] Keyboard or Gamepad
    Duplicate [IMC_Default_{customname}]
    Set duplicated IMC name to [IMC_Mappable_{customname}]
    Open your project directory and delete Saved folder
::


 Variables
    
 `Name` -> Internal Name Of Input For Binding Can be same or different [AnyString]
    
`Display Name` -> Display Name Of Input All Action Keys Must Be Same [UniqueDisplayLabel]
    
  `Display Category` -> Display Category Of Input [Gamepad] or [Keyboard] For Binding
    
    

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
 Folder :  `Content/ModularMenu/Widgets/LayoutComponents/LC_TabPanel`
:::

:: Set Up Path

    Open [LC_TabPanel]
    Select MC_InputBindList on the hierarchy
    Examine [Details] panel
    Find [Default] section
    Add item on [ContextIMC]
    Set Up your input block with new created IMC

::

