# Item Horizontal Grid

- Item Horizontal Grid
    - [Example](#example)

<a name="example"></a>
### Example
    
     RageUI.Panel.GridHorizontal(0.1, 'LeftText', 'RightText', {
                     onPositionChange = function(X, Y)
                         print(X, Y)
                     end,
                     onSelected = function(X, Y)
                         print(X, Y)
                     end
                 }, 1)
