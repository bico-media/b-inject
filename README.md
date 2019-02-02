# Dynamic data from a static blockchain

This repo contains the definition for the protocol B://andlebars (pronounced bandlebars). 

Main message: **Lets get a shared way of indicating that content in one transaction is to be placed within content from another transaction**. 

## High-level description

### v1

_Direct injection_

If you provide content from the blockchain you are compatible with the B://andlebars protocol v1 if

- The text `{{B://[TX]}}` will be replaced with the raw unprocessed content of TX

- The text `{{B://[TX]/}}` will be replaced with the B://andlebar converted content of the TX (nested injections)


#### v1+

_Talking about direct injections_

If you provide content from the blockchain you are compatible with the B://andlebars protocol v1+ if you

- Are compatible with the B://andlebar protocol v1

- The text `{{B:\\TX}}` will be replaced with the text `{{B://TX}}` in the final content presented to a client 


### v2

_Open injection_

If you provide content from the blockchain you are compatible with the B://andlebars protocol v2 if you

- Are compatible with the B://andlebar protocol v1 or v1+

- Have a way for the client to indicate that the text `{{B://xyz}}` will be replaced with the raw unprocessed content of one specific other TX

- Have a way for the client to indicate that the text `{{B://xyz/}}` will be replaced with the B://andlebars treated content of the TX (nested injections)

Please note that v2 does not indicate how a content provider lets a client indicate what TX to target


### v3

_Multiple open injections_

If you provide content from the blockchain you are compatible with the B://andlebars protocol v3 if you

- Are compatible with the B://andlebars protocol v2

- Have a way of letting the client indicate a sequence of open injections to replace (`{{B://xyz1}}{{B://xyz2}}{{B://xyz3}}` to be replaced with TX1, TX2 and TX3)

Please note that v3 does not indicate how a content provider lets a client indicate what TXs to target.


