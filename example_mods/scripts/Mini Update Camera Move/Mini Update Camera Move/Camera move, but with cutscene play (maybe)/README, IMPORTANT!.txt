Hey, I'm not sure if this works because my pc is 32-bit and it doesn't allow me to see cutscenes, 
     please, I would appreciate if you would inform me of any error in this script.

Before putting the script, make sure your cutscene is in mods / videos and is in .mp4 format. after achieving this. 
        open the script, go below, and you should see something like this:

local allowCountdown = false
function onStartCountdown()
	if not allowCountdown and isStoryMode and not seenCutscene then --Block the first countdown
		setProperty('inCutscene', true);
		startVideo('put your .mp4 cutscene name here');
		allowCountdown = true;
		return Function_Stop;
	end
	return Function_Continue;
end   

In "put your .mp4 cutscene name here" you must put the name of your custcene. something like this:


                startVideo('verybadvideotutorial');

do not remove the quotes, they are part of the code.
