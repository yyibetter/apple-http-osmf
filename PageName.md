# Introduction #

Welcome to the apple-http-osmf project.  The goal of this project is implement the Apple HTTP Live Streaming (HLS) protocol using the OSMF based flash player.  Currently the handling of mpeg2 transport stream files is handled, basic support for both VOD and Live streaming is complete.

We don't have a mailing list setup yet, so please just use the ISSUES section of google code until we do.

## ToDo ##
  * Live streaming:
    * Buffer management / chunk pre-fetching
    * Adaptive switching algorithm refinement
    * Properly reporting current position and duration in mediaplayer object to allow for:
      * live seeking
      * pause (with forced play when HLS lookback buffer is exceeded)
    * Updated logic to only retrieve the manifest for the quality levels requested
  * General:
    * Support for pantos AES encryption (chunk descrambling)