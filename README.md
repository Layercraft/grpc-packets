# GRPC-Packets Documentation from Layercraft.io Version 0.0.1

## Introduction

Uses Buf [Buf](https://buf.build/) for Building and Style Check (Minimal).




## Style Guide

### Standard file formating

- Keep the line length to 80 characters.
- Use an indent of 2 spaces.
- Prefer the use of double quotes for strings.

#### File Structure

1. License header (if applicable)
2. File overview
3. Syntax
4. Package
5. Imports (sorted)
6. File options
7. Everything else

#### File Naming
{package_name}/{file_name}.proto

Example: `package_name` is `auth` and `file_name` is `authplayerservice`.

#### Package Naming
layercraft/api/{package_name}

Example: `package_name` is `auth`.

```protobuf
package layercraft.api.auth;
```


#### Service Naming

If your .proto defines an RPC service, you should use CamelCase (with an initial capital) for both the service name and any RPC method names:

{service_name}

Example: `service_name` is `AuthPlayerService`.

```protobuf
service FooService {
  rpc GetSomething(GetSomethingRequest) returns (GetSomethingResponse);
  rpc ListSomething(ListSomethingRequest) returns (ListSomethingResponse);
}
```


### Syntax

#### Repeated fields
Use pluralized names for repeated fields.

```protobuf
repeated string keys = 1;
repeated MyMessage accounts = 17;
```

#### Enums
Use CamelCase (with an initial capital) for enum type names and CAPITALS_WITH_UNDERSCORES for value names.

```protobuf
enum FooBar {
    FOO_BAR_UNSPECIFIED = 0;
    FOO_BAR_FIRST_VALUE = 1;
    FOO_BAR_SECOND_VALUE = 2;
}
```



