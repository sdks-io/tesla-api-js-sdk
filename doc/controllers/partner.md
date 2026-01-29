# Partner

Partner account and telemetry endpoints

```ts
const partnerController = new PartnerController(client);
```

## Class Name

`PartnerController`

## Methods

* [Get Vins With Fleet Telemetry Errors](../../doc/controllers/partner.md#get-vins-with-fleet-telemetry-errors)
* [Get Recent Fleet Telemetry Errors](../../doc/controllers/partner.md#get-recent-fleet-telemetry-errors)
* [Get Public Key for a Domain](../../doc/controllers/partner.md#get-public-key-for-a-domain)
* [Register a Partner Account](../../doc/controllers/partner.md#register-a-partner-account)


# Get Vins With Fleet Telemetry Errors

```ts
async getVinsWithFleetTelemetryErrors(
  requestOptions?: RequestOptions
): Promise<ApiResponse<BackupResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`BackupResponse`](../../doc/models/backup-response.md).

## Example Usage

```ts
try {
  const response = await partnerController.getVinsWithFleetTelemetryErrors();

  // Extracting fully parsed response body.
  console.log(response.result);

  // Extracting response status code.
  console.log(response.statusCode);
  // Extracting response headers.
  console.log(response.headers);
  // Extracting response body of type `string | Stream`
  console.log(response.body);
} catch (error) {
  if (error instanceof ApiError) {
    // Extracting response error status code.
    console.log(error.statusCode);
    // Extracting response error headers.
    console.log(error.headers);
    // Extracting response error body of type `string | Stream`.
    console.log(error.body);
  }
}
```


# Get Recent Fleet Telemetry Errors

```ts
async getRecentFleetTelemetryErrors(
  requestOptions?: RequestOptions
): Promise<ApiResponse<FleetTelemetryErrorsResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`FleetTelemetryErrorsResponse`](../../doc/models/fleet-telemetry-errors-response.md).

## Example Usage

```ts
try {
  const response = await partnerController.getRecentFleetTelemetryErrors();

  // Extracting fully parsed response body.
  console.log(response.result);

  // Extracting response status code.
  console.log(response.statusCode);
  // Extracting response headers.
  console.log(response.headers);
  // Extracting response body of type `string | Stream`
  console.log(response.body);
} catch (error) {
  if (error instanceof ApiError) {
    // Extracting response error status code.
    console.log(error.statusCode);
    // Extracting response error headers.
    console.log(error.headers);
    // Extracting response error body of type `string | Stream`.
    console.log(error.body);
  }
}
```


# Get Public Key for a Domain

```ts
async getPublicKeyForADomain(
  domain: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<PublicKeyResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `domain` | `string` | Query, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`PublicKeyResponse`](../../doc/models/public-key-response.md).

## Example Usage

```ts
const domain = 'domain6';

try {
  const response = await partnerController.getPublicKeyForADomain(domain);

  // Extracting fully parsed response body.
  console.log(response.result);

  // Extracting response status code.
  console.log(response.statusCode);
  // Extracting response headers.
  console.log(response.headers);
  // Extracting response body of type `string | Stream`
  console.log(response.body);
} catch (error) {
  if (error instanceof ApiError) {
    // Extracting response error status code.
    console.log(error.statusCode);
    // Extracting response error headers.
    console.log(error.headers);
    // Extracting response error body of type `string | Stream`.
    console.log(error.body);
  }
}
```


# Register a Partner Account

```ts
async registerAPartnerAccount(
  body: RegisterPartnerRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<RegisterPartnerResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`RegisterPartnerRequest`](../../doc/models/register-partner-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`RegisterPartnerResponse`](../../doc/models/register-partner-response.md).

## Example Usage

```ts
const body: RegisterPartnerRequest = {
  domain: 'domain.com',
};

try {
  const response = await partnerController.registerAPartnerAccount(body);

  // Extracting fully parsed response body.
  console.log(response.result);

  // Extracting response status code.
  console.log(response.statusCode);
  // Extracting response headers.
  console.log(response.headers);
  // Extracting response body of type `string | Stream`
  console.log(response.body);
} catch (error) {
  if (error instanceof ApiError) {
    // Extracting response error status code.
    console.log(error.statusCode);
    // Extracting response error headers.
    console.log(error.headers);
    // Extracting response error body of type `string | Stream`.
    console.log(error.body);
  }
}
```

