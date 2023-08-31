# ARCore Barcode Detection

An [ARCore](https://developers.google.com/ar) sample based on  [https://github.com/googlesamples/arcore-ml-sample.git](https://github.com/googlesamples/arcore-ml-sample.git), demonstrates how to utilize Dynamsoft Barcode Reader to detect 1D and 2D barcodes and
create anchors for detected barcodes in the AR scene.

## Prerequisites
- An ARCore compatible device running [Google Play Services for AR](https://play.google.com/store/apps/details?id=com.google.ar.core) (ARCore) 1.24 or later
- Android Studio 4.1 or later

## Getting Started
1. Request a license key for Dynamsoft Barcode Reader from [here](https://www.dynamsoft.com/customer/license/trialLicense?product=dbr&package=android&utm_source=github).
2. Update the license key in `MainActivity.kt`.
    
    ```kotlin
    BarcodeReader.initLicense("LICENSE-KEY") { isSuccessful, e ->
      runOnUiThread {
        if (!isSuccessful) {
          e.printStackTrace()
          Log.e(TAG, "Failed to verify the license: $e")
        }
      }
    }
    ```
3. Build and run the sample.
 



