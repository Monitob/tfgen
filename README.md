# tfgen - Terraform Configuration Generator

`tfgen` is a command-line utility for generating Terraform configuration files for managing cloud resources. It allows you to create Terraform configurations for AWS and Scaleway providers, enabling you to define and provision infrastructure resources in a declarative and repeatable way.

## Installation

Before using `tfgen`, make sure you have Go installed on your system. You can build the CLI as follows:

```bash
go build tfgen.go
```

## Usage

You can use `tfgen` to generate Terraform configurations for both AWS and Scaleway providers. It provides a `generate` command with several flags to customize the generated configuration.

### Generate Terraform Configuration

To generate a Terraform configuration, use the `generate` command. Here's the basic usage:

```bash
./tfgen generate [flags]
```

**Flags:**

- `--aws-region`: Specifies the AWS region to be used in the generated AWS provider block. The default is `us-west-2`.
- `--scaleway-access-key`: The Scaleway access key required for the Scaleway provider configuration.
- `--scaleway-secret-key`: The Scaleway secret key required for the Scaleway provider configuration.

### Example

Generate a Terraform configuration with AWS and Scaleway providers:

```bash
./tfgen generate --aws-region us-east-1 --scaleway-access-key YOUR_ACCESS_KEY --scaleway-secret-key YOUR_SECRET_KEY
```

**Note:** You can modify the generated Terraform configuration to include more resources and further customize it according to your specific infrastructure requirements.

## Use Case

`tfgen` is useful for quickly generating Terraform configurations for managing cloud infrastructure on both AWS and Scaleway, making it easier to define and deploy cloud resources with Terraform's infrastructure as code approach.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

You can copy and paste this Markdown content into your project's README.md file.
