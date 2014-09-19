#!/bin/bash

sleep 12
wmctrl -n 3
wmctrl -s 0

gnome-terminal --tab-with-profile=Main --title="Main Terminal" &
gnome-terminal --tab-with-profile=Haskell --title="Haskell Terminal" &
gnome-terminal --tab-with-profile=Blink --title="Blink Terminal" &
sleep 2

wmctrl -r "Haskell Terminal" -t 1
wmctrl -r "Blink Terminal" -t 2
sleep 1

sublime -a --project "~/code/Maxifill/web-animations-next/web-animations-next.sublime-project" &
sleep 3
sublime -a -n --project "~/code/JSTypeInference/JSTypeInference/Code_JSTypeInference.sublime-project" &
sleep 3
wmctrl -r :ACTIVE: -t 1
sleep 2

google-chrome &

