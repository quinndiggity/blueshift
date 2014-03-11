Request for contribution:

	If anyone have a monitor with backlight
	supported by xbacklight. src/blueshift_randr_c.c
	needs to be extended to be able to read and set
	backlight settings. src/blueshift_idcrtc.c can
	be used as a starting point of the implementation.



Blueshift adjusts the colour temperature of your
monitor according to brightness outside to reduce
eye strain and make it easier to fall asleep when
going to bed. It can also be used to increase the
colour temperature and make the monitor bluer,
this helps you focus on your work.

Blueshift is inspired by Redshift but is vastly
more flexible and solves some problems with Redshift:

    - Decreases the colour temperature too early
      during the winter which can make you tired
      during daytime.

    - Limited support for settings such as
      brightness and contrast. Technologies like
      Blueshift and Redshift needs to remove all
      settings made by other programs, to be
      portable and to have get accuracy, which
      means that you cannot any use other program
      at the same time. Redshift supports only
      gamman and a limited brightness range.
      Blueshift can be extended by the user to
      do anything and have built in support for
      unlimited brightness, contrast, gamma
      correction and S-curve correction.
      Brightness and contrast are normally not
      important because you should configure
      that on the monitors control panel. But
      one may want to temporarly so a change
      to contrast to increase the brightness
      beyond 100 %. Blueshift is to might
      knowledge the first program to support
      S-curve correction which is important
      for LCD monitors which suffers the effects
      of S-curves.

    - No support of ICC profiles.

Blueshift is not user friendly and it is not
meant too be. Blueshift does offer limited
use of command line options to apply settings,
but it is really meant for you to have configuration
files (written in Python 3) where all the policies
are implemented, Blueshift is only meant to provide
the mechanism for modifying the colour curves.
Blueshift neither provides any means of automatically
getting your geographical position; the intention is
that you should implement that in the policy yourself
using library which can do that. Additionally
Blueshift provides not safe guards from making your
screen unreadable or otherwise miscoloured; and
Blueshift will never, officially, add support
specifically for any proprietary operating system.
Blueshift is fully extensible so it is possible to
make extensions that make it usable under unsupported
systems, the base code is written in Python 3 without
calls to any system dependent functions.
If Blueshift does not work for you for any of these
reasons, you should take a look at Redshift.
