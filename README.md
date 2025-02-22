# capacitor-flash

Switch the Flashlight / Torch of your device.

## Install

```bash
npm install capacitor-flash
npx cap sync
```

## iOS

Works out of the box

## Android

1. Declare permissions in your app's `AndroidManifest.xml` file

```xml
<!-- Permissions: Allows access to flashlight -->
<uses-permission android:name="android.permission.CAMERA" android:maxSdkVersion="23" />
<uses-permission android:name="android.permission.FLASHLIGHT" />

<!-- Actual Hardware Features Used-->
<uses-feature android:name="android.hardware.camera.flash" android:required="true" />
```

## API

<docgen-index>

* [`isAvailable()`](#isavailable)
* [`switchOn(...)`](#switchon)
* [`switchOff()`](#switchoff)
* [`isSwitchedOn()`](#isswitchedon)
* [`toggle()`](#toggle)

</docgen-index>

<docgen-api>
<!--Update the source file JSDoc comments and rerun docgen to update the docs below-->

### isAvailable()

```typescript
isAvailable() => Promise<{ value: boolean; }>
```

Checks if flashlight is available

**Returns:** <code>Promise&lt;{ value: boolean; }&gt;</code>

--------------------


### switchOn(...)

```typescript
switchOn(options: { intensity?: number; }) => Promise<void>
```

Turns the flashlight on

| Param         | Type                                 |
| ------------- | ------------------------------------ |
| **`options`** | <code>{ intensity?: number; }</code> |

--------------------


### switchOff()

```typescript
switchOff() => Promise<void>
```

Turns the flashlight off

--------------------


### isSwitchedOn()

```typescript
isSwitchedOn() => Promise<{ value: boolean; }>
```

Checks if the flashlight is turned on or off

**Returns:** <code>Promise&lt;{ value: boolean; }&gt;</code>

--------------------


### toggle()

```typescript
toggle() => Promise<{ value: boolean; }>
```

Toggle the flashlight

**Returns:** <code>Promise&lt;{ value: boolean; }&gt;</code>

--------------------

</docgen-api>
