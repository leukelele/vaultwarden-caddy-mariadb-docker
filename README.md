# vaultwarden

Vaultwarden is a reimplementation of Bitwarden in the Rust programming language, designed to offer greater flexibility. Bitwarden's self-hosting option is distributed in a containerized form, which is essentially a one-size-fits-all solution and may not include all its features immediately out of the box, though the overall service and support is reportedly excellent. Vaultwarden, on the other hand, allows for more customization in installation and has less overhead.[^1] While Bitwarden, built on Microsoft's tech stack with .NET and MySQL, requires around 2 GB of memory, Vaultwarden reportedly uses only about 60 MB.[^2] However, unlike Bitwarden, Vaultwarden does not include a reverse proxy by default, requiring manual setup for that component.

## setup dependencies

This vaultwarden Docker instance is installed along with a [plugin of Caddy](https://github.com/lucaslorentz/caddy-docker-proxy) that allows Caddy to be used as a reverse proxy for the Docker containers. In addition, the vaultwarden uses MariaDB as a backend.

[^1]: This is stated in the [vaultwarden repository](https://github.com/dani-garcia/vaultwarden)
[^2]: [This youtube](https://www.youtube.com/watch?v=xdiUoXwjahk) states as such; although, I have not verified the correctness of the information.
