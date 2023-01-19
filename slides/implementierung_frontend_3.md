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

```ts {all|1|4-10}
export function useSocket(host: string, basePath: string) {
	// WebSocket Setup ...
	return {
		participants: (domainId: string, workspaceId: string) => useParticipants(ws, domainId, workspaceId, listeners),
		participantsPointers: (domainId: string, workspaceId: string) =>
			useParticipantsPointers(ws, domainId, workspaceId, listeners),
		editors: (domainId: string, workspaceId: string) => useEditors(ws, domainId, workspaceId, listeners),
		followMe: (domainId: string, workspaceId: string) => useFollowMe(ws, domainId, workspaceId, listeners),
		laserpointer: (domainId: string, workspaceId: string) => useLaserpointer(ws, domainId, workspaceId, listeners),
		pushNotifications: () => usePushNotifications(ws),
	};
}
```
