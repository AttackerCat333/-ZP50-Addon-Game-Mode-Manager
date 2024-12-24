[ZP50] Addon: Game Mode Manager:

    - Description:
        This plugin manage your gamemodes with admin vote ready.
    
    - Compatibility:
        - Only works on Zombie Plague 5.0, planned to be worked for Zombie Plague Special in the next updates.
    
    - Credits:
        - Lord. Death. - For the original plugin, Link: https://zppv.boards.net/thread/4987/zp-5-gamemode-vote
    
    - Natives & Forwards:
        - Native 'zp_gamemode_manager_register(modeId, type, chance, allowparticipate, max_participated_players, access_flag)'
        	- modeId: the game mode id.
        	- type: game mode type (Normal, Special)
        	- chance: percentage to be choosen (1 to 100)
        	- allowparticipate: this game mode support participating as specials?
        	- max_participated_players: maxiumum players to be specials for this game mode.
        	- access_flag: the required admin level to start voting by that admin.
        
        - Forward 'zp_fw_gamemode_choose_post(selected_mode)':
        	- selected_mode: selected game mode id.
    
    - Changelog(s)

        - v1.0:
            - Initial Release.
            - Fixed original plugin.
            - Added Countdown in the menu.
            - Random modes can't be started until reaching a number of players.
            - Added Pcvars check.
        
        - v1.0.1:
            - Fixed "RANDOM_MODE_PLAYERS_MIN" doesn't work correctly
        
        - v2.0:
            - Plugin is reworked from scratch.
            - Plugin is using natives "gamemode_manager_register(mode_id, type, chance(or percentage 1 to 100), allowparticipate, max_participated_players, access_flag)".
            - Plugin is using forward "gamemode_manager_choose_post(selected_mode)".
            - Plugin is required include to add it in your favorite mode(s).
            - Added some features from ported gamer club version by Lord. Death.
            - Removed feature (Countdown in menu), i don't know ill restore it or not, let me know guys.
