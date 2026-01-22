# User

User account and settings endpoints

```ts
const userController = new UserController(client);
```

## Class Name

`UserController`

## Methods

* [Get Custom Feature Flags for a User](../../doc/controllers/user.md#get-custom-feature-flags-for-a-user)
* [Get Summary of a User S Account](../../doc/controllers/user.md#get-summary-of-a-user-s-account)
* [Get Active Orders for a User](../../doc/controllers/user.md#get-active-orders-for-a-user)
* [Get User S Region and Fleet-Api Base URL](../../doc/controllers/user.md#get-user-s-region-and-fleet-api-base-url)


# Get Custom Feature Flags for a User

```ts
async getCustomFeatureFlagsForAUser(
  requestOptions?: RequestOptions
): Promise<ApiResponse<BackupResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`BackupResponse`](../../doc/models/backup-response.md).

## Example Usage

```ts
try {
  const response = await userController.getCustomFeatureFlagsForAUser();

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


# Get Summary of a User S Account

```ts
async getSummaryOfAUserSAccount(
  requestOptions?: RequestOptions
): Promise<ApiResponse<MeResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`MeResponse`](../../doc/models/me-response.md).

## Example Usage

```ts
try {
  const response = await userController.getSummaryOfAUserSAccount();

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


# Get Active Orders for a User

```ts
async getActiveOrdersForAUser(
  requestOptions?: RequestOptions
): Promise<ApiResponse<OrdersResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`OrdersResponse`](../../doc/models/orders-response.md).

## Example Usage

```ts
try {
  const response = await userController.getActiveOrdersForAUser();

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


# Get User S Region and Fleet-Api Base URL

```ts
async getUserSRegionAndFleetApiBaseUrl(
  requestOptions?: RequestOptions
): Promise<ApiResponse<RegionResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`RegionResponse`](../../doc/models/region-response.md).

## Example Usage

```ts
try {
  const response = await userController.getUserSRegionAndFleetApiBaseUrl();

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

