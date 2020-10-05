# Panel Percentage

- Panel Percentage
    - [Example](#example)

<a name="example"></a>
### Example
    
     RageUI.Panel.PercentagePanel(1.0, "HeaderText", "MinText", "MaxText", {
                     onPercentageChange = function(Percentage)
                         print(Percentage)
                     end,
                     onSelected = function(Percentage)
                         print(Percentage)
                     end
                 }, 1)
