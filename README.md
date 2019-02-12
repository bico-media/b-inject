Status: _idea_ → __lose draft__ → _draft_ → _proposal_ → _final review_ → _stable_

# Dynamic content from a static blockchain

> Let's get a shared way of indicating that content in one transaction is to be placed within content from another transaction.

This document describes a protocol named "B://inject" (pronounced _Binject_).
Please share [inputs and comments](https://github.com/bico-media/binject/issues).

## Overview

### Version 1

The protocol B://inject v1 describes "direct injections". In short: 

> The text `{{B://[TX]}}` will be replaced with the raw unprocessed content of TX
>
> The text `{{B://[TX]/}}` will be replaced with the B://inject treated content of the TX (nested injections)

See [binject.bico.media/v1](http://binject.bico.media/v1) for more information.


### Version 1 plus

The protocol B://inject v1+ describes "How to talking about direct injections using direct injections". In short:_

> The text `{{B:\\TX}}` will be replaced with the text `{{B://TX}}` in the final content presented to a client 

See [binject.bico.media/v1-plus](http://binject.bico.media/v1-plus) for more information.


### Version 2

The protocol B://inject v2 describes "open injections". In short: 

> Have a way for the client to indicate that the text `{{B://xyz}}` will be replaced with the raw unprocessed content of one specific other TX
> 
> Have a way for the client to indicate that the text `{{B://xyz/}}` will be replaced with the B://inject treated content of a specific other TX (nested injections)

See [binject.bico.media/v2](http://binject.bico.media/v2) for more information.



### Version 3

The protocol B://inject v3 describes "Multiple open injections". In short: 

> Have a way of letting the client indicate a sequence of open injections to replace (i.e `{{B://xyz1}}{{B://xyz2}}{{B://xyz3}}` to be replaced with TX1, TX2 and TX3)

See [binject.bico.media/v3](http://binject.bico.media/v3) for more information.

----

Please share [inputs and comments](https://github.com/bico-media/binject/issues).

