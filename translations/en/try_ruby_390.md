---
lang:   EN
title:  Noble Kinsmen
answer: ^The Two Noble Kinsmen$
ok:     That's much better
error:  
load:   prev
---

If you inspect the list of plays carefully you will see that it has a kind of nested
structure. (This is actually quite common in data you get from the internet.)
Looks like this:

<ul>
  <li>"William Shakespeare"
  <ul>
      <li>"1"
      <ul>
        <li>"title": "The Two Gentlemen of Verona"</li>
        <li>"finished": 1591</li>
      </ul>
      </li>
      <li>"2"
      <ul>
        <li>"title": "The Taming of the Shrew"</li>
        <li>"finished": 1591</li>
      </ul>
      </li>
      <li>...</li>
  </ul>
  </li>
</ul>

To list the plays we first have to access the top "William Shakespeare" hash element by its name.
Next we have to __iterate__ through each element below it.

Ruby has a method for iterating. It is called __each__. We have seen it before when
creating our book rating system.

Everything that method __each__ returns is passed to a block:

    s = get_shakey
    
    s["William Shakespeare"].each { |key, val|
      puts val["title"]
    }
