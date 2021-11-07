# GRPC-Packets Documentation from Layercraft.io Version 0.0.1

## Introduction

Uses Buf [Buf](https://buf.build/) for Building and Style Check (Minimal).


## Style Guide

-> Google Style Guide (https://developers.google.com/protocol-buffers/docs/style)


### File Header


Example:
´´´protobuf

syntax = "proto3";

package layercraft.api.auth;

option java_multiple_files = true;
option java_package = "io.layercraft.api.auth";

option go_package = "layercraft/api/auth";

´´´


