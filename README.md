# Laravel API Response Snippet

## Description

This VS Code extension provides a handy snippet for Laravel API response handling. The snippet is designed to streamline the process of managing API responses by inserting a standardized code template that handles execution time, exception management, and API response generation.

## Snippet Details

**Prefix:** `api-laravel`

**Snippet Content:**
```php
    $this->api->time();
    try {
        $data = null;
    } catch (\Exception $e) {
        $data = $e;
    }
    return $this->api->data($data)->generate();
```
**Functions:**

- **$this->api->time():** Logs the API execution time.
- **try-catch block:** Handles the main process and any exceptions that occur.
  - **$data = null:** Initializes the data variable.
  - **catch (\Exception $e):** Catches exceptions and stores exception information.
- **return $this->api->data($data)->generate():** Generates the API response based on the data.

## Installation

To install the package, use the following link: [laravel-api-core-response-generator](https://packagist.org/packages/krozamdev/laravel-core-response).
