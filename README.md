#  SassChallenge
https://deroodirk.github.io/SassChallenge/.

## first solution 
i used the files from the exercises (same names and stuff)

## Another solution 

use base 

add 2 extra classes to the things you want to change 
example with 1 colorchange (imagen yourself doing same but with classes red and blue )

---example---

base.scss file 

$font-stack:    Helvetica, sans-serif;
$primary-color: #333;

body {
  font: 100% $font-stack;
  color: $primary-color;
}

styles.scss file 

@use 'base';  (use things out of basescss file )

.inverse {
  background-color: base.$primary-color; ( for bg color in file base scss take the primary color
                                          and change it to white in this case )
  color: white;
}

---compiles in---

body {
  font: 100% Helvetica, sans-serif;
  color: #333;
}

.inverse {
  background-color: #333;
  color: white;
}


So the class inverse change the color of the Bg

Do the same but with a class red and and a class blue

