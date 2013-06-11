# C++ expression parsing.
 + Expression parsing in C++ with Dijkstra's
   [Shunting-yard algorithm](http://en.wikipedia.org/wiki/Shunting-yard_algorithm).
 + Original version by
   [Jessee Brown](http://www.daniweb.com/software-development/cpp/code/427500/calculator-using-shunting-yard-algorithm).

## Minimal example.
```C
#include <stdio>
#include "shunting-yard.h"

int main() {
  std::map<std::string, double> vars;
  vars["pi"] = 3.14;
  std::cout << calculator::calculate ("pi+1", vars) << std::endl;
  return 0;
}
```

## More examples.
 + See `test-shunting-yard.cpp` for more conditions.

## Features.
 + Operators: +, -, /, +, <<, >>
 + Map of variable names to be replaced in string.

## TODO
 + Unary operators.
 + Make a PersistentCalculator object to store data
   to make chains of calculations possible.
 + Suggestions from post.