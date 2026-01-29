# Vehicle Commands

```ts
const vehicleCommandsController = new VehicleCommandsController(client);
```

## Class Name

`VehicleCommandsController`

## Methods

* [Actuate Trunk](../../doc/controllers/vehicle-commands.md#actuate-trunk)
* [Add Charge Schedule](../../doc/controllers/vehicle-commands.md#add-charge-schedule)
* [Add Precondition Schedule](../../doc/controllers/vehicle-commands.md#add-precondition-schedule)
* [Adjust Media Volume](../../doc/controllers/vehicle-commands.md#adjust-media-volume)
* [Start Climate Preconditioning](../../doc/controllers/vehicle-commands.md#start-climate-preconditioning)
* [Stop Climate Preconditioning](../../doc/controllers/vehicle-commands.md#stop-climate-preconditioning)
* [Cancel Software Update](../../doc/controllers/vehicle-commands.md#cancel-software-update)
* [Charge Max Range](../../doc/controllers/vehicle-commands.md#charge-max-range)
* [Open Charge Port Door](../../doc/controllers/vehicle-commands.md#open-charge-port-door)
* [Close Charge Port Door](../../doc/controllers/vehicle-commands.md#close-charge-port-door)
* [Charge Standard](../../doc/controllers/vehicle-commands.md#charge-standard)
* [Start Charging](../../doc/controllers/vehicle-commands.md#start-charging)
* [Stop Charging](../../doc/controllers/vehicle-commands.md#stop-charging)
* [Clear PIN to Drive Admin](../../doc/controllers/vehicle-commands.md#clear-pin-to-drive-admin)
* [Lock Doors](../../doc/controllers/vehicle-commands.md#lock-doors)
* [Unlock Doors](../../doc/controllers/vehicle-commands.md#unlock-doors)
* [Erase User Data](../../doc/controllers/vehicle-commands.md#erase-user-data)
* [Flash Lights](../../doc/controllers/vehicle-commands.md#flash-lights)
* [Enable or Disable Guest Mode](../../doc/controllers/vehicle-commands.md#enable-or-disable-guest-mode)
* [Honk Horn](../../doc/controllers/vehicle-commands.md#honk-horn)
* [Next Favorite Media Track](../../doc/controllers/vehicle-commands.md#next-favorite-media-track)


# Actuate Trunk

Controls the front or rear trunk

```ts
async actuateTrunk(
  vehicleTag: string,
  body: ActuateTrunkRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`ActuateTrunkRequest`](../../doc/models/actuate-trunk-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

const body: ActuateTrunkRequest = {
  whichTrunk: WhichTrunk.Front,
};

try {
  const response = await vehicleCommandsController.actuateTrunk(
    vehicleTag,
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


# Add Charge Schedule

```ts
async addChargeSchedule(
  vehicleTag: string,
  body: AddChargeScheduleRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`AddChargeScheduleRequest`](../../doc/models/add-charge-schedule-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

const body: AddChargeScheduleRequest = {
  lat: 213.84,
  lon: 209.06,
  id: 120,
  enabled: false,
};

try {
  const response = await vehicleCommandsController.addChargeSchedule(
    vehicleTag,
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


# Add Precondition Schedule

```ts
async addPreconditionSchedule(
  vehicleTag: string,
  body: AddPreconditionScheduleRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`AddPreconditionScheduleRequest`](../../doc/models/add-precondition-schedule-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

const body: AddPreconditionScheduleRequest = {
  lat: 213.84,
  lon: 209.06,
  id: 120,
  enabled: false,
};

try {
  const response = await vehicleCommandsController.addPreconditionSchedule(
    vehicleTag,
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


# Adjust Media Volume

```ts
async adjustMediaVolume(
  vehicleTag: string,
  body: AdjustVolumeRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`AdjustVolumeRequest`](../../doc/models/adjust-volume-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

const body: AdjustVolumeRequest = {
  volume: 74,
};

try {
  const response = await vehicleCommandsController.adjustMediaVolume(
    vehicleTag,
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


# Start Climate Preconditioning

```ts
async startClimatePreconditioning(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.startClimatePreconditioning(vehicleTag);

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


# Stop Climate Preconditioning

```ts
async stopClimatePreconditioning(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.stopClimatePreconditioning(vehicleTag);

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


# Cancel Software Update

```ts
async cancelSoftwareUpdate(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.cancelSoftwareUpdate(vehicleTag);

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


# Charge Max Range

```ts
async chargeMaxRange(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.chargeMaxRange(vehicleTag);

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


# Open Charge Port Door

```ts
async openChargePortDoor(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.openChargePortDoor(vehicleTag);

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


# Close Charge Port Door

```ts
async closeChargePortDoor(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.closeChargePortDoor(vehicleTag);

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


# Charge Standard

```ts
async chargeStandard(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.chargeStandard(vehicleTag);

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


# Start Charging

```ts
async startCharging(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.startCharging(vehicleTag);

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


# Stop Charging

```ts
async stopCharging(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.stopCharging(vehicleTag);

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


# Clear PIN to Drive Admin

Deactivates PIN to Drive and resets the associated PIN for supported firmware versions.

```ts
async clearPinToDriveAdmin(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.clearPinToDriveAdmin(vehicleTag);

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


# Lock Doors

```ts
async lockDoors(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.lockDoors(vehicleTag);

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


# Unlock Doors

```ts
async unlockDoors(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.unlockDoors(vehicleTag);

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


# Erase User Data

Erases user data from the vehicle UI. Requires Guest Mode.

```ts
async eraseUserData(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.eraseUserData(vehicleTag);

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


# Flash Lights

Briefly flashes vehicle headlights.

```ts
async flashLights(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.flashLights(vehicleTag);

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


# Enable or Disable Guest Mode

```ts
async enableOrDisableGuestMode(
  vehicleTag: string,
  body: GuestModeRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`GuestModeRequest`](../../doc/models/guest-mode-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

const body: GuestModeRequest = {
  enable: false,
};

try {
  const response = await vehicleCommandsController.enableOrDisableGuestMode(
    vehicleTag,
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


# Honk Horn

```ts
async honkHorn(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.honkHorn(vehicleTag);

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


# Next Favorite Media Track

```ts
async nextFavoriteMediaTrack(
  vehicleTag: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CommandResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```ts
const vehicleTag = 'vehicle_tag6';

try {
  const response = await vehicleCommandsController.nextFavoriteMediaTrack(vehicleTag);

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

