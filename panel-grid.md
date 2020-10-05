# Item Grid

- Item Grid
    - [Example](#example)

<a name="example"></a>
### Example
    
     RageUI.Panel.Grid(0.5, 0.2, 'TopText', 'BottomText', 'LeftText', 'RightText', {
                    onPositionChange = function(X, Y)
                        print(X, Y)
                    end,
                    onSelected = function(X, Y)
                        print(X, Y)
                    end
                }, 1)
