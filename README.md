# Set up BIND 9 for DNS forwarding

## Simple Ex


## [Dynamic Update](https://bind9.readthedocs.io/en/v9.16.16/advanced.html#dynamic-update)

- https://datatracker.ietf.org/doc/html/rfc8945

### How to get

```sh
docker run --rm -it --entrypoint tsig-keygen internetsystemsconsortium/bind9:9.20 -a hmac-sha256
# key "tsig-key" {
#         algorithm hmac-sha256;
#         secret "GK3CEKSn6XCjUwOXS5DBoLg9pjlARinXCUYaQw50gGg=";
# };
```