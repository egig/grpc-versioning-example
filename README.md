# README

This Repo created to test Go implementation of GRPC Versioning using the package.

Reference: https://docs.microsoft.com/en-us/aspnet/core/grpc/versioning?view=aspnetcore-3.1

This is how I generate the GO PB Interface:
```shell
cd helloworld
protoc -I. --go_out=plugins=grpc:.  helloworld.proto
```
and
```
cd helloworldv2
protoc -I. --go_out=plugins=grpc:.  helloworldv2.proto
```