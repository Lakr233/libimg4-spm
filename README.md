# libimg4-spm

Pure Swift library for parsing and manipulating Apple IMG4/IM4P firmware containers.

## Features

- ASN.1 DER parsing for IMG4, IM4P, IM4M containers
- Payload extraction with LZSS/LZFSE decompression
- AES-256-CBC decryption (CommonCrypto) and signature validation (Security.framework)
- Container construction and modification
- All Apple platforms supported (macOS, iOS, tvOS, watchOS, visionOS)

## Install

Add to your `Package.swift`:

```swift
dependencies: [
    .package(url: "https://github.com/Lakr233/libimg4-spm.git", from: "1.0.0"),
],
targets: [
    .target(
        name: "YourTarget",
        dependencies: [
            .product(name: "Img4tool", package: "libimg4-spm"),
        ]
    ),
]
```

## License

MIT
