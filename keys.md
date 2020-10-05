# Keys

- Keys
    - [Descriptions](#descriptions)
    - [Example](#example)
    
<a name="descriptions"></a>
### Descriptions

The Keys utility allows you to manage the key you press to open or close your menus, you can of course use it for anything other than opening or closing menus.

<a name="example"></a>
### Example

Here is an example of how to create in listener to perform the action you want when the user presses the key you have chosen.

    Keys.Register('E', 'E', 'Description available in the key pause menu.', function()
       --- Perform your actions
    end)
