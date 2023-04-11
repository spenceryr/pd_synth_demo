# PD Synth Demo
This is a Pure Data patch to demonstrate a very simple wavetable synthesizer with 4 voices created using additive synthesis.

To run my patch, open the file called **OPEN_ME.pd**. You can play from a midi keyboard or you can press the "play"
button to play from my qlist. Make sure the volume of the output object is high enough to hear.

If the patch doesn't work or if something gets messed up, press the "grand reset" button. You are able to change each
waveform by drawing on it, or if you go into the subpatch, you can send a "sinesum" message to the wavesynth objects. 

In order to do a polyphonic synth, I had to make the wavesynth subpatches seperate and they had to use the same
wavetable and parameters. The only parameter that is variable (i.e. has $0) is the carrier frequency because each
note being played polyphonically can be a different frequency.

As for the drums, you can either use the pre-loaded sounds, load sounds in from the extras I included, or load
your own. You can in theory use any sound, but it is meant to act as both a drum machine and sample player, so
drum hits are recommended. You can play the samples loaded in by pressing the "play" buttons on the right of the
rows, and you can also send midi notes 48, 49, 50, and 51 which corresponds to each sample.

As for the effects racks, the drum machine/sampler and the synth voice have their own effects rack, and each effect
can be turned on/off and modulated. The delay effect and the flanger can be turned on/off using the delay/flanger
level sliders (putting them at the bottom is all the way off). You can turn on autopanning and change the
speed/direction it goes by messing with the number box. The Spacial slider sends the audio forwards and backwards in
space.
