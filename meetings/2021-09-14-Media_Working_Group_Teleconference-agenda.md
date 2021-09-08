### Agenda

This agenda can be viewed and updated on [GitHub](https://github.com/w3c/media-wg/blob/main/meetings/2021-09-14-Media_Working_Group_Teleconference-agenda.md).

If you would like to add an item to the agenda or volunteer to scribe please open a pull request against this agenda.

This time, we have a number of issues related to MSE, and in particular [MSE in Workers](https://github.com/w3c/media-source/issues/175): 

* [w3c/media-source#184 MSE for WebCodecs (comment)](https://github.com/w3c/media-source/issues/184#issuecomment-720771445). See explainer: https://github.com/wolenetz/mse-for-webcodecs/blob/main/explainer.md - wolenetz

  Explainer describes supporting buffering containerless WebCodecs encoded media chunks with MSE for low-latency buffering and seekable playback.

* [w3c/media-source#280 MSE-in-Workers: {Audio,Video,Text}Track{,List} IDL in HTML need additional DedicatedWorker in Exposed](https://github.com/w3c/media-source/issues/280) - wolenetz

  The extended HTML AudioTrack, VideoTrack, TextTrack, and their *TrackList IDLs need updating to have exposure to both Window and DedicatedWorker, not just Window.

* [w3c/media-source#277 MSE-in-Workers: Consider (eventually) transitioning attached element to error upon termination of MediaSource's worker/what should media element do?](https://github.com/w3c/media-source/issues/277) - wolenetz

  Should HTMLMediaElement do any error transition upon the termination of the DedicatedWorkerGlobalScope that owns the attached MediaSource?

* [w3c/media-source#275 Consider relaxing timing of initial HAVE_METADATA transitioning](https://github.com/w3c/media-source/issues/275) - wolenetz

  There is inconsistent behaviour between implementations in the `updateend` event associated with an `appendBuffer()` whose parsing causes a `HAVE_METADATA` state transition.

* [w3c/media-source#281 MSE-in-Workers: Track enable/selection change behavior needs clarity](https://github.com/w3c/media-source/issues/281) - wolenetz

  What to do with selected/enabled track state management if MSE is in a DedicatedWorker, while the HTMLMediaElement remains in Window?

* [w3c/media-source#156 Restore auto-revoking behavior of createObjectURL(MediaSource) to revert breaking change introducing memory leaks](https://github.com/w3c/media-source/issues/156) - wolenetz

* [w3c/media-source#28 Support attachment (and inspection) of MediaSource to HTMLMediaElement via HTMLMediaElement.srcObject](https://github.com/w3c/media-source/issues/28) - wolenetz

### Media Working Group Teleconference - 2021-09-14

| Location | Date & Time |
| -------- | ----------- |
| San Francisco (U.S.A.) | Tuesday, September 14, 2:00 PM PDT |
| Boston (U.S.A.) | Tuesday, September 14, 5:00 PM EDT |
| London (United Kingdom) | Tuesday, September 14, 10:00 PM GMT+1 |
| Paris (France) | Tuesday, September 14, 11:00 PM GMT+2 |
| Tokyo (Japan) | Wednesday, September 15, 6:00 AM GMT+9 |
| Corresponding UTC (GMT) | Tuesday, September 14, 9:00 PM UTC |

### Logistics

Chairs: Jer Noble, Chris Needham

Webex: https://lists.w3.org/Archives/Member/w3c-archive/2020Jan/0323.html

IRC: https://irc.w3.org/?channels=#mediawg

If you are unable to login to view the call details please ask on the IRC before the call.

For assistance go to https://mit.webex.com/mit/mc  and on the left navigation bar, click "Support".
