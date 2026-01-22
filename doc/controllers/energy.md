# Energy

Energy site and Powerwall endpoints

```ts
const energyController = new EnergyController(client);
```

## Class Name

`EnergyController`

## Methods

* [Adjust Site S Backup Reserve](../../doc/controllers/energy.md#adjust-site-s-backup-reserve)
* [Get Backup or Energy History](../../doc/controllers/energy.md#get-backup-or-energy-history)
* [Get Wall Connector Charging History](../../doc/controllers/energy.md#get-wall-connector-charging-history)
* [Get Live Site Status](../../doc/controllers/energy.md#get-live-site-status)
* [Set Site Mode Autonomous or Self Consumption](../../doc/controllers/energy.md#set-site-mode-autonomous-or-self-consumption)
* [Allow Disallow Charging From the Grid and Exporting Energy to the Grid](../../doc/controllers/energy.md#allow-disallow-charging-from-the-grid-and-exporting-energy-to-the-grid)
* [Adjust Site S Off-Grid Vehicle Charging Reserve](../../doc/controllers/energy.md#adjust-site-s-off-grid-vehicle-charging-reserve)
* [Update Storm Watch Participation](../../doc/controllers/energy.md#update-storm-watch-participation)
* [Update Time-of-Use TOU Settings](../../doc/controllers/energy.md#update-time-of-use-tou-settings)
* [Get User Products Vehicles Energy Sites](../../doc/controllers/energy.md#get-user-products-vehicles-energy-sites)
* [Get Site Information Assets Settings Features](../../doc/controllers/energy.md#get-site-information-assets-settings-features)


# Adjust Site S Backup Reserve

```ts
async adjustSiteSBackupReserve(
  energySiteId: string,
  body: BackupRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<BackupResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`BackupRequest`](../../doc/models/backup-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`BackupResponse`](../../doc/models/backup-response.md).

## Example Usage

```ts
const energySiteId = 'energy_site_id2';

const body: BackupRequest = {
  backupReservePercent: 76,
};

try {
  const response = await energyController.adjustSiteSBackupReserve(
    energySiteId,
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


# Get Backup or Energy History

```ts
async getBackupOrEnergyHistory(
  energySiteId: string,
  kind: Kind,
  startDate: string,
  endDate: string,
  period?: string,
  timeZone?: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<CalendarHistoryResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `kind` | [`Kind`](../../doc/models/kind.md) | Query, Required | - |
| `startDate` | `string` | Query, Required | - |
| `endDate` | `string` | Query, Required | - |
| `period` | `string \| undefined` | Query, Optional | - |
| `timeZone` | `string \| undefined` | Query, Optional | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`CalendarHistoryResponse`](../../doc/models/calendar-history-response.md).

## Example Usage

```ts
const energySiteId = 'energy_site_id2';

const kind = Kind.Backup;

const startDate = '2016-03-13T12:52:32.123Z';

const endDate = '2016-03-13T12:52:32.123Z';

try {
  const response = await energyController.getBackupOrEnergyHistory(
    energySiteId,
    kind,
    startDate,
    endDate
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


# Get Wall Connector Charging History

```ts
async getWallConnectorChargingHistory(
  energySiteId: string,
  kind: KindGetWallConnectorChargingHistory,
  startDate: string,
  endDate: string,
  timeZone?: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<ChargeHistoryResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `kind` | [`KindGetWallConnectorChargingHistory`](../../doc/models/kind-get-wall-connector-charging-history.md) | Query, Required | - |
| `startDate` | `string` | Query, Required | - |
| `endDate` | `string` | Query, Required | - |
| `timeZone` | `string \| undefined` | Query, Optional | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`ChargeHistoryResponse`](../../doc/models/charge-history-response.md).

## Example Usage

```ts
const energySiteId = 'energy_site_id2';

const kind = KindGetWallConnectorChargingHistory.Charge;

const startDate = '2016-03-13T12:52:32.123Z';

const endDate = '2016-03-13T12:52:32.123Z';

try {
  const response = await energyController.getWallConnectorChargingHistory(
    energySiteId,
    kind,
    startDate,
    endDate
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


# Get Live Site Status

```ts
async getLiveSiteStatus(
  energySiteId: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<LiveStatusResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`LiveStatusResponse`](../../doc/models/live-status-response.md).

## Example Usage

```ts
const energySiteId = 'energy_site_id2';

try {
  const response = await energyController.getLiveSiteStatus(energySiteId);

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


# Set Site Mode Autonomous or Self Consumption

```ts
async setSiteModeAutonomousOrSelfConsumption(
  energySiteId: string,
  body: OperationRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<GenericUpdateResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`OperationRequest`](../../doc/models/operation-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`GenericUpdateResponse`](../../doc/models/generic-update-response.md).

## Example Usage

```ts
const energySiteId = 'energy_site_id2';

const body: OperationRequest = {
  defaultRealMode: DefaultRealMode.Autonomous,
};

try {
  const response = await energyController.setSiteModeAutonomousOrSelfConsumption(
    energySiteId,
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


# Allow Disallow Charging From the Grid and Exporting Energy to the Grid

```ts
async allowDisallowChargingFromTheGridAndExportingEnergyToTheGrid(
  energySiteId: string,
  body?: unknown,
  requestOptions?: RequestOptions
): Promise<ApiResponse<GenericUpdateResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | `unknown \| undefined` | Body, Optional | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`GenericUpdateResponse`](../../doc/models/generic-update-response.md).

## Example Usage

```ts
const energySiteId = 'energy_site_id2';

try {
  const response = await energyController.allowDisallowChargingFromTheGridAndExportingEnergyToTheGrid(energySiteId);

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


# Adjust Site S Off-Grid Vehicle Charging Reserve

```ts
async adjustSiteSOffGridVehicleChargingReserve(
  energySiteId: string,
  body: OffGridVehicleChargingReserveRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<GenericUpdateResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`OffGridVehicleChargingReserveRequest`](../../doc/models/off-grid-vehicle-charging-reserve-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`GenericUpdateResponse`](../../doc/models/generic-update-response.md).

## Example Usage

```ts
const energySiteId = 'energy_site_id2';

const body: OffGridVehicleChargingReserveRequest = {
  offGridVehicleChargingReservePercent: 52,
};

try {
  const response = await energyController.adjustSiteSOffGridVehicleChargingReserve(
    energySiteId,
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


# Update Storm Watch Participation

```ts
async updateStormWatchParticipation(
  energySiteId: string,
  body: StormModeRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<GenericUpdateResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`StormModeRequest`](../../doc/models/storm-mode-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`GenericUpdateResponse`](../../doc/models/generic-update-response.md).

## Example Usage

```ts
const energySiteId = 'energy_site_id2';

const body: StormModeRequest = {
  enabled: false,
};

try {
  const response = await energyController.updateStormWatchParticipation(
    energySiteId,
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


# Update Time-of-Use TOU Settings

```ts
async updateTimeOfUseTouSettings(
  energySiteId: string,
  body: TimeOfUseSettingsRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<GenericUpdateResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`TimeOfUseSettingsRequest`](../../doc/models/time-of-use-settings-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`GenericUpdateResponse`](../../doc/models/generic-update-response.md).

## Example Usage

```ts
const energySiteId = 'energy_site_id2';

const body: TimeOfUseSettingsRequest = {
  touSettings: {
  },
};

try {
  const response = await energyController.updateTimeOfUseTouSettings(
    energySiteId,
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


# Get User Products Vehicles Energy Sites

```ts
async getUserProductsVehiclesEnergySites(
  requestOptions?: RequestOptions
): Promise<ApiResponse<ProductsResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`ProductsResponse`](../../doc/models/products-response.md).

## Example Usage

```ts
try {
  const response = await energyController.getUserProductsVehiclesEnergySites();

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


# Get Site Information Assets Settings Features

```ts
async getSiteInformationAssetsSettingsFeatures(
  energySiteId: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<SiteInfoResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`SiteInfoResponse`](../../doc/models/site-info-response.md).

## Example Usage

```ts
const energySiteId = 'energy_site_id2';

try {
  const response = await energyController.getSiteInformationAssetsSettingsFeatures(energySiteId);

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

