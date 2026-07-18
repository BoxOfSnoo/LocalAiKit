Create a single-page HTML racing management game with these features:

**Track & Visuals:**
- Closed circuit track with some straight but mostly curved sections (not oval). Curves affect speed according to sharpness.
- Show entire track on screen.
- Start/finish line marked at track start
- A pit lane branches off to the side of the track and rejoins after a short distance
- 10 racers (player + 9 AI) rendered as mini race car shapes with distinct colors
- Include a minimap that all car positions. Highlight the player's car so it's easy to see

**Gameplay:**
- Multiple-lap race, tires degrade to 0 over 80% of total race distance (same rate for all racers)
- Include button to trigger race start, boost and pit stop request
- Pit stop required: when player requests a pit stop, car drives to pit lane entry then to a pit box for 4-second tire change, then rejoins the track.
- Speed while in the pit lane is restricted to 20% of maximum race speed.
- Boost: hold SPACE for 1.6x speed burst (~3 seconds), recharges at 12%/s when released
- Boost wears tires 15% faster.
- Gap shows distance to car ahead
- AI drivers manage their own tire strategy, boost, and pit stops automatically

**UI:**
- Sidebar with race info and control buttons
- Data grid showing position, driver name, speed, lap, gap, tire %, boost % for all racers
- Finish screen with results table (position, time, best lap, pit stops)

Save the file as racing{model}.html where {model} is a simplified unique name indicating the model used to generate the game.