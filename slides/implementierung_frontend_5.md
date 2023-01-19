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

```ts
api().socket().participants(domainId, workspaceId).send({ type: "addParticipant", userId: "1234" });
```
