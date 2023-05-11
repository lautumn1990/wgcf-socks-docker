# wgcf-socks-docker

a docker compose file for wgcf-socks

## Usage

```bash
# use root
git clone https://github.com/lautumn1990/wgcf-socks-docker
cd wgcf-socks-docker

docker-compose up -d

# check and test
curl --proxy socks5h://127.0.0.1:1080 https://www.cloudflare.com/cdn-cgi/trace
```

custom license and endpoint

```bash
# if you have warp license key
mkdir wgcf
echo "your_key" > wgcf/custom-wgcf-license.conf

# like 
# echo "3KOY1u56-pf2S09g7-xxxxxxx" > wgcf/custom-wgcf-license.conf


# if you have a custom endpoint
echo "your_endpoint" > wgcf/custom-wgcf-endpoint.conf

# like
# echo "162.159.195.168:5279" > wgcf/custom-wgcf-endpoint.conf

```

## reference

- [Neilpang/wgcf-docker](https://github.com/Neilpang/wgcf-docker)
- [Mon-ius/Docker-Warp-Socks](https://github.com/Mon-ius/Docker-Warp-Socks)
- [vimagick/dante](https://hub.docker.com/r/vimagick/dante/)
- [shturman/dante](https://hub.docker.com/r/shturman/dante)