# Implementierung Frontend

<ul>
    <li >Vue SFC</li>
    <li >Vue Composition API</li>
    <li ><strong>WebSocket Client</strong></li>
</ul>

<style>
    strong {
        color: lightgreen !important;
    }
</style>

```ts {all|1,3|5|7|9-15|17-19|21-24|25-27} {maxHeight:'350px'}
import * as teamlyClient from "teamly/client";

let teamlySocket = new teamlyClient.Socket();

teamlySocket.initialize(domainId, workspaceId).register(userId);

teamlySocket.ParticipantPointers(domainId, workspaceId).register(userId);

let payload = {
	x: 0,
	y: 0,
	color: "red",
	userId: userId,
};
teamlySocket.ParticipantPointers(domainId, workspaceId).send(payload);

teamlySocket.ParticipantPointers(domainId, workspaceId).on((data: any) => {
	// ... do something with data
});

teamlySocket.ParticipantPointers(domainId, workspaceId).off((data: any) => {
	// ... do something with data
});

teamlySocket.ParticipantPointers(domainId, workspaceId).unregister(userId);
```
