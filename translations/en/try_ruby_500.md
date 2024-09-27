---
lang:   EN
title:  Quickening it Up
answer: ^\d{4}
ok:     Noted
error:  
---

Let's add an __initialize__ method to our class. This method is called whenever a new Blurb<sup>TM</sup>
is created.
At the same time we can limit the length of the Blurb<sup>TM</sup> content to 40 characters.

    class Blurb
      attr_accessor :content, :time, :mood

      def initialize(mood, content="")
        @time    = Time.now
        @content = content[0..39]
        @mood    = mood
      end
    end
    
    Blurb.new(:sick).time

(That parameter __content=""__ is there to make sure that we know content is a string,
even if no content parameter is passed to the initialize method.)
