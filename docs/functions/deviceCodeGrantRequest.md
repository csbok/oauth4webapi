# Function: deviceCodeGrantRequest

[💗 Help the project](https://github.com/sponsors/panva)

▸ **deviceCodeGrantRequest**(`as`, `client`, `deviceCode`, `options?`): `Promise`<[`Response`]( https://developer.mozilla.org/en-US/docs/Web/API/Response )\>

Performs a Device Authorization Grant request at the
[`as.token_endpoint`](../interfaces/AuthorizationServer.md#token_endpoint).

**`see`** [RFC 8628 - OAuth 2.0 Device Authorization Grant](https://www.rfc-editor.org/rfc/rfc8628.html#section-3.4)

**`see`** [draft-ietf-oauth-dpop-11 - OAuth 2.0 Demonstrating Proof-of-Possession at the Application Layer (DPoP)](https://www.ietf.org/archive/id/draft-ietf-oauth-dpop-11.html#name-dpop-access-token-request)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `as` | [`AuthorizationServer`](../interfaces/AuthorizationServer.md) | Authorization Server Metadata. |
| `client` | [`Client`](../interfaces/Client.md) | Client Metadata. |
| `deviceCode` | `string` | Device Code. |
| `options?` | [`TokenEndpointRequestOptions`](../interfaces/TokenEndpointRequestOptions.md) | - |

#### Returns

`Promise`<[`Response`]( https://developer.mozilla.org/en-US/docs/Web/API/Response )\>
