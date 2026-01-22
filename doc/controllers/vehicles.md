# Vehicles

```ts
const vehiclesController = new VehiclesController(client);
```

## Class Name

`VehiclesController`

## Methods

* [List Vehicles](../../doc/controllers/vehicles.md#list-vehicles)
* [Get Vehicle](../../doc/controllers/vehicles.md#get-vehicle)
* [Mobile Enabled](../../doc/controllers/vehicles.md#mobile-enabled)
* [Nearby Charging Sites](../../doc/controllers/vehicles.md#nearby-charging-sites)
* [Vehicle Live Data](../../doc/controllers/vehicles.md#vehicle-live-data)
* [Wake up Vehicle](../../doc/controllers/vehicles.md#wake-up-vehicle)
* [Vehicle Specs](../../doc/controllers/vehicles.md#vehicle-specs)
* [Vehicle Options](../../doc/controllers/vehicles.md#vehicle-options)
* [Warranty Details](../../doc/controllers/vehicles.md#warranty-details)
* [Get Allowed Drivers for a Vehicle](../../doc/controllers/vehicles.md#get-allowed-drivers-for-a-vehicle)
* [Remove Driver Access From a Vehicle](../../doc/controllers/vehicles.md#remove-driver-access-from-a-vehicle)
* [Get Eligible Vehicle Subscriptions](../../doc/controllers/vehicles.md#get-eligible-vehicle-subscriptions)
* [Get Eligible Vehicle Upgrades](../../doc/controllers/vehicles.md#get-eligible-vehicle-upgrades)
* [Set Enterprise Payer Roles](../../doc/controllers/vehicles.md#set-enterprise-payer-roles)
* [Get Enterprise Roles for a Vehicle](../../doc/controllers/vehicles.md#get-enterprise-roles-for-a-vehicle)
* [Get Fleet Status for Vehicles](../../doc/controllers/vehicles.md#get-fleet-status-for-vehicles)
* [Create or Update Fleet Telemetry Configuration](../../doc/controllers/vehicles.md#create-or-update-fleet-telemetry-configuration)
* [Get Fleet Telemetry Configuration](../../doc/controllers/vehicles.md#get-fleet-telemetry-configuration)
* [Delete Fleet Telemetry Configuration](../../doc/controllers/vehicles.md#delete-fleet-telemetry-configuration)
* [Configure Fleet Telemetry Using Signed JWS Token](../../doc/controllers/vehicles.md#configure-fleet-telemetry-using-signed-jws-token)
* [Get Fleet Telemetry Errors for a Vehicle](../../doc/controllers/vehicles.md#get-fleet-telemetry-errors-for-a-vehicle)


# List Vehicles

```ts
async listVehicles(
  requestOptions?: RequestOptions
): Promise<ApiResponse<Api1VehiclesResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`Api1VehiclesResponse`](../../doc/models/api-1-vehicles-response.md).

## Example Usage

```ts
try {
  const response = await vehiclesController.listVehicles();

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


# Get Vehicle

```ts
async getVehicle(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<Api1VehiclesResponseGetVehicle>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`Api1VehiclesResponseGetVehicle`](../../doc/models/api-1-vehicles-response-get-vehicle.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehiclesController.getVehicle(vehicleTag);

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


# Mobile Enabled

```ts
async mobileEnabled(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<Api1VehiclesMobileEnabledResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`Api1VehiclesMobileEnabledResponse`](../../doc/models/api-1-vehicles-mobile-enabled-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehiclesController.mobileEnabled(vehicleTag);

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


# Nearby Charging Sites

```ts
async nearbyChargingSites(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<Api1VehiclesNearbyChargingSitesResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`Api1VehiclesNearbyChargingSitesResponse`](../../doc/models/api-1-vehicles-nearby-charging-sites-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehiclesController.nearbyChargingSites(vehicleTag);

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


# Vehicle Live Data

```ts
async vehicleLiveData(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<SiteInfoResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`SiteInfoResponse`](../../doc/models/site-info-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehiclesController.vehicleLiveData(vehicleTag);

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


# Wake up Vehicle

```ts
async wakeUpVehicle(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<Api1VehiclesWakeUpResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`Api1VehiclesWakeUpResponse`](../../doc/models/api-1-vehicles-wake-up-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehiclesController.wakeUpVehicle(vehicleTag);

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


# Vehicle Specs

```ts
async vehicleSpecs(
  vin: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<SiteInfoResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`SiteInfoResponse`](../../doc/models/site-info-response.md).

## Example Usage

```ts
const vin = 'vin6';

try {
  const response = await vehiclesController.vehicleSpecs(vin);

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


# Vehicle Options

```ts
async vehicleOptions(
  vin: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<Api1DxVehiclesOptionsResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Query, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`Api1DxVehiclesOptionsResponse`](../../doc/models/api-1-dx-vehicles-options-response.md).

## Example Usage

```ts
const vin = 'vin6';

try {
  const response = await vehiclesController.vehicleOptions(vin);

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


# Warranty Details

```ts
async warrantyDetails(
  requestOptions?: RequestOptions
): Promise<ApiResponse<Api1DxWarrantyDetailsResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`Api1DxWarrantyDetailsResponse`](../../doc/models/api-1-dx-warranty-details-response.md).

## Example Usage

```ts
try {
  const response = await vehiclesController.warrantyDetails();

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


# Get Allowed Drivers for a Vehicle

```ts
async getAllowedDriversForAVehicle(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<DriversResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`DriversResponse`](../../doc/models/drivers-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehiclesController.getAllowedDriversForAVehicle(vehicleTag);

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


# Remove Driver Access From a Vehicle

```ts
async removeDriverAccessFromAVehicle(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<SimpleOkResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`SimpleOkResponse`](../../doc/models/simple-ok-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehiclesController.removeDriverAccessFromAVehicle(vehicleTag);

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


# Get Eligible Vehicle Subscriptions

```ts
async getEligibleVehicleSubscriptions(
  vin: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<SiteInfoResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Query, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`SiteInfoResponse`](../../doc/models/site-info-response.md).

## Example Usage

```ts
const vin = 'vin6';

try {
  const response = await vehiclesController.getEligibleVehicleSubscriptions(vin);

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


# Get Eligible Vehicle Upgrades

```ts
async getEligibleVehicleUpgrades(
  vin: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<SiteInfoResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Query, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`SiteInfoResponse`](../../doc/models/site-info-response.md).

## Example Usage

```ts
const vin = 'vin6';

try {
  const response = await vehiclesController.getEligibleVehicleUpgrades(vin);

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


# Set Enterprise Payer Roles

```ts
async setEnterprisePayerRoles(
  vin: string,
  body: EnterprisePayerRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Template, Required | - |
| `body` | [`EnterprisePayerRequest`](../../doc/models/enterprise-payer-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const vin = 'vin6';

const body: EnterprisePayerRequest = {
  role: 'role0',
};

try {
  const response = await vehiclesController.setEnterprisePayerRoles(
    vin,
    body
  );

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


# Get Enterprise Roles for a Vehicle

```ts
async getEnterpriseRolesForAVehicle(
  vin: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<unknown | undefined>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type `unknown`.

## Example Usage

```ts
const vin = 'vin6';

try {
  const response = await vehiclesController.getEnterpriseRolesForAVehicle(vin);

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


# Get Fleet Status for Vehicles

```ts
async getFleetStatusForVehicles(
  body: FleetStatusRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<unknown | undefined>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`FleetStatusRequest`](../../doc/models/fleet-status-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type `unknown`.

## Example Usage

```ts
const body: FleetStatusRequest = {
};

try {
  const response = await vehiclesController.getFleetStatusForVehicles(body);

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


# Create or Update Fleet Telemetry Configuration

```ts
async createOrUpdateFleetTelemetryConfiguration(
  body: unknown,
  requestOptions?: RequestOptions
): Promise<ApiResponse<unknown | undefined>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | `unknown` | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type `unknown`.

## Example Usage

```ts
const body = { 'key1': 'val1', 'key2': 'val2' };

try {
  const response = await vehiclesController.createOrUpdateFleetTelemetryConfiguration(body);

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


# Get Fleet Telemetry Configuration

```ts
async getFleetTelemetryConfiguration(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<unknown | undefined>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type `unknown`.

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehiclesController.getFleetTelemetryConfiguration(vehicleTag);

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


# Delete Fleet Telemetry Configuration

```ts
async deleteFleetTelemetryConfiguration(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<unknown | undefined>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type `unknown`.

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehiclesController.deleteFleetTelemetryConfiguration(vehicleTag);

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


# Configure Fleet Telemetry Using Signed JWS Token

```ts
async configureFleetTelemetryUsingSignedJwsToken(
  body: FleetTelemetryJwsRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<unknown | undefined>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`FleetTelemetryJwsRequest`](../../doc/models/fleet-telemetry-jws-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type `unknown`.

## Example Usage

```ts
const body: FleetTelemetryJwsRequest = {
};

try {
  const response = await vehiclesController.configureFleetTelemetryUsingSignedJwsToken(body);

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


# Get Fleet Telemetry Errors for a Vehicle

```ts
async getFleetTelemetryErrorsForAVehicle(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<unknown | undefined>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type `unknown`.

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehiclesController.getFleetTelemetryErrorsForAVehicle(vehicleTag);

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

