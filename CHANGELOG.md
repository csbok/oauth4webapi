# Changelog

All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.

## [2.0.6](https://github.com/panva/oauth4webapi/compare/v2.0.5...v2.0.6) (2022-12-16)


### Fixes

* **build:** fixup user agent version after version bump ([e1c3ed8](https://github.com/panva/oauth4webapi/commit/e1c3ed876c6e1f1baf9b260661ba33688f89b31c))

## [2.0.5](https://github.com/panva/oauth4webapi/compare/v2.0.4...v2.0.5) (2022-12-11)

## [2.0.4](https://github.com/panva/oauth4webapi/compare/v2.0.3...v2.0.4) (2022-11-27)


### Refactor

* weak maps instead of symbols ([e551edc](https://github.com/panva/oauth4webapi/commit/e551edc7f1a43df01895161fd27d0b19e5a827d4))

## [2.0.3](https://github.com/panva/oauth4webapi/compare/v2.0.1...v2.0.3) (2022-11-25)


### Fixes

* omit zealous response cloning() to reduce edge compute memory bills ([a785223](https://github.com/panva/oauth4webapi/commit/a78522393e7b7f4ac38a35a055375dfeb645c02f)), closes [#37](https://github.com/panva/oauth4webapi/issues/37)

## [2.0.1](https://github.com/panva/oauth4webapi/compare/v2.0.0...v2.0.1) (2022-11-21)


### Fixes

* claims parameter encoding in issued request objects ([3eb165a](https://github.com/panva/oauth4webapi/commit/3eb165a425212a12cf9e48f899a999d32dd9ec86))


### Performance

* cache public DPoP CryptoKey's JWK representation for re-use ([2858d06](https://github.com/panva/oauth4webapi/commit/2858d069325da31d72bfb45dad637b5ec54e4850))

## [2.0.0](https://github.com/panva/oauth4webapi/compare/v1.4.1...v2.0.0) (2022-11-20)


### ⚠ BREAKING CHANGES

* Use the TLS server validation in `processAuthorizationCodeOpenIDResponse` to validate the issuer instead of checking the ID Token's signature. The function's `options` argument was removed.
* Use the TLS server validation in `processDeviceCodeResponse` to validate the issuer instead of checking the optional ID Token's signature. The function's `options` argument was removed.
* Use the TLS server validation in `processIntrospectionResponse` to validate the issuer instead of checking the optional JWT Introspection Response signature. The function's `options` argument was removed.
* Use the TLS server validation in `processRefreshTokenResponse` to validate the issuer instead of checking the optional ID Token's signature. The function's `options` argument was removed.
* Use the TLS server validation in `processUserInfoResponse` to validate the issuer instead of checking the optional JWT UserInfo Response signature. The function's `options` argument was removed.
* PAR w/ DPoP no longer automatically adds `dpop_jkt` to the authorization request.
* Removed `calculateJwkThumbprint` function export.
* Removed `jwksRequest` function export.
* Removed `processJwksResponse` function export.

### Refactor

* remove ignored and unused exports ([4a545df](https://github.com/panva/oauth4webapi/commit/4a545df452840c183b377809cd5ac9f5b87c2aed))
* use TLS server validation instead of jwt signature validations ([f728110](https://github.com/panva/oauth4webapi/commit/f72811023f8816e3e1a5915a99a0fa7de9163069))

## [1.4.1](https://github.com/panva/oauth4webapi/compare/v1.4.0...v1.4.1) (2022-11-20)


### Refactor

* **deno:** add mod.ts to deno.land/x ([0778278](https://github.com/panva/oauth4webapi/commit/07782786053da9a2f58fbac933832a14fdf7c613))
* use RsaHashedKeyAlgorithm in checkRsaKeyAlgorithm ([94aa31c](https://github.com/panva/oauth4webapi/commit/94aa31c7ef7729ecddb52e6e47a6edc3db3c961d))

## [1.4.0](https://github.com/panva/oauth4webapi/compare/v1.3.0...v1.4.0) (2022-11-08)


### Features

* add bun as a supported runtime ([707efd1](https://github.com/panva/oauth4webapi/commit/707efd13046cf5297427f8a8acc5282c99fd3e48))

## [1.3.0](https://github.com/panva/oauth4webapi/compare/v1.2.2...v1.3.0) (2022-10-31)


### Features

* allow to skip JWT signature validation on select responses ([44d9114](https://github.com/panva/oauth4webapi/commit/44d9114e72e8c26e9ece195d5f92e776c7efef7e))

## [1.2.2](https://github.com/panva/oauth4webapi/compare/v1.2.1...v1.2.2) (2022-10-20)


### Refactor

* add a type check on AbortSignal ([b013fef](https://github.com/panva/oauth4webapi/commit/b013fef2a4bcbee9da558748b13a022182ebe214))
* align argument and function names in assert functions ([8ea65f6](https://github.com/panva/oauth4webapi/commit/8ea65f6a22af523ca1a75565d0ce28e05b1224b9))
* update "as" error messages ([3e894f5](https://github.com/panva/oauth4webapi/commit/3e894f59e573588c0608c95cc4e2d3465a7d08f3))

## [1.2.1](https://github.com/panva/oauth4webapi/compare/v1.2.0...v1.2.1) (2022-10-10)

## [1.2.0](https://github.com/panva/oauth4webapi/compare/v1.1.4...v1.2.0) (2022-09-14)


### Features

* add experimental EdDSA (Ed25519) JWS algorithm support ([f70d4d5](https://github.com/panva/oauth4webapi/commit/f70d4d52fb5473644c2c4b4c01cb4c8938f83f4d))

## [1.1.4](https://github.com/panva/oauth4webapi/compare/v1.1.3...v1.1.4) (2022-08-26)


### Fixes

* **typescript:** resolve ts4.8 issue ([572c6de](https://github.com/panva/oauth4webapi/commit/572c6dec99915fd52c958725d1cf15b8bbea4ab4))

## [1.1.3](https://github.com/panva/oauth4webapi/compare/v1.1.2...v1.1.3) (2022-07-20)

## [1.1.2](https://github.com/panva/oauth4webapi/compare/v1.1.1...v1.1.2) (2022-07-12)

## [1.1.1](https://github.com/panva/oauth4webapi/compare/v1.1.0...v1.1.1) (2022-07-04)


### Fixes

* processing pure oauth2 code response ignores invalid ID tokens ([282705a](https://github.com/panva/oauth4webapi/commit/282705a846a5d17c3d58f566a6e9e816ee753131))

## [1.1.0](https://github.com/panva/oauth4webapi/compare/v1.0.5...v1.1.0) (2022-06-28)


### Features

* allow AbortSignal-returning function as well as an instance ([90d21b8](https://github.com/panva/oauth4webapi/commit/90d21b871c00e74fbea584c700260067edea350b))

## [1.0.5](https://github.com/panva/oauth4webapi/compare/v1.0.4...v1.0.5) (2022-06-17)


### Fixes

* allow zero-length scope in token endpoint responses ([#15](https://github.com/panva/oauth4webapi/issues/15)) ([d54c821](https://github.com/panva/oauth4webapi/commit/d54c821aeb578dea93690801282d3e3d44bda8b8))

## [1.0.4](https://github.com/panva/oauth4webapi/compare/v1.0.3...v1.0.4) (2022-06-09)


### Fixes

* do not set a user-agent in CORS-enabled runtimes ([8899a6b](https://github.com/panva/oauth4webapi/commit/8899a6b58bd8ff7784db52264bb50623b2ffa07e)), closes [#13](https://github.com/panva/oauth4webapi/issues/13)

## [1.0.3](https://github.com/panva/oauth4webapi/compare/v1.0.2...v1.0.3) (2022-05-23)


### Fixes

* skip recalculating dpop_jkt in PAR if already set ([9499ccd](https://github.com/panva/oauth4webapi/commit/9499ccd45471b2404a9894f0411352ea36395ac7))

## [1.0.2](https://github.com/panva/oauth4webapi/compare/v1.0.1...v1.0.2) (2022-05-19)

## [1.0.1](https://github.com/panva/oauth4webapi/compare/v1.0.0...v1.0.1) (2022-05-18)


### Fixes

* reject unsupported token_type values ([3d2cc0c](https://github.com/panva/oauth4webapi/commit/3d2cc0cbcd53c9d33fe0c8cae44675736459ed1a))

## [1.0.0](https://github.com/panva/oauth4webapi/compare/v0.9.0...v1.0.0) (2022-05-13)

## [0.9.0](https://github.com/panva/oauth4webapi/compare/v0.8.0...v0.9.0) (2022-05-13)


### ⚠ BREAKING CHANGES

* **types:** rename TokenEndpointAuthMethod type to ClientAuthenticationMethod

### Refactor

* **types:** rename TokenEndpointAuthMethod type to ClientAuthenticationMethod ([6028fd8](https://github.com/panva/oauth4webapi/commit/6028fd85be4489eb999c934792d0cf3baaf88af3))

## [0.8.0](https://github.com/panva/oauth4webapi/compare/v0.7.0...v0.8.0) (2022-05-06)


### ⚠ BREAKING CHANGES

* getValidatedIdTokenClaims throws if ref isnt weak referenced
* remove client_secret_jwt

### Refactor

* getValidatedIdTokenClaims throws if ref isnt weak referenced ([1ee5485](https://github.com/panva/oauth4webapi/commit/1ee54858402d3099258f78e746ee14f6185f5cdf))
* remove client_secret_jwt ([7611169](https://github.com/panva/oauth4webapi/commit/7611169deb68cd9f8283ce8356a75bf8b5ab0f7f))

## [0.7.0](https://github.com/panva/oauth4webapi/compare/v0.6.4...v0.7.0) (2022-05-05)


### ⚠ BREAKING CHANGES

* ensure supported key in calculateJwkThumbprint
* clientCredentialsGrantRequest now requires parameters

### Features

* explicitly add dpop_jkt to par request when using dpop ([e6acd99](https://github.com/panva/oauth4webapi/commit/e6acd99220188b1f13a97e9a6e8f315ba0a2dfc9))


### Refactor

* clientCredentialsGrantRequest now requires parameters ([76e4fea](https://github.com/panva/oauth4webapi/commit/76e4fea3f1f9ec19dd1e24e51d29a91f91379837))
* ensure supported key in calculateJwkThumbprint ([540f6cf](https://github.com/panva/oauth4webapi/commit/540f6cfca4ae5757757542432e543430429391a7))

## [0.6.4](https://github.com/panva/oauth4webapi/compare/v0.6.3...v0.6.4) (2022-05-04)


### Features

* add utility for calculating dpop_jkt from a crypto key ([045dd10](https://github.com/panva/oauth4webapi/commit/045dd102e0886d01d41a28ec0a338da0e3e8ebe4))

## [0.6.3](https://github.com/panva/oauth4webapi/compare/v0.6.2...v0.6.3) (2022-05-04)

## [0.6.2](https://github.com/panva/oauth4webapi/compare/v0.6.1...v0.6.2) (2022-05-03)


### Features

* add utility for generating crypto key pairs ([d8f3e90](https://github.com/panva/oauth4webapi/commit/d8f3e90d001897587b8f7b496db43080e16ac1d5))

## [0.6.1](https://github.com/panva/oauth4webapi/compare/v0.6.0...v0.6.1) (2022-05-02)


### Fixes

* **types:** validateJwtAuthResponse expectedState is optional ([e618089](https://github.com/panva/oauth4webapi/commit/e61808900805813aed59197fa8b821eb48ecc526))

## [0.6.0](https://github.com/panva/oauth4webapi/compare/v0.5.2...v0.6.0) (2022-04-28)


### ⚠ BREAKING CHANGES

* remove encrypted JAR support

### Refactor

* remove encrypted JAR support ([4352049](https://github.com/panva/oauth4webapi/commit/435204953f80567f8b1711cb5796d1c1dd8f8d40))


### Fixes

* remove sub from request object ([41d49fa](https://github.com/panva/oauth4webapi/commit/41d49fa71707c9467219670b52d44d1e1e331870))
* signed userinfo aud and iss expected values ([38edd37](https://github.com/panva/oauth4webapi/commit/38edd37ea87f6d04446ea00507167920bf494ded))

## [0.5.2](https://github.com/panva/oauth4webapi/compare/v0.5.1...v0.5.2) (2022-04-27)


### Features

* force jwks refetch every 10 minutes ([ae35bae](https://github.com/panva/oauth4webapi/commit/ae35bae4e84a66c606eb6b40f2588a1aa1955b77))


### Fixes

* correct jwks refetch minimal interval ([8af6f85](https://github.com/panva/oauth4webapi/commit/8af6f85010f415ca519c668dbf8c3bcf5961d270))

## [0.5.1](https://github.com/panva/oauth4webapi/compare/v0.5.0...v0.5.1) (2022-04-27)


### Fixes

* assert no client private key is provided unless needed ([ac6be64](https://github.com/panva/oauth4webapi/commit/ac6be64ee4160a8c8d77577a2deb02a9a0388654))
* assert no client secret is provided unless needed ([604d8f3](https://github.com/panva/oauth4webapi/commit/604d8f36071912d064b1acacac38e5cf6bd6eb7c))
* ensure issueRequestObject does not mutate input parameters ([7b62b82](https://github.com/panva/oauth4webapi/commit/7b62b8211cad052f79eba61391d61ed24af69a3b))

## [0.5.0](https://github.com/panva/oauth4webapi/compare/v0.4.0...v0.5.0) (2022-04-27)


### ⚠ BREAKING CHANGES

* **deno:** support deno ^1.21.0 (removed 1.20.x from CI)
* **types:** rename SignalledRequestOptions interface to HttpRequestOptions

### Features

* option to add headers to http requests ([94a2ecb](https://github.com/panva/oauth4webapi/commit/94a2ecb2a5f7c17c84ff3fa39bc855e2c48466d6))


### Refactor

* **deno:** support deno ^1.21.0 (removed 1.20.x from CI) ([764db58](https://github.com/panva/oauth4webapi/commit/764db587cb83e2be0a6a085f5d75d97e5841ad55))
* **types:** rename SignalledRequestOptions interface to HttpRequestOptions ([e4058d8](https://github.com/panva/oauth4webapi/commit/e4058d82c79ca17216dbaabb306a8487211952c4))

## [0.4.0](https://github.com/panva/oauth4webapi/compare/v0.3.3...v0.4.0) (2022-04-25)


### ⚠ BREAKING CHANGES

* trim down the supported JOSE algorithms

### Refactor

* trim down the supported JOSE algorithms ([3a9e9a5](https://github.com/panva/oauth4webapi/commit/3a9e9a57a6b752c9789792364baf22e577377c5c))

## [0.3.3](https://github.com/panva/oauth4webapi/compare/v0.3.2...v0.3.3) (2022-04-14)

## [0.3.2](https://github.com/panva/oauth4webapi/compare/v0.3.1...v0.3.2) (2022-04-11)


### Features

* allow all key inputs to be CryptoKey instances ([f405719](https://github.com/panva/oauth4webapi/commit/f40571911856ffed541503d16d95fd724a980639))

## [0.3.1](https://github.com/panva/oauth4webapi/compare/v0.3.0...v0.3.1) (2022-04-10)

## [0.3.0](https://github.com/panva/oauth4webapi/compare/v0.2.2...v0.3.0) (2022-04-10)


### ⚠ BREAKING CHANGES

* **types:** force types without string defaults

### Refactor

* **types:** force types without string defaults ([188b252](https://github.com/panva/oauth4webapi/commit/188b25240a542a40044373f2696c0a2ef49964fa))

## [0.2.2](https://github.com/panva/oauth4webapi/compare/v0.2.1...v0.2.2) (2022-04-07)


### Features

* add generateRandomNonce ([ad60b2c](https://github.com/panva/oauth4webapi/commit/ad60b2c32b856b08b105372a201127669e344b74))
* add generateRandomState ([a39cc6b](https://github.com/panva/oauth4webapi/commit/a39cc6b2946c7824a7fbe169d49899e3ecaf5ec0))

## [0.2.1](https://github.com/panva/oauth4webapi/compare/v0.2.0...v0.2.1) (2022-04-05)

## [0.2.0](https://github.com/panva/oauth4webapi/compare/v0.1.0...v0.2.0) (2022-04-01)


### ⚠ BREAKING CHANGES

* ensure 2048 RSA keys are used for RSA-OAEP too

### Fixes

* ensure 2048 RSA keys are used for RSA-OAEP too ([f4eda79](https://github.com/panva/oauth4webapi/commit/f4eda799b6e461c121f365af213de8bc1379dadf))

## [0.1.0](https://github.com/panva/oauth4webapi/compare/v0.0.11...v0.1.0) (2022-04-01)


### ⚠ BREAKING CHANGES

* ensure 2048 RSA keys are used

### Fixes

* ensure 2048 RSA keys are used ([ad707c0](https://github.com/panva/oauth4webapi/commit/ad707c0e22651b45972aa14d797bcb36f14cd9f3))

## [0.0.11](https://github.com/panva/oauth4webapi/compare/v0.0.10...v0.0.11) (2022-04-01)

## [0.0.10](https://github.com/panva/oauth4webapi/compare/v0.0.9...v0.0.10) (2022-03-29)


### Fixes

* remove off-spec "default optional JWT typ" checks ([34e524a](https://github.com/panva/oauth4webapi/commit/34e524a8df08e9dfce5bce724ff7061aacd8a095))

## [0.0.9](https://github.com/panva/oauth4webapi/compare/v0.0.8...v0.0.9) (2022-03-28)


### Fixes

* normalize jwt typ when one is expected ([e161ee3](https://github.com/panva/oauth4webapi/commit/e161ee37be948d5b82e216e849a3a31c19ea02da))

## [0.0.8](https://github.com/panva/oauth4webapi/compare/v0.0.7...v0.0.8) (2022-03-28)

## [0.0.7](https://github.com/panva/oauth4webapi/compare/v0.0.6...v0.0.7) (2022-03-23)

## [0.0.6](https://github.com/panva/oauth4webapi/compare/v0.0.5...v0.0.6) (2022-03-18)

## [0.0.5](https://github.com/panva/oauth4webapi/compare/v0.0.4...v0.0.5) (2022-03-17)


### Fixes

* **jarm:** correct message when jarm response is passed to validateAuthResponse ([9ef7ce8](https://github.com/panva/oauth4webapi/commit/9ef7ce8526ef45e5944881f57353495681249c19))

## [0.0.4](https://github.com/panva/oauth4webapi/compare/v0.0.3...v0.0.4) (2022-03-17)

## [0.0.3](https://github.com/panva/oauth4webapi/compare/v0.0.2...v0.0.3) (2022-03-16)


### Features

* client_secret_jwt authentication method ([93fc723](https://github.com/panva/oauth4webapi/commit/93fc723d78e6e63de0c6bf87d028c8dc0559b313))


### Fixes

* **typescript:** allow any string into "alg" and "enc" client fields ([e6a8649](https://github.com/panva/oauth4webapi/commit/e6a86493cc8039d459f0d8de03c46f3918bccd8e))

## [0.0.2](https://github.com/panva/oauth4webapi/compare/v0.0.1...v0.0.2) (2022-03-16)


### Fixes

* set a proper user-agent string ([1fbb173](https://github.com/panva/oauth4webapi/commit/1fbb1733021b286cf242292c1b61a1336d0aed72))

### 0.0.1 (2022-03-16)
