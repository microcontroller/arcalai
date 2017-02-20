# arcalai

This Acorn Archimedes machine emulator started off over 10 years ago with
the realization that none of the existing emulators at the time would let
me play my favorite Archimedes games from the 80s and early 90s. Either
the screen modes didn't look right, or they would simply crash in the
attempt.

I set out to fix this, going back to the datasheets to copy the exact
behavior of the relevant system components. By 2007, the chips were
working, though sound was kinda patchy because nobody builds audio
hardware at 1MHz anymore, and the user interface was almost non-existent.

Then came a major life change, and I no longer had the time or energy to
pursue the project. The code just sat there, transferred from one storage
solution to another over the course of nearly a decade.

Now I'm bringing it back! Of course, the audio/video libraries I used back
then have changed over the years, and since this is an ongoing concern I've
decided to make a cleaner interface between the machine-level emulation
code and the front-end audio/video system. You should be able to take the
back-end library, write your own front-end user interface, and glue it all
together by way of callback functions.
