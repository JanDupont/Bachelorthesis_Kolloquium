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

```ts {all|7|11}
import { useSocket } from "../socket/index.client";

const protocol = window.location.protocol == "http:" ? "ws" : "wss";
const socketUrl = `${protocol}://${window.location.host}`;
const s = useSocket(socketUrl, "/api/v1.0");

export function api(config: { host: string; basePath: string } = { host: "", basePath: "/api/v1.0" }) {
	const h = config.host;
	const bp = config.basePath;
	return {
		socket: () => s,
	};
}
```

</v-clicks>
