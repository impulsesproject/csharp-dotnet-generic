FROM mcr.microsoft.com/devcontainers/dotnet:1-8.0-bookworm

# refresh
RUN apt update -y && apt upgrade -y

# refresh .NET toolchain
RUN dotnet tool update --all
RUN dotnet workload update

WORKDIR /workspace
COPY .. .

USER root