# Remote-Scopie
Remote control a telescope, cameras and accessories via a Raspberry Pi based web server.

26/2/2015 -
Initial goals:


Phone / tablet / pc web interface -

Simple web interface (framework=?) served from nodejs/iojs server hosted on Raspberry Pi. Web interface initial requirements to control RA, Dec movement and set tracking speed.


Raspberry Pi nodejs/iojs server -

Uses Gertbot motor controller module that plugs into Pi GPIO port. Connects via node-serial to Gertbot API to control/monitor RA stepper motor, Dec stepper motor and end stop detectors.


Hardware -

Development will be carried out on my second hand Meade LX90 where I intend to strip out the old (and annoyingly flakey) control, motor and gearbox system. 3d printed adaptors will be used to mount Nema-17 sized stepper motors then coupled to last gear step shaft of RA and Dec drives. 3d printed adaptors also used to mount Pi inside the fork covers.


Enhanced goals:

1. Improve web interface responsivenss using websockets.
2. Connect DSLR camera to Pi and control/process via web interface. Feedback live view via websockets? Use gphoto2 and node-gphoto2 node module, processing and processing node module.
3. Enhance control/monitoring ability eg. dome, battery monitore, etc.
4. Connect Webcam to Pi and control/process via web interface.
5. Enhance scope control. Align scope to allow slewing to specified co-ords, possibly supplied by 3rd party app.
6. Plan is to develop software so any telescope can be controlled with suitable API config information.
