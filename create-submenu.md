# Create SubMenu

- Create SubMenu
    - [Create a menu](#create-submenu)
    - [Settings available](/docs/{{version}}/menu-settings)
    
<a name="create-submenu"></a>
### Create a SubMenu

To create your menu we will use the [RMenu](/docs/{{version}}/rmenu) utility provided with RageUI, if you want to understand how it works I invite you to check by yourself on the documentation.

    RMenu.Add('showcase', 'submenu', RageUI.CreateSubMenu(RMenu:Get('showcase', 'main'), "RageUI", "showcase"))
