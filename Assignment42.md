# Read42

## Location

### Build location-aware apps

**One of the unique features of mobile applications is location awareness. Mobile users take their devices with them everywhere, and adding location awareness to your app offers users a more contextual experience. The location APIs available in Google Play services facilitate adding location awareness to your app with automated location tracking, wrong-side-of-the-street detection, geofencing, and activity recognition.**

### Request location permissions

**To protect user privacy, apps that use location services must request location permissions. When you request location permissions, follow the same best practices as you would for any other runtime permission. One important difference when it comes to location permissions is that the system includes multiple permissions related to location. Which permissions you request, and how you request them, depend on the location requirements for your app's use case.**

### Types of location access

- Foreground location - If your app contains a feature that shares or receives location information only once, or for a defined amount of time, then that feature requires foreground location access.

- Background location - An app requires background location access if a feature within the app constantly shares location with other users or uses the Geofencing API.

### Request location access at runtime

When a feature in your app needs location access, wait until the user interacts with the feature before making the permission request. This workflow follows the best practice of asking for runtime permissions in context

### Get the last known location

Using the Google Play services location APIs, your app can request the last known location of the user's device. In most cases, you are interested in the user's current location, which is usually equivalent to the last known location of the device.

Specifically, use the fused location provider to retrieve the device's last known location. The fused location provider is one of the location APIs in Google Play services. It manages the underlying location technology and provides a simple API so that you can specify requirements at a high level, like high accuracy or low power. It also optimizes the device's use of battery power.