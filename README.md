# Set up BIND 9 for DNS forwarding

## Simple Ex


## [Dynamic Update](https://bind9.readthedocs.io/en/v9.16.16/advanced.html#dynamic-update)

- https://datatracker.ietf.org/doc/html/rfc8945

### How to get

Execute a command inside a container

```sh
runner@dns-server:~$ docker exec -it bind9 sh -c "tsig-keygen -a hmac-sha256"
# key "tsig-key" {
#         algorithm hmac-sha256;
#         secret "8+WxElMp7R28wwPg7J4tekaLLhBzknipZQjKhKwuru0=";
# };
```