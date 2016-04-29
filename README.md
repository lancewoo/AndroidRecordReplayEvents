# AndroidRecordReplayEvents
This is a native event recorder and player on Android devices.
It's a convenience tool for testing.
You have to take the root previlege to run them.

Build it under your Android source code tree, say, in system/core/injectevents.

Transfer both event_record and event_replay to any directory you want, say, in /data.
Make them executable by chmod 777 event_*.
Run ./event_record /data/myevents to record touch or hardware key events. When you want
to finish recording, just press CTRL+C to terminate it.
Run ./event_replay /data/myevents to replay the events. Be aware that you have to start
from the same point to replay the event sequences.

The original code comes from:
http://code.lardcave.net/entries/2009/08/01/160953/
http://code.lardcave.net/entries/2009/08/01/160953/injectevents.tar.gz

