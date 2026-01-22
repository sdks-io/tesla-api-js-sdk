# Charging

Charging history, invoices, and session data

```ts
const chargingController = new ChargingController(client);
```

## Class Name

`ChargingController`

## Methods

* [Get Charging History](../../doc/controllers/charging.md#get-charging-history)
* [Get Charging Invoice](../../doc/controllers/charging.md#get-charging-invoice)
* [Get Charging Sessions](../../doc/controllers/charging.md#get-charging-sessions)


# Get Charging History

Returns the paginated charging history for the authenticated account.

```ts
async getChargingHistory(
  requestOptions?: RequestOptions
): Promise<ApiResponse<ChargingHistoryResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`ChargingHistoryResponse`](../../doc/models/charging-history-response.md).

## Example Usage

```ts
try {
  const response = await chargingController.getChargingHistory();

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


# Get Charging Invoice

Returns a charging invoice PDF for a charging session.

```ts
async getChargingInvoice(
  id: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<unknown>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `string` | Template, Required | Charging session invoice identifier |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type `unknown`.

## Example Usage

```ts
const id = 'id0';

try {
  const response = await chargingController.getChargingInvoice(id);

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


# Get Charging Sessions

Returns charging session information. Only available for business fleet owners.

```ts
async getChargingSessions(
  requestOptions?: RequestOptions
): Promise<ApiResponse<ChargingSessionsResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`ChargingSessionsResponse`](../../doc/models/charging-sessions-response.md).

## Example Usage

```ts
try {
  const response = await chargingController.getChargingSessions();

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

