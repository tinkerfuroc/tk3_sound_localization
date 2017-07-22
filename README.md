# tk3_sound_localization
using Tamago-03 and hark
## Usage:
-  1.Install hark environment according to http://www.hark.jp/wiki.cgi?page=HARK+Installation+Instructions
-  2.Run 'hark_designer' in terminal and load tk3_sound_localization.n
-  3.Double-click 'LocalizeMUSIC' module under 'sub_localization' subnet and replace the path of A_MATRIX with that of your 'tamago_rectf.zip'
-  4.Plug in Tamago-03, run 'arecord -l' to list ALSA devices and found the ID of Tamago-03, such as 'Card N', and double-click 'AudioStreamFromMic' module under 'MAIN_LOOP' tab, then set DEVICE to 'plughw:N,0'
-  5.Click 'Execute' to run(autosave) or 'Save', and then you can exit browser and run ./tk3_sound_localization.n directly from terminal
-  6.In case the performance is suboptimal, adjust the parameters of modules under 'sub_localization' subnet
