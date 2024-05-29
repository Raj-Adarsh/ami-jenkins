# Jenkins Master AMI Builder

This project uses Packer to build an Amazon Machine Image (AMI) with a Jenkins Server.

## Prerequisites

- Packer
- AWS Account

## Configuration

The Packer configuration is defined in the `packer/packer.pkr.hcl` file. 

The configuration includes the following main sections:

- `source`: Defines the type of machine image to be built and the details of the build process.
- `build`: Defines the provisioners that install and configure software within running machines prior to turning them into machine images.

## Usage

1. Set your AWS credentials in your environment or AWS credentials file.
2. Update the `packer/packer.pkr.hcl` file with your specific values.
3. Run `packer build packer/packer.pkr.hcl` to start the build process.

## Built With

- [Packer](https://www.packer.io/) - Open source tool for creating identical machine images for multiple platforms from a single source configuration.
- 
