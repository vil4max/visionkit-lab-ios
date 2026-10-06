# VisionKit Lab

iOS demo of the [VisionKit](https://developer.apple.com/documentation/visionkit) camera and image interfaces for recognizing text, barcodes, and documents on device.

## What it demonstrates

| Screen | API |
|--------|-----|
| Live Text | `ImageAnalyzer` + `ImageAnalysisInteraction` |
| Data Scanner | `DataScannerViewController` (live text and barcodes) |
| Document Camera | `VNDocumentCameraViewController` (multi-page scan, preview, save) |

Details of each surface are in [docs/architecture.md](docs/architecture.md).

## Requirements

- Xcode 16 or later, iOS 17+ deployment target
- Swift 6, SwiftUI, Swift Testing
- A physical device for Data Scanner and Document Camera; Live Text works with library photos on supported devices

## Build and run

1. Open `ios/VisionLab.xcodeproj` in Xcode.
2. Select the `VisionLab` scheme and a device (or a simulator for the Live Text screen).
3. Set your own signing team and bundle identifier under Signing & Capabilities, then run.

The project is also described in `ios/project.yml` for [XcodeGen](https://github.com/yonaskolb/XcodeGen).

Run the unit tests with the `VisionLab` scheme (Product > Test).

## Screenshots

| Home | Live Text |
|------|-----------|
| ![VisionKit Lab home](Screenshots/home.png) | ![Live Text on a document photo](Screenshots/live-text.png) |

| Data Scanner | Document Camera |
|--------------|-----------------|
| ![Data Scanner camera view](Screenshots/data-scanner.png) | ![VisionKit document camera](Screenshots/document-camera.png) |
