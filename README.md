# Meet Protocol

Protocol buffer definitions and generated Go/JS code for the Meet conferencing system.

## Overview

This package contains:

- **Proto source files** (`proto_files/`) — Protocol buffer definitions for all API messages
- **Generated Go code** (`plugnmeet/`) — Go structs and validation helpers
- **Generated JS code** (`js/`) — TypeScript/JavaScript package for client-side usage

## Building

### Go

The generated Go code is committed directly. To regenerate:

```bash
buf generate
```

### JavaScript

```bash
cd js
pnpm install
pnpm run build
```

## Usage

### Go

```go
import "github.com/silentlamp/zenleader-protocol/plugnmeet"
```

### JavaScript

```bash
pnpm add plugnmeet-protocol-js
```

## License

MIT
