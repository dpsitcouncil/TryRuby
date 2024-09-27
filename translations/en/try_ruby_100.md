---
lang:   EN
title:  Stop, You're Barking Mad!
answer: ^\d{1,}$
ok:     Only strings can be reversed
error:  
---

You can't reverse the number 40. Ruby has tossed an error message. Ruby is telling you there is no method reverse for numbers.

Maybe if you turn the number into a string first:

    40.to_s.reverse
