# Installation

- Installation
    - [Requirements](#requirements)
    - [Installing RageUI](#installing-rageui)
    - [Using RageUI](#using-rageui)

<a name="requirements"></a>
### Requirements

<div class="content-list" markdown="1">
 - GIT
 - FXServer
</div>

<a name="installing-rageui"></a>
### Installing RageUI

First you will need to download the latest version of the project by executing the following command in the folder where your resources are located.

    git clone https://github.com/iTexZoz/RageUI.git RageUI
    
Once this is done you just need to add in your server configuration the RageUI resource startup.

    start RageUI

Then you have to create your new resource in which you want to use the library, once this is done restart your server.

<a name="using-rageui"></a>
### Using RageUI in your resources

To use RageUI in your resources, you just need to modify the resource's manifest. 
If you want to include the whole library in a global way, just copy and paste the code below.

    client_scripts {
        "@RageUI/RMenu.lua",
        "@RageUI/menu/RageUI.lua",
        "@RageUI/menu/Menu.lua",
        "@RageUI/menu/MenuController.lua",
    
        "@RageUI/components/Audio.lua",
        "@RageUI/components/Enum.lua",
        "@RageUI/components/Keys.lua",
        "@RageUI/components/Rectangle.lua",
        "@RageUI/components/Sprite.lua",
        "@RageUI/components/Text.lua",
        "@RageUI/components/Visual.lua",
    
        "@RageUI/menu/elements/ItemsBadge.lua",
        "@RageUI/menu/elements/ItemsColour.lua",
        "@RageUI/menu/elements/PanelColour.lua",
    
        "@RageUI/menu/items/UIButton.lua",
        "@RageUI/menu/items/UICheckBox.lua",
        "@RageUI/menu/items/UIList.lua",
        "@RageUI/menu/items/UISeparator.lua",
        "@RageUI/menu/items/UISlider.lua",
        "@RageUI/menu/items/UISliderHeritage.lua",
        "@RageUI/menu/items/UISliderProgress.lua",
    
        "@RageUI/menu/panels/UIColourPanel.lua",
        "@RageUI/menu/panels/UIGridPanel.lua",
        "@RageUI/menu/panels/UIPercentagePanel.lua",
        "@RageUI/menu/panels/UIStatisticsPanel.lua",
    
        "@RageUI/menu/windows/UIHeritage.lua",
    }

All I have to do now is back up and restart your server, congratulations you now have RageUI working on your resources.
