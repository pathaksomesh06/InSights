# InSights - Intune Management App

Welcome to **InSights**, the ultimate Intune management app designed to simplify and enhance your device management experience. With InSights, you can seamlessly manage your Intune tenant and access a wealth of information about your configuration profiles, apps, and policies. This powerful app provides a comprehensive read-only view of your Intune environment with plans for future updates that will include editing and updating capabilities.


## Features

- **Tenant Information**
  - View detailed information about your Intune tenant.

- **Policy Management**
  - Access all configuration and compliance policies within your tenant.

- **App Management**
  - See all managed apps deployed within your tenant.

- **Device Management**
  - Get detailed information about all managed devices.

- **App Configuration (App & Device)**
  - View app and device configuration profiles.

- **App Protection**
  - Access app protection policies.

- **Apple Enrollment Types**
  - View Apple enrollment types configured in your tenant.

- **AutoPilot**
  - Manage AutoPilot profiles.

- **Endpoint Security**
  - View endpoint security policies.

- **Enrollment Restrictions**
  - Check enrollment restrictions applied.

- **Enrollment Status Page**
  - View the enrollment status page configurations.

- **Feature Updates**
  - Access feature update configurations.

- **iOS/iPadOS Update Policies**
  - View update policies for iOS/iPadOS devices.

- **Scripts & Remediations**
  - Manage scripts and remediations.

- **Shell Scripts (macOS)**
  - Access macOS shell scripts.

- **Custom Attributes (macOS)**
  - View custom attributes for macOS devices.

- **macOS Update Policies**
  - Check update policies for macOS.

- **Antivirus Policies**
  - Access antivirus policies.

- **Keychain Storage**
  - The app securely stores the client ID in the keychain for seamless authentication.

- **Log Out**
  - Easy log out to ensure secure access management.

## Upcoming Features

- **Edit and Update Policies**
- **App Deployment**
- **Configuration Profile Updates**

## API Permissions Required

To use the InSights app, ensure that the following API permissions are granted in your Azure app registration:

- `DeviceManagementManagedDevices.Read.All`
- `DeviceManagementConfiguration.Read.All`
- `DeviceManagementApps.Read.All`
- `Directory.Read.All`
- `User.Read`
- `Device.Read`
- `Group.Read.All`

## App Registration Setup

1. **Register the App in Azure:**
   - Go to the [Azure portal](https://portal.azure.com/) and navigate to **Azure Active Directory** > **App registrations** > **New registration**.
   - Enter the name for your app, such as "InSights".
   - Enter the Redirect URI: `https://login.microsoftonline.com/common/oauth2/nativeclient`.

2. **API Permissions:**
   - Go to your app registration and navigate to **API permissions** > **Add a permission**.
   - Select **Microsoft Graph** and then **Delegated permissions**.
   - Add the following permissions:
     - `DeviceManagementManagedDevices.Read.All`
     - `DeviceManagementConfiguration.Read.All`
     - `DeviceManagementApps.Read.All`
     - `Directory.Read.All`
     - `User.Read`
     - `Device.Read`
     - `Group.Read.All`
   - Grant admin consent for the required permissions.

3. **Using the App:**
   - Upon first launch, you will be prompted to enter your **Client ID**.
   - The app will securely store the Client ID in the keychain for seamless future authentication.

## Installation

1. Go to the [Releases](https://github.com/pathaksomesh06/InSights/releases) page.
2. Download the latest release for your operating system.
3. Follow the installation instructions provided with the release.