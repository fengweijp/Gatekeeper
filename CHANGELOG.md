# Change Log

## Current Version

v2.2.0

- Minor refactor
- MessageReceivedEventArgs now includes the type of message (Text, Binary)

## Previous Versions

v2.1.7

- Minor fixes
- SendAsync using string
- Statistics object for both client and server

v2.1.6

- Cosmetic fix in logger output

v2.1.5

- Fix for ClientConnected event placement (thank you @AK5nowman!)

v2.1.4

- Added generic HTTP handler that can be overridden for non-websocket requests (thanks @Data33!)

v2.1.3

- Fix typo in ClientDisconnectedEventArgs class name (thank you @caozero and @Danatobob)

v2.1.2

- Fix ClientConnectedEventArgs.HttpRequest issue (thank you @Danatobob)

v2.1.1

- Fix for ```IPAddress.Any``` server constructor use case

v2.1.0

- BREAKING CHANGES
- Migrated from Func-based callbacks to Event
- Fix for using hostnames in server constructor (thank you @Danatobob); WatsonWebsocket will now bind to the first address returned in hostname resolution
- Overrideable method for logging ```void Logger(string msg)``` and ```Action<string> Logger```
- Code refactor and cleanup
- ```IpPort``` is now a ```ClientMetadata``` property rather than a method

v2.0.2

- Fixed connection bug (thank you @wirmachenbunt)

v2.0.1

- XML documentation

v2.0.0

- Breaking changes!  Task-based callbacks, simplified constructors, and ```.Start()``` methods for both client and server
- Bugfixes and improvements around callbacks and SSL
 
v1.3.x

- Big thanks to @FodderMK for his time and contributions to WatsonWebsocket!
- Breaking change, ```ClientConnected``` now returns entire HttpListenerRequest
- Simplifications to test programs for both client and server
- More appropriate status codes for various scenarios including non-websocket requests and denied requests

v1.2.x

- Return value from ```ClientConnected``` now acts as permit/deny for the connection - thank you @FodderMK!
- Bugfixes to client disconnect handling - thank you @FodderMK!
- Integrated pull requests from @FodderMK (thank you!) for fixes and GetAwaiter() 
- Retarget to support both .NET Core 2.0 and .NET Framework 4.5.2
- Enhancements and fixes, new constructor using Uri (thank you @BryanCrotaz!)
- Bugfixes, client kill API (thank you @BryanCrotaz!)

v1.1.x

- threading fixes, code cleanup, client connected signature change (thank you @BryanCrotaz!)
- Remove unnecessary framing

v1.0.x 

- initial release, bugfixes
