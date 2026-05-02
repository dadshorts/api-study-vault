# API Types — In My Own Words
Date: 2026-05-02
Source: Phase 0 Chunk 2 conversation with Claude

## REST
Text messages back and forth, mostly for simple requests. You get the whole menu sent back, not just pizza options.

## GraphQL
Text message, but the power is asking for specific pieces of data — like "I just want specialty pizza options for vegetarians." Good for many clients accessing the same resources.

## gRPC
Smart as hell. Binary code for computer-to-computer talk. Smaller format, lightning fast. (Used service-to-service inside one company, not on the public internet.)

## WebSocket
Phone call vs. text message. Good for when the server needs to push data unprompted. Online video games — player does X and the server pushes a new map or mission onto the map.

## SOAP
Run. Old, extremely structured. Used in legacy enterprises — banking, healthcare, gov, etc.

## Webhooks
The nightwatchman who calls you when something happens — instead of you calling every 5 minutes to see if everything is good. (The "every 5 min" approach has a name: **polling**.)
