﻿# Date.IsInPreviousNWeeks
Indicates whether this date occurs during the previous number of weeks, as determined by the current date and time on the system.
***
function (optional dateTime as nullable any, weeks as number) as nullable any
***
# Descrition 
Indicates whether the given datetime value <code>dateTime</code> occurs during the previous number of weeks, as determined by the current date and time on the system.
      <ul>
      <li><code>dateTime</code>: A <code>date</code>, <code>datetime</code>, or <code>datetimezone</code> value to be evaluated.</li>
      <li><code>weeks</code>: The number of weeks.</li>
      </ul>
# Category 
Date
# Examples 
Determine if the week before the current system time is in the previous two weeks.
```
Date.IsInPreviousNWeeks(Date.AddDays(DateTime.FixedLocalNow(), -7), 2)
```
> true
***