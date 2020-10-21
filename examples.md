Please note: Tha data your function will get will look like an array of strings as defined in your language. No additional parsing is needed! The form ['', ''] is just a convention! <br>
**Please make sure your solution runs correctly with these test cases!** <br>


### Test Data
**intervalConstruction**<br>
|Input|Output|
|---|---|
|['M2', 'C', 'asc']|D|
|['P5', 'B', 'asc']|F#|
|['m2', 'Bb', 'dsc']|A|
|['M3', 'Cb', 'dsc']|Ab|
|['P4', 'G#', 'dsc']|D#|
|['m3', 'B', 'dsc']|G#|
|['m2', 'Fb', 'asc']|Gbb|
|['M2', 'E#', 'dsc']|D#|
|['P4', 'E', 'dsc']|B|
|['m2', 'D#', 'asc']|E|
|['M7', 'G', 'asc']|F#|

**intervalIdentification** <br>
|Input|Output|
|---|---|
|['C', 'D']|M2|
|['B', 'F#', 'asc']|P5|
|['Fb', 'Gbb']|m2|
|['G', 'F#', 'asc']|M7|
|['Bb', 'A', 'dsc']|m2|
|['Cb', 'Abb', 'dsc']|error|
|['G#', 'D#', 'dsc']|P4|
|['E', 'B', 'dsc']|P4|
|['E#', 'D#', 'dsc']|M2|
|['B', 'G#', 'dsc']|m3|
