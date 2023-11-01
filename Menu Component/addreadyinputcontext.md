---
label: Add Ready Input Context
order: 57
icon: "/static/arrowi.png"
---

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


# New Ready Input List [Without IMC]

Add a Input List structure for input binding/settings

# Setting

:::sample
 Folder :  `Content/ModularMenu/Widgets/MenuComponents/InputBind/ReadyInputList_Mouse`
:::

:: Creation Path

    Create custom blueprint base of [ReadyInputBindList]
    Name it like ReadyInputList_{yourlistname}
    Open and switch to Graph
    Delete all event on Graph
    In MyBlueprint panel click setting icon
    Enable [ShowInheritedVariable]
    On Graph select a [Event Reset Save Data]
    Return to Designer
    Open [ReadyInputList_Mouse]
    Copy hierarchy structure for easy implementation
    Paste on your own ReadyInputBindList
    Examine all component and add your own
    Return to Graph on [Event Reset Save Data]
    Drag your MC_{components} and in this component call [ResetSave] function
    Connect all execution pin to [Event Reset Save Data]
    Your Graph must be like [ReadyInputList_Mouse] Graph
::


 MC_[component] Variables
    
 `Slot Name` -> Save Slot name [AnyString]
    
`Default Value` -> Default value of setting [For Slider like components (check range of data in component) ]
    
`Default State` -> Default value for flag/boolean options [For Toggle like components]
    
    

:::sample
 Folder :  `Content/ModularMenu/Widgets/LayoutComponents/LC_TabPanel`
:::

:: Set Up Path

    Open [LC_TabPanel]
    Select MC_InputBindList on the hierarchy
    Examine [Details] panel
    Find [Default] section
    Add item on [Context Ready Input Lists]
    Set Up your input block with new created ReadyInputList_{yourlistname}

::