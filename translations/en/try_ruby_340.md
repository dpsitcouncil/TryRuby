---
lang:   EN
title:  In Ruby, Def Leppard means: define method Leppard
answer: ^tame
ok:     Tame is not lame
error:  
---

Hey, okay, you done it. You're making your own method. You started with def, followed by the name of the method. And a list of arguments which the method will need.

Here's the code:
    
    def tame( number_of_shrews )
      number_of_shrews.times {
        puts "Tamed a shrew"
      }
    end
