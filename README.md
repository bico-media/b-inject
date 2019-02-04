# Dynamic content from a static blockchain

> Lets get a shared way of indicating that content in one transaction is to be placed within content from another transaction.

This document describes a protocol named "B://andlebars" (pronounced bandlebars).
Please share [inputs and comments](https://github.com/bico-media/bandlebars/issues).


## Overview

### B://andlebar v1

B://andlebar v1 describes "direct injections". In short: 

> - The text `{{B://[TX]}}` will be replaced with the raw unprocessed content of TX
>
> - The text `{{B://[TX]/}}` will be replaced with the B://andlebar converted content of the TX (nested injections)

See [banlebars.bico.media/v1](//banlebars.bico.media/v1) for more information.


### B://andlebar v1+

B://andlebar v1 describes "How to talking about direct injections using direct injections". In short:_


> - The text `{{B:\\TX}}` will be replaced with the text `{{B://TX}}` in the final content presented to a client 

See [banlebars.bico.media/v1](//banlebars.bico.media/v1-plus) for more information.


### B://andlebar v2

B://andlebar v2 describes "open injections". In short: 

> - Have a way for the client to indicate that the text `{{B://xyz}}` will be replaced with the raw unprocessed content of one specific other TX
> 
> - Have a way for the client to indicate that the text `{{B://xyz/}}` will be replaced with the B://andlebars treated content of the TX (nested injections)

See [banlebars.bico.media/v1](//banlebars.bico.media/v2) for more information.


### B://andlebar v3

_Multiple open injections_

B://andlebar v3 describes "Multiple open injections". In short: 

> - Have a way of letting the client indicate a sequence of open injections to replace (`{{B://xyz1}}{{B://xyz2}}{{B://xyz3}}` to be replaced with TX1, TX2 and TX3)

See [banlebars.bico.media/v1](//banlebars.bico.media/v3) for more information.


----

Please share [inputs and comments](https://github.com/bico-media/bandlebars/issues).

