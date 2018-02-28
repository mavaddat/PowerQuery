﻿# Text.PositionOf
Returns the first position of the value (-1 if not found).
***
function (text as text, substring as text, optional occurrence as nullable any, optional comparer as nullable function) as nullable any
***
# Descrition 
Returns the position of the specified occurrence of the text value <code>substring</code> found in <code>text</code>. 
    An optional parameter <code>occurrence</code> may be used to specify which occurrence position to return (first occurrence by default).
    
      <div>
        <code>comparer</code> is a <code>Comparer</code> which is used to control the comparison. Comparers can be used to provide case insensitive or culture and locale aware comparisons.
      </div>
      <div>
        The following built in comparers are available in the formula language:
      </div>
      <ul>
        <li><code>Comparer.Ordinal</code>: Used to perform an exact ordinal comparison</li>
        <li><code>Comparer.OrdinalIgnoreCase</code>: Used to perform an exact ordinal case-insensitive comparison</li>
        <li> <code>Comparer.FromCulture</code>: Used to perform a culture aware comparison</li>      
      </ul>
# Category 
Text.Membership
# Examples 
Get the position of the first occurrence of "World" in the text "Hello, World! Hello, World!".
```
Text.PositionOf("Hello, World! Hello, World!", "World")
```
> 7
***
Get the position of last occurrence of "World" in "Hello, World! Hello, World!".
```
Text.PositionOf("Hello, World! Hello, World!", "World", Occurrence.Last)
```
> 21
***