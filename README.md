# elsabot_game_data

This repository holds game data files used for the ElsaBot games.

This environment various must be setup to point to this directory and is used by the elsabot_bt package.

export GAME_DATA_DIR= \<path to elsabot_game_data directory\>

Files:
- **game_settings.json** - general game settings.  Currently used to set the player name.
- **robot_find.json** - used to specify the objects used for the robot find game and their physical room locations.  The locations are saved during game setup. Revise the RobotFindnitAction action of the game behavior tree to specify a different file.
- **robot_seek_1.json** - used to specify the search locations for the robot hide and seek game.  Revise the RobotSeekInitAction action of the game behavior tree to specify a different file. The coordinates are map coordinates.  At each location the robot can be configured to spin around or scan by moving the head from left to right.
