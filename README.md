# iso4217_protobuf
ISO 4217 Currency codes for Protocol Buffers ( proto2 / proto3 )

# Version Compatibility
Enums are not compatible between proto2 and proto3. The default is proto3 but you can simply switch `syntax = "proto3"` for `syntax = "proto2"` if you need to. The rest of the file is compatible with both.

# Differences to ISO 4217
- `XXX = 999` (No currency) has been changed to `XXX = 0` because proto3 requires the default to be 0 and XXX may not be redeclared with `XXX = 999`
- `XTS = 963` *"Codes specifically reserved for testing purposes"* has been commented out by default
