#

## Instalação brave debian 9

```bash
echo "deb [arch=amd64] https://brave-browser-apt-release.s3.brave.com/ stretch main" | sudo tee /etc/apt/sources.list.d/brave-browser-release-stretch.list
sudo apt update
sudo apt install brave-keyring brave-browser
```

    - Rodar o seguinte comando caso der o erro: No usable sandbox! You probably need to enable user namespaces in your kernel

```bash
sudo echo 'kernel.unprivileged_userns_clone=1' > /etc/sysctl.d/00-local-userns.conf
```
