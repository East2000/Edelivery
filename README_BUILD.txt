E-DELIVER NATIVE ANDROID PROJECT

This is the native Android project for the rider app.

Included:
- CameraX + Google ML Kit QR/barcode scanning
- Android GPS permission and live rider location
- OpenStreetMap via osmdroid (no Google Maps API key)
- Parcel list
- Priority-first nearest-neighbor route ordering
- Map pins
- Next Delivery

LIMITATIONS OF THIS FIRST BUILD:
- It does not automatically obtain a buyer address from an SPX tracking number.
  That requires an authorized SPX API/data source or rider-entered address.
- For parcels without coordinates, tap the map to assign a pin.
- Routing is a simple nearest-neighbor heuristic, not a traffic-aware turn-by-turn
  route. A later version can integrate an appropriate routing provider.
- This package is source code. It is NOT a compiled APK.

HOW TO BUILD APK:
1. Open the folder in Android Studio.
2. Let Gradle sync.
3. Build > Build APK(s).
4. Install the generated app-debug.apk on Android.

The project uses public OpenStreetMap tiles through osmdroid. Production use
must comply with the tile provider's usage policy and attribution requirements.
