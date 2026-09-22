# Go

The Go implementation provides the core admin experience for Go applications.
The current web adapter mounts go-polyadmin into Fiber.

## Install from Git

```bash
go get github.com/MagicRodri/go-polyadmin
```

## First steps

1. Embed `core.BaseModelAdmin` in a resource admin.
2. Implement the lifecycle methods against your storage.
3. Register the admin with `core.Admin`.
4. Mount it with the Fiber adapter.

Then continue with the [Go ModelAdmin guide](reference/model-admin.md) and the
[Go architecture guide](reference/architecture.md).