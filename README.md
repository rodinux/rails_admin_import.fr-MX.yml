
 * A french translation for stephskardal/rails_admin_import (https://github.com/stephskardal/rails_admin_import)
 
I put all my locales I use on my project with Rails. 
The major problem was with the format of the date and of the hours with the code of rails_admin as the datepicker have a bug to translate the hours.
See this issue to understand :https://github.com/sferik/rails_admin/issues/982

I found this solution, I have to keep the default american format for the date 
```
    default: ! '%d/%m/%Y'
```
and added a date format :very_long for my views translated. 
To get the time in datepicker I found this format :
```
long: ! '%d %B %Y %H:%M %p'
```

Also the translation of the date fr.yml, I have to correct some lines from the source I get it to have the good order of the days, I think my sources found a file with the american order where the weeks begin on Sunday and not on Monday in France...

I hope it can be hepfull to someone. 
Have fun.

