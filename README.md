# osrm_profiles_india

Primary goal : To adapt OSRM's driving / walking / other profiles to Indian road routing.

This repo has the `profiles/`folder originally copied from https://github.com/Project-OSRM/osrm-backend/tree/master/profiles

Won't host any of the actual OSRM program here; just the profiles so that this repo stays open to collaboration, PRs etc without affecting the program side.

Note: Keep the original .lua's same as they are in official osrm-backend repo ; clone to new .lua files and edit those.


First thing to do: left-side driving

car-modified.lua:
```
function setup()
...
function setup()
  return {
    properties = {
    ...
      left_hand_driving              = true,
    },
```

There's lots more to customize here : driving speeds for various conditions, turn delays etc.

