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
Ok, so you can record sounds over the entire audio spectrum. Now, how do they sound with respect to each other? Do bass sounds recorded at the same volume (or Sound Pressure Level) as treble sounds look to have the same level as each other on the decibel scale? What does that even mean? Welcome to frequency response. 

Lets define something first.

SPL or 'Sound Pressure Level' is the root-mean-square pressure of the sound wave compared to (divided by) the ambient room pressure, and then translated into the decibel scale. 
`SPL = 20*log(Prms/Po)`

Ideally, if a microphone is used to record a tone sweeping linearly from 20Hz-20kHz at 1 Sound Pressure Level will have the same value (pressure in dB) across the entire frequency spectrum. This is a 'flat' frequency response. A frequency response that has a portion, say 10kHz-15kHz which has a higher gain (ie. part of the response is higher than the rest), will create the effect of an increased volume for only that part of the spectrum. In that case, you might hear bells and high string instruments really well. Since our goal is to accurately represent the true sound, this result is undesirable.

#### Takeaway: 
When looking for a microphone, try to find one with a flat frequency response. (This can be found in the datasheet)


### DIRECTIVITY PATTERNS

### SENSITIVITY

### NOISE FLOOR
