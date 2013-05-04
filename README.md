TOLEQSlider
===========

A `UISlider` subclass that mimics the EQ slider found on Twitter's #music app.

You'll need to bring your own assets for the frame, track and slider thumb, or just use the ones I've created in the sample project - I don't care.

##Interface
Pretty simple interface:

``` lang:objc
/** The value for the left channel eq in the range of 0 to 1.
 
 @warning This value is clipped at 1.
 */
@property (nonatomic, assign) CGFloat leftChannelLevel;

/** The value for the right channel eq in the range of 0 to 1.
 
 @warning This value is clipped at 1.
 */
@property (nonatomic, assign) CGFloat rightChannelLevel;

/** The inactive color for the eq. This is the color that the eq light takes on past the right side of the slider thumb knob.
 */
@property (nonatomic, strong) UIColor *inactiveColor;

/** The active color for the eq when it is available to be lit up. This is the color that the eq light takes on before the slider thumb knob.
 */
@property (nonatomic, strong) UIColor *activeColor;

/** The EQ light glow colors. The number of light sections the light takes on depends on how many colors you pass in here.
 */
@property (nonatomic, copy) NSArray *glowColors;
```

##License
MIT License. Go nuts.

##Homepage
If you're not on github, you can find the page here: https://github.com/larsacus/TOLEQSlider

##Other
Demo project uses [Novocaine](https://github.com/alexbw/novocaine) for audio input. Other than that - have fun.

Yours truly,

_Lars_ ([@theonlylars](http://twitter.com/theonlylars))