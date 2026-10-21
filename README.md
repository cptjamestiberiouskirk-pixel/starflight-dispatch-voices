# Starflight Dispatch Voices

Voice recordings for the dialog of Starflight Dispatch, my remake of the 1986 space RPG Starflight. The game loads each recording from here when a line is spoken, so the game itself stays small.

## Layout

- `aliens/<id>.mp3`: one recording per line of the original game's alien comm table (and the player's own side of the talk), named by the line's id. The words are the original game's, and every race speaks with a voice of its own.

- `crew/<hash>.mp3`: the crew's banter on the bridge, one recording per line, named by the FNV-1a 32-bit hash of the line's exact text (8 lowercase hex digits), so the game finds each recording from the words it shows.

Lines that name the player's captain or ship are recorded with a neutral word in place of the name, since the game shows the name the player chose on screen.

## Format

MP3, mono, 44.1 kHz, 128 kbps.
