---
lang:   EN
title:  All together now
answer: ^4$
ok:     Yes, Shakespeare wrote 4 plays in 1591
error:  Answer for the year 1591 should be 4
load:   prev
---

I have prepared the __count\_plays__ method for you. See if you can find out how many plays
were written by Shakespeare in the year __1591__. Try this:

    def count_plays(year)
      s = get_shakey
      
      s["William Shakespeare"]
        .select { |k, v|
          v["finished"] == year
        }.each { |key, val|
          puts val["title"]
        }.count
    end
    
    puts count_plays(0)

Did you notice that I chained the count method at the end of the each method? This gives
us a return value for the __count\_plays__ method.
