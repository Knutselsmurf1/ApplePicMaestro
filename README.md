# ApplePicMaestro
Purpose:
1. Group only the pictures/movies taken by iPhone
2. Group only the pictures/movies imported by iPhone for example by USB cable
3. Group other pictures/movies, for example iPhone most assumable has collected from WhatsApp
4. Give all pictures/movies as prefix the date/time stamp in which the pictures/movies are taken
   However in case EFIX date does not exist, then date/time stamp in which the pictures/movies are last modified
5. Correct as far as possible wrong suspicious date/time stamp for .mov files, depending on the EFIX time of last valid picture
   Unfortunately meta data (basically not EFIX) of .mov files basically does not contain a (valid) taken date.
   Also the last modified date/time of file itself (and which for example also Windows Photos uses to sort movies) could
   be invalid especially if directly copying from https://www.icloud.com/photos/.

   Note that movies on the iPhone itself and on https://www.icloud.com/photos/ are ordered correctly.
   The issue occurs in copying files from iPhone to PC. For pictures taken by the iPhone it is no issue even in case
   the file date/time might change, since by design the EFIX date remains correct.

How to use:
-Copy(part of) pictures from iCloud Photos to c:\copyOfiCloudPhotos
- ApplePicMaestro.exe < path with pictures>
  Its output is in subfolders:
  - \output(see 1)
  - \anotherbrand(see 2)
  - \unknown(see 3)
