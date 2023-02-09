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

<v-clicks>

```ts {all|8|10,11,13,15,17} {maxHeight:'350px'}
export class Socket {
	// private socket Variables ...

	constructor() {
		// init socket
	}

	ParticipantPointers(domainId: string, instanceId: string) {
		return {
			register: (userId: string) => this.register(Category.ParticipantsPointers, domainId, instanceId, userId),
			unregister: (userId: string) =>
				this.unregister(Category.ParticipantsPointers, domainId, instanceId, userId),
			on: (callback: (payload: any) => void) =>
				this.on(Category.ParticipantsPointers, domainId, instanceId, callback),
			off: (callback: (payload: any) => void) =>
				this.off(Category.ParticipantsPointers, domainId, instanceId, callback),
			send: (payload: any) => this.send(Category.ParticipantsPointers, domainId, instanceId, payload),
		};
	}
}
```

</v-clicks>
