# Versal SoundCloud recording gadget

This Versal gadget intends make it easy for teachers to record themselves and insert audio into Versal lesson. It uses the SoundCloud API to record and store audio, since Versal doesn't have a way to upload audio.

## Installation and running

NOTE: In order to upload sound files, the SoundCloud API requires a user's authentication, and to do this, it needs an extra "callback.html" file to be provided by the application's server (in this case the application is this gadget, so the callback.html file has to live on the versal.com domain). SoundCloud requires that the link to this file be set in the app's settings on the app owner's SoundCloud account, as well as provided by the code that uses the API. Currently, the link to this file is `https://stack.versal.com/api2/gadgets/223244417/workshop-gadget/0.0.2/callback.html`, in the same directory as the rest of the files for this gadget.

The gadget has been uploaded to my personal Versal account and works when dragged in from the sandbox menu.

When the `record` button is pressed, a 10 sec sound clip is recorded then immediately uploaded to the current user's SoundCloud account (after authetication by the user). The Versal SoundCloud gadget can then be used to play the recording just like any other SoundCloud clip. 

The next step is to have the student's version of this recording gadget automatically load a SoundCloud UI to play the recording, rather than requiring an extra widget to play the sound.
