# doc_comp_sway_rpi4
How to make sway runs ok in rpi4 with two monitors

Why?
Wayland is not only the future but actually fills better. By example, firefox in wayland with gpu accel is by large faster than in X.

Anyway, I love sway!
sway runs amazing in low resources machines. Since I use Raspberry Pi 4 as my main desktop computer I decided to use sway as my DM (sway is not a DM!)
But, there is a bug, maybe a lwroots bug or a kernel bug (probably the last), that prevent me to run sway with two monitors in the rpi4 (https://github.com/swaywm/wlroots/issues/1943#issue-531838199). But FSM be praised, https://github.com/schauveau has develop a patch to workaround the bug (https://github.com/swaywm/wlroots/issues/1943#issuecomment-660498155)

So, I downloaded sway from github (https://github.com/swaywm/sway.git) and then make subprojects/wlroots subdir. Now I go to this directory and got wlroots (https://github.com/swaywm/wlroots.git). Then I dowloaded and applied the patch. Then I go back to sway directory, compiled and installed it. 

Now, I'm able to run sway. TADA! :-)
