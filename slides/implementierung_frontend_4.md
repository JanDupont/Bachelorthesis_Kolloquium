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

```ts {all|1|9,12,15}
export function useParticipants(
	ws: WebSocket,
	domainId: string,
	workspaceId: string,
	listeners: { [key: string]: (payload: any) => void }
) {
	const topic = `/${domainId}/${workspaceId}/participants`;

	function on(userId: string, cb: (data: any) => void) {
		// ...
	}
	function off() {
		// ...
	}
	function send(payload: { type: "addParticipant" | "removeParticipant"; userId: string }) {
		// ...
	}
	return { on, off, send };
}
```
