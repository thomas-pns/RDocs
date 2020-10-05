# Item Vertical Grid

- Item Vertical Grid
    - [Example](#example)

<a name="example"></a>
### Example
    
      RageUI.Panel.GridVertical(0.1, 'TopText', 'BottomText', {
                     onPositionChange = function(X, Y)
                         print(X, Y)
                     end,
                     onSelected = function(X, Y)
                         print(X, Y)
                     end
                 }, 1)
