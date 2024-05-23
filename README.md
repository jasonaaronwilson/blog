#  404: Idea Not Found

## Thoughts about technology (especially software development and AI -- assuming there is a difference anymore).

<br>
<br>

> 2024-05-23 - ollama
> 
```
AI is moving fast both in both the "proprietary"
commercial space as well as a sligtly more "open"
space (surely fraught with land-mines if you want
to use them for commericial purposes but great for
a learner/hobbyist).

ollama allows you to play around locally with
inference (aka run, not train the models) on your
own computer provided it is beefy enough (RAM is
king for the larger models). It's literally two
copy/pastes from their website to get to a prompt
you can use from the terminal on Linux or MacOS
and it seems like they are getting pretty close to
a click to download for Windows too.

The first use of a new model requires a download
which happens automatically (and models can be
quite large) but ollama can juggle mutiple models
and has a nice library of models though a subset
of what's available on "hugging face" (I guess a
reference to Aliens?).

It's worth noting that Mozilla also offers a
single-file binary that runs Llama 2 on six
different operating systems. While intriguing for
its portability, Ollama currently surpasses it in    <====
terms of model variety and ease of use. As a Linux   <====
enthusiast, I'm keen to explore Mozilla's              
"Cosmopolitan Libc" for future projects, but for       This is how Gemini rewrote my text.
now, Ollama remains my top choice for                    + I'm using github so you can see
experimenting with LLMs independent of the more          + what I wrote first since it's
curated, aligned models offered by commercial            + in the git history...
cloud services (which, for the record, are way
faster than anything a hobbyist could                 <====
realistically run).                                   <====

You don't necessarily need top-of-the-line
hardware to run these models (especially if you're
patient), and it's great that industry giants like
Microsoft, Google, and Meta are releasing smaller
models (many easily accessible through                <==== Another major rewite by Gemini
Ollama). However, be aware that more capable
models often come with stricter licenses. This
isn't surprising, given the massive investments        <== The word massive here is correct
required to train them. Always read the fine print         but *my* original bias was a bit
to understand the terms of use.                            different... It's in git to see.

My favorite model that fits within my CPU RAM (not
VRAM, GPUs are insanely expensive and "gaming" CPU
cards never have enough RAM to run the model you
wish you could run though perhaps still fast
enough - I don't have first hand experience with
those), 

*IS*

   wizard-vicuna-uncensored:30b

Hopefully this will change!

In any event, ollama is super easy to setup and
use.

Upcoming: thoughts on RAG, LORA, etc. and maybe
steps to get a "stable diffusion" type model
running locally (I'm hopeful there is a Docker
file that makes this easy.)
```

<br>
> 2024-05-23 - lazygit
> 
```
I've only recently started using lazygit. Since
I'm an emacs user, you'd think I'd just use magit
however the Emacs team has gotten out of sync with
old-school folks and I don't want to spend much
time messing around with stuff like this.

Here is a feature request to that team for integrating
"fzf" technology right into lazygit.



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
│                                               ALL │    <== this is what's "new" just a button.
└───────────────────────────────────────────────────┘        not sure what the UI should look like
                                                             and of course a better name is possible
                                                             (browse?, search?, ...)


                                   * All Files View *
                                   ------------------


┌─[2]─Files──────────Worktrees───────────Submodules─┐
│                                                   │
│ ▼src                                              │|
│ M lexer.c                                         │|   <== standard lazygit scroll-bars
│   _clang-format                                   │
│   compiler-errors.c                               │
│   debug-printer.c                                 │
├───────────────────────────────────────────────────┤
│ <fuzzy-filter>                              [ x ] │    <== <fuzzy-filter> should be grey
└───────────────────────────────────────────────────┘        like the fzf tool since no filter
                                                             is being used. cancel button can be
                                                             prettier I'm sure or more descriptive

                  * All Files View After Filtering  *
                  -----------------------------------

┌─[2]─Files──────────Worktrees───────────Submodules─┐
│                                                   │
│ ▼src                                              │
│ M lexer.c                                         │    <== no scroll-bars because only
│   debug-printer.c                                 │        one file matches
│                                                   │
│                                                   │
├───────────────────────────────────────────────────┤
│ d                                           [ x ] │    <== the d should not be in grey like
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
