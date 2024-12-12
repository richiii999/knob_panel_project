Group Members: Richard Nelson, Ali Siddiqi, Ali Ayash

The only modified code file was the "ui_light_2color.c" file. The changes are summarized as follows:
- The audio header was included
- The switch-case for light level was moved to it's own task
- A task for audio was created similarly to the light task, via a switch-case
- Tasks are created via xTaskCreate, which call the relevant light/audio functions. After setting their respective bits, they self-delete.
- The audio files names are unchanged, so no changes were made to any code files for linking the audio files. The audio files content are of course changed.
