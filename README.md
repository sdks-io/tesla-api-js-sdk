
# Getting Started with Tesla Fleet Management API

## Introduction

Unofficial OpenAPI specification for Tesla Fleet Management Charging endpoints.

## Install the Package

Run the following command from your project directory to install the package from npm:

```bash
npm install tesla-api-sdk@1.0.2
```

For additional package details, see the [Npm page for the tesla-api-sdk@1.0.2 npm](https://www.npmjs.com/package/tesla-api-sdk/v/1.0.2).

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| environment | `Environment` | The API environment. <br> **Default: `Environment.Production`** |
| timeout | `number` | Timeout for API calls.<br>*Default*: `0` |
| httpClientOptions | [`Partial<HttpClientOptions>`](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/http-client-options.md) | Stable configurable http client options. |
| unstableHttpClientOptions | `any` | Unstable configurable http client options. |
| logging | [`PartialLoggingOptions`](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/partial-logging-options.md) | Logging Configuration to enable logging |
| bearerAuthCredentials | [`BearerAuthCredentials`](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/auth/oauth-2-bearer-token.md) | The credential object for bearerAuth |
| thirdpartytokenCredentials | [`ThirdpartytokenCredentials`](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/auth/oauth-2-authorization-code-grant.md) | The credential object for thirdpartytoken |

The API client can be initialized as follows:

### Code-Based Client Initialization

```ts
import {
  Client,
  Environment,
  LogLevel,
  OAuthScopeThirdpartytoken,
} from 'tesla-api-sdk';

const client = new Client({
  bearerAuthCredentials: {
    accessToken: 'AccessToken'
  },
  thirdpartytokenCredentials: {
    oAuthClientId: 'OAuthClientId',
    oAuthClientSecret: 'OAuthClientSecret',
    oAuthRedirectUri: 'OAuthRedirectUri',
    oAuthScopes: [
      OAuthScopeThirdpartytoken.Openid,
      OAuthScopeThirdpartytoken.OfflineAccess
    ]
  },
  timeout: 0,
  environment: Environment.Production,
  logging: {
    logLevel: LogLevel.Info,
    logRequest: {
      logBody: true
    },
    logResponse: {
      logHeaders: true
    }
  },
});
```

### Configuration-Based Client Initialization

```ts
import * as path from 'path';
import * as fs from 'fs';
import { Client } from 'tesla-api-sdk';

// Provide absolute path for the configuration file
const absolutePath = path.resolve('./config.json');

// Read the configuration file content
const fileContent = fs.readFileSync(absolutePath, 'utf-8');

// Initialize client from JSON configuration content
const client = Client.fromJsonConfig(fileContent);
```

See the [Configuration-Based Client Initialization](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/configuration-based-client-initialization.md) section for details.

### Environment-Based Client Initialization

```ts
import * as dotenv from 'dotenv';
import * as path from 'path';
import * as fs from 'fs';
import { Client } from 'tesla-api-sdk';

// Optional - Provide absolute path for the .env file
const absolutePath = path.resolve('./.env');

if (fs.existsSync(absolutePath)) {
  // Load environment variables from .env file
  dotenv.config({ path: absolutePath, override: true });
}

// Initialize client using environment variables
const client = Client.fromEnvironment(process.env);
```

See the [Environment-Based Client Initialization](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/environment-based-client-initialization.md) section for details.

## Authorization

This API uses the following authentication schemes.

* [`bearerAuth (OAuth 2 Bearer token)`](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/auth/oauth-2-bearer-token.md)
* [`thirdpartytoken (OAuth 2 Authorization Code Grant)`](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/auth/oauth-2-authorization-code-grant.md)

## List of APIs

* [Vehicle Commands](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/controllers/vehicle-commands.md)
* [Charging](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/controllers/charging.md)
* [Energy](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/controllers/energy.md)
* [Partner](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/controllers/partner.md)
* [User](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/controllers/user.md)
* [Vehicles](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/controllers/vehicles.md)

## SDK Infrastructure

### Configuration

* [HttpClientOptions](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/http-client-options.md)
* [RetryConfiguration](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/retry-configuration.md)
* [ProxySettings](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/proxy-settings.md)
* [Configuration-Based Client Initialization](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/configuration-based-client-initialization.md)
* [Environment-Based Client Initialization](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/environment-based-client-initialization.md)
* [PartialLoggingOptions](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/partial-logging-options.md)
* [PartialRequestLoggingOptions](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/partial-request-logging-options.md)
* [PartialResponseLoggingOptions](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/partial-response-logging-options.md)
* [LoggerInterface](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/logger-interface.md)

### HTTP

* [HttpRequest](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/http-request.md)

### Utilities

* [ApiResponse](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/api-response.md)
* [ApiError](https://www.github.com/sdks-io/tesla-api-js-sdk/tree/1.0.2/doc/api-error.md)

