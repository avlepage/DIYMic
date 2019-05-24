# Microphone Attributes

What makes sound sound the way it does? What makes a microphone a good microphone? There are several attributes of a microphone which must be taken into account in order to accurately represent sound as it is heard in real life. These include: 
>- Frequency Range
>- Frequency Response
>- Directivity Patterns
>- Sensitivity
>- Noise Floor

### FREQUENCY RANGE
The frequency range of the (very sensitive) human ear is 20Hz-20kHz. This range has 5 sub-bands, categorized according to their characteristics. Most of this spectrum is essential in order to accurately represent sounds as they exist in real life. It's possible to hand-wave a bit below 50Hz and above 16kHz, but generally it should be aimed to capture every part of this spectrum.

#### 20-30Hz
Have you ever sat in a church with a huge pipe organ and felt your chest vibrate with the lowest notes? That's this band. If you haven't, that's okay. The best explanation of this range is that these tones are felt as much as they are heard, and can be difficult to reproduce on a loudspeaker. 

#### 30-500Hz
This band is attributed to the lower- and upper-bass pitches if we're speaking musically. This is below the typical human speaking range, but makes a music sound.. fuller.

#### 500Hz-3kHz
Are you a typical human? Then your voice likely makes most of its noises in this range. This is referred to as the midrange, because humans like to define things with respect to themselves. 

#### 3kHz-8kHz
The 3-8kHz range is known as the presence range. This is because while you can hear a human voice in the previous range, you wouldn't be able to hear all of the s and saliva sounds which occur in this band. Adding this range to the previous bands would give you a sense of, well, presence. 

#### 8kHz-16kHz
This range is associated with very high pitched sounds. The bells or the triangle would have sounds occurring in this band, making it still an essential part of music. 

#### 16kHz-20kHz
Unless you have significant hearing loss, your hearing probably cuts off somewhere in this spectrum. Very few people can hear up to 20kHz (mainly just children). If you're testing your hearing range, and hear sounds fading in this spectrum, don't turn up the volume. Accept your limitations.

### FREQUENCY RESPONSE
Ok, so you can record sounds over the entire audio spectrum. Now, how do they sound with respect to each other? Do bass sounds recorded at the same volume (or Sound Pressure Level) as treble sounds sound like they're the same volume when played back? What does that even mean? Welcome to frequency response. 

Lets define something first.

SPL or 'Sound Pressure Level' is the root-mean-square pressure of the sound wave compared to (divided by) the ambient room pressure, and then translated into the decibel scale. 
`SPL = 20*log(Prms/Po)`

Ideally, if a microphone is used to record a tone sweeping linearly from 20Hz-20kHz at 1 Sound Pressure Level, it will have the same value (pressure in dB) across the entire frequency spectrum. This is a 'flat' frequency response. A frequency response that has a portion, say 10kHz-15kHz which has a higher gain (ie. part of the response is higher than the rest), will create the effect of an increased volume for only that part of the spectrum. In that case, you might hear bells and high string instruments really well. Since our goal is to accurately represent the true sound, this result is undesirable.

#### Takeaway: 
When looking for a microphone, try to find one with a flat frequency response. (This can be found in the datasheet)

### DIRECTIVITY PATTERNS
If you cover your left ear, in an ideal situation, you will no longer hear sound stimulae from the left-hand side. In a similar manner, some microphones only take input from certain directions. The graph of how strongly a signal at a certain location relative to the microphone will be picked up is called a directivity pattern. Here are a few common ones:

#### Omnidirectional
![Polar Pattern: Omnidirectional](https://github.com/avlepage/DIYMic/blob/master/Microphone%20Attributes/Omni%20Polar%20Pattern.png "Omni Polar Pattern.png")
A microphone with an omnidirectional polar pattern will pick up sounds equally from all directions. In general, these microphones have the most accrate frequency response. They can, however, produce a lot of feedback if the recorded sound can be picked up by the microphone (if it's being played back in the same room). You won't have to wory about this if you play back through headphones, or play back once the recording is finished. To avoid noise, recording with an omnidirectional microphone should be done in a quiet environment. 

#### Cardioid 
![Polar Pattern: Supercardioid](https://github.com/avlepage/DIYMic/blob/master/Microphone%20Attributes/Cardioid%20Polar%20Pattern.png "Cardioid Polar Pattern.png")
Microphones with cardioid polar patterns are usually used on a stage where the amplification of the singer (front) is desirable, and the amplificaiton of the crowd (back) is undesirable. They work in an environment where there is a lot of noise coming from one direction. There are some problematic effects of the cardioid pattern. It results in something called the 'Proximity Effect' when recording is done too close to the microphone, which causes a boost to bass sounds below 200Hz. It is important to be aware of and avoid this when using these microphones. 

#### Supercardioid
![Polar Pattern: Supercardioid](https://github.com/avlepage/DIYMic/blob/master/Microphone%20Attributes/Supercardioid%20Polar.png "Supercardioid Polar Pattern.png")
Supercardioid microphones are used to pick up a single source in a noisy environment. They have a narrower polar pattern than cardioid microphones and have a small section of pickup at the rear of the microphone. Fix the position of this microphone and don't move it while recording!

### SENSITIVITY
The sensitivity of a microphone determines the volume range that a microphone will pick up. You probably want a microphone that can capture high volume sounds without distorting them and low-volume sounds without attenuating them so much that they can't be heard. In general, the minimum sensitivity range that should be used to capture the human voice is 15dB SPL, and the minimum sensitivity of a microphone should be -60 dB so that voices won't be too quiet.


### NOISE FLOOR
Every microphone has a noise floor, and it is likely that there'll be other sources of noise present in a room where sound is being recorded. When recording, the ratio of recorded sound to noise should be at minimum 15dB for recording voices. This can be measured by recording the ambient noise in a room, and then recording speech in the same room, and then comparing the singal strengths on the decibel scale.

