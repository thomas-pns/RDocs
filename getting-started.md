# Getting Started

- Getting Started
    - [Create a menu](#create-menu)
    - [Managing the opening of the menu](#keys-managing)
    - [Menu displaying Tick](#display)
    - [The result you must have obtained](#result)

Once the installation is done you just have to create a client-side file in which we will run your first menuu

<a name="create-menu"></a>
### Create a menu

To create your menu we will use the [RMenu](/docs/{{version}}/rmenu) utility provided with RageUI, if you want to understand how it works I invite you to check by yourself on the documentation.

    RMenu.Add('showcase', 'main', RageUI.CreateMenu("RageUI", "showcase"))
    
You have just created your first menu, this one and instantiate it in a distance table that can be called in any client-side file.

<a name="keys-managing"></a>
### Managing the opening of the menu

Now with a new feature in RageUI you can now manage opening and closing in Menu while having the possibility to change the key in your game settings.

For this we will use [Keys](/docs/{{version}}/keys)

    Keys.Register('E', 'E', 'Open RageUI Showcase menu default.', function()
        RageUI.Visible(RMenu:Get('showcase', 'main'), not RageUI.Visible(RMenu:Get('showcase', 'main')))
    end)

Pressing the E key will open or close your menu.

<a name="display"></a>
### Menu displaying Tick

Let's now move on to the display of your menu content

In the display loop of your menu just use the RageUI.IsVisible function, here is a quick example.

        RageUI.IsVisible(RMenu:Get('showcase', 'main'), function()
                RageUI.Item.Button('RageUI Button', nil, {  }, true, {
                    onHovered = function()

                    end,
                    onSelected = function()

                    end,
                    onActive = function()

                    end,
                })
        end)

Once this is done if you press the E key you will see the menu you have just created displayed with a [basic button.](/docs/{{version}}/item-button)
 
<a name="result"></a>
### The result you must have obtained

Here is the final result you must have obtained in your client-side file

        RMenu.Add('showcase', 'main', RageUI.CreateMenu("RageUI", "showcase"))
        
        Keys.Register('E', 'E', 'Open RageUI Showcase menu default.', function()
            RageUI.Visible(RMenu:Get('showcase', 'main'), not RageUI.Visible(RMenu:Get('showcase', 'main')))
        end)
        
        Citizen.CreateThread(function()
            while (true) do
                Citizen.Wait(1.0)
                RageUI.IsVisible(RMenu:Get('showcase', 'main'), function()
                    RageUI.Item.Button('Basic Items', nil, {  }, true, {
                        onHovered = function()
        
                        end,
                        onSelected = function()
        
                        end,
                        onActive = function()
        
                        end,
                    })
                end)
            end
        end)
        
Congratulations you know about creating menus with this library, now you just have to read about the different features of this library. Have fun and don't hesitate to support the library via the sponsor button.
