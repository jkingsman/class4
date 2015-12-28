# classIV

Passive network reconnaissance of 802.11 'probe' packets for wireless breadcrumb analysis. Listen in to all the lonely 802.11 devices calling for mama around you, and watch for authentication packets - where have these devices been, and have they been here before? ClassIV can help; read below to learn more.

## Using classIV

You can't. I haven't written it yet. It's probably gonna be in python, though.

Ooooooh or maybe Clojure. Clojure is cool; maybe I should learn that and build this in it..

\**googles clojure packet capture**

Yeah so it'll be in python.

## What are 802.11 probe packets?

They're just these packets, ya know?

802.11 has a number of management frame types which build out the support structure for wireless connections, including clients advertising their presence to access points and vice versa, authentication/deauthentication, and so forth.

Devices searching for a WLAN can use active or passive search mode. Passive mode is usually less common, and consists of the client waiting to hear a broadcast frame from a suitable access point, at which point it will initiate connection.

Active mode, which is more common and efficient, consists of the client sending out requests on each channel for what networks are available. What classIV listens for are *directed probe requests*, where the client has a specifc SSID that they're looking for, meaning the client only gets a response if there's an SSID they've seen before.

By listening for these directed probes, classIV can see where various wireless clients have connected in the past. What you do with that info in terms of forensics is up to you ¯\\_(ツ)_/¯ 

## Celebrity Endorsements

*"Sometimes you got to go back... to actually move forward [...] going back to see where you came from, where you've been, how you got here and see where you’re going." --Matthew McConaughey*

*"My girl, my girl, don't lie to me/Tell me where did you [get wifi] last night" --Kurt Cobain, more or less*
