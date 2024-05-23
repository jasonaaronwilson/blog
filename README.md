#  404: Idea Not Found

Thoughts about technology (especially
software development and AI -- assuming there is a difference
anymore).

> 2024-05-23 - lazygit
> 
```
I've only recently started using lazygit. Since
I'm an emacs user, you'd think I'd just use magit
however the Emacs team has gotten out of sync with
old-school folks and I don't want to spend much
time messing around with stuff like this.

I'm listed on several patents 

                              * Original Appearance *
                              -----------------------

┌─[2]─Files──────────Worktrees───────────Submodules─┐
│                                                   │
│ ▼src                                              │
│ M lexer.c                                         │
│                                                   │
│                                                   │
│                                                   │
│                                                   │
│                                               ALL │    <-- this is what's "new" just a button.
└───────────────────────────────────────────────────┘        not sure what the UI should look like
                                                             and of course a better name is possible
                                                             (browse?, search?, ...)


                                   * All Files View *
                                   ------------------


┌─[2]─Files──────────Worktrees───────────Submodules─┐
│                                                   │
│ ▼src                                              │|
│ M lexer.c                                         │|   <-- standard lazygit scroll-bars
│   _clang-format                                   │
│   compiler-errors.c                               │
│   debug-printer.c                                 │
├───────────────────────────────────────────────────┤
│ <fuzzy-filter>                              [ x ] │    <- <fuzzy-filter> should be grey
└───────────────────────────────────────────────────┘       like the fzf tool since no filter
                                                            is being used. cancel button can be
                                                            prettier I'm sure or more descriptive

                  * All Files View After Filtering  *
                  -----------------------------------

┌─[2]─Files──────────Worktrees───────────Submodules─┐
│                                                   │
│ ▼src                                              │
│ M lexer.c                                         │    <-- no scroll-bars because only
│   debug-printer.c                                 │        one file matches
│                                                   │
│                                                   │
├───────────────────────────────────────────────────┤
│ d                                           [ x ] │    <-- the d should not be in grey like
└───────────────────────────────────────────────────┘        the <fuzzy-filter> prompt

At this point, clicking on debug-printer.c file
would display the full file in the "Staged
Changes" window.

More importantly, things like "e" and "b" (which
both Gemini and ChatGPT4o think exist but I can't
find a blame command when I press "b"), would do
useful work on those files. Using normaly google
search, I did find some possible integrations with
"tig" which quite frankly has a very similar
feature set to lazygit though I'm pretty sure
lazygit is easier to pick up but I'll give tig a
try soon. (Of course I already kicked the tires,
and it seems less approachable than lazygit and at
least initially kind of boring unless you love
walls of text you could get by doing git log...")
```

-----

Copyright © 2024 Jason A. Wilson. All Rights Reserved.
