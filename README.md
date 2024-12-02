# Install .NET SDK

Install current [LTS and STS versions](https://dotnet.microsoft.com/en-us/platform/support/policy/dotnet-core) of .NET SDK with optional support for preview version of .Net and End Of Life. Leverages the official [setup-dotnet action](https://github.com/actions/setup-dotnet) pre-configured specifically for the majority.

## Usage

To use this action in your GitHub repository, you can follow these steps:

```yaml
uses: maurosoft1973/dotnet-install@v1
```

### Inputs

```yaml
with:
  # Whether to include end of life versions of .NET SDK or not. Default is to exclude.
  includeEndOfFileVersion: 'false'
  # Whether to include preview versions of .NET SDK or not. Default is to exclude preview versions.
  includePreview: 'false'
```

### Outputs

This action has no outputs.

## Examples

### Install LTS e STS supported versions of .NET SDK

```yaml
steps:
  - name: Install .NET
    uses: maurosoft1973/dotnet-install@v1
```

### Install LTS,STS, end of life and preview versions of .NET SDK

```yaml
steps:
  - name: Install .NET
    uses: maurosoft1973/dotnet-install@v1
    with:
      includeEndOfFileVersion: 'true'
      includePreview: 'true'
```

## Contributing to Install .NET SDK

Contributions are welcome! 
Feel free to submit issues, feature requests, or pull requests to help improve this action.

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
