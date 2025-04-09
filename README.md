# Open Device Partnership's Rust Crate Audits

Open Device Partnership (ODP) uses cargo vet to audit third party Rust dependencies.

This repository serves as the centralized audit repository for all ODP repositories.
To import audits from this repository into your cargo vet instance, add the following lines to your config.toml:

```
[imports.OpenDevicePartnership]
url = "https://raw.githubusercontent.com/OpenDevicePartnership/rust-crate-audits/refs/heads/main/audits.toml"
```

## Aggregation
Repositories in ODP might have their own sets of audits. This repository also aggregates all those audits to provide an overview of dependencies and audits across ODP.

For crates that are being used in multiple repositories, it's preferred to add the audits to this repository directly and import the audits to individual repositories. This reduces the overhead of each project to conduct its own set of audits for shared dependencies.

## License

This project is licensed under the [MIT License](LICENSE).