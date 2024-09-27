---
lang:   EN
title:  Give and take
answer: \d+
ok:     Right on. Bravo.
error:
---

Most methods do not only want some parameters as input, but will also __give something back__.
I have changed our method a bit so it will return a value to you. Try it:

    def tame( number_of_shrews )
      number_of_shrews.times {
        puts "Tamed a shrew"
      }
      return number_of_shrews
    end

    puts tame(3)
