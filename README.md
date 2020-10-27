#  SassChallenge
https://deroodirk.github.io/SassChallenge/.

## first solution 
i used the files from the exercises (same names and stuff)

## Another solution 
use base 
add 2 extra classes to the things you want to change 
example with 1 colorchange (imagen yourself doing same but with classes red and blue )

example
base.scss file 

$font-stack:    Helvetica, sans-serif;
$primary-color: #333;

body {
  font: 100% $font-stack;
  color: $primary-color;
}

styles.scss file 

@use 'base';  

.inverse {
  background-color: base.$primary-color;
  color: white;
}

compiles in 
body {
  font: 100% Helvetica, sans-serif;
  color: #333;
}

.inverse {
  background-color: #333;
  color: white;
}
