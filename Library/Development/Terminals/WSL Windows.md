

- [Developing in WSL](https://code.visualstudio.com/docs/remote/wsl#_i-see-eaccess-permission-denied-error-trying-to-rename-a-folder-in-the-open-workspace)
- [Port Query](https://www.microsoft.com/en-us/download/confirmation.aspx?id=24009)
- [Images](https://docs.microsoft.com/en-us/windows/wsl/install-manual)
- [Update Assistant](https://www.microsoft.com/nl-nl/software-download/windows10)
- [Linux kernel update package](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi)
- [Sysinternals Utilities Index](https://docs.microsoft.com/en-us/sysinternals/downloads/)
- [Autoruns](https://docs.microsoft.com/en-us/sysinternals/downloads/autoruns)
- [TCPView](https://docs.microsoft.com/en-us/sysinternals/downloads/tcpview)
- [PsTools](https://docs.microsoft.com/en-us/sysinternals/downloads/pstools)
- [PipeList](https://docs.microsoft.com/en-us/sysinternals/downloads/pipelist)

- C:\Users\User\AppData\Local\Packages\CanonicalGroupLimited.Ubuntu20.04onWindows_79

```
wslconfig /s Ubuntu-20.04
wslconfig /l
wsl (If a WSL2 distro is your default distro)
wsl --set-version <Distro> 2,
wsl --set-default-version 2
wsl --import and wsl --export targeting WSL2
wsl -u root
wsl.exe --export Ubuntu-20.04 X:\Ubuntu20.04\Ubuntu20.04.tar
wsl.exe --import Ubuntu-20.04 X:\Ubuntu20.04\Ubuntu20.04.tar
wsl --distribution <DistributionName>
wsl.exe --unregister <DistributionName>
wsl -t Ubuntu
```

### Creating a Docker image from a WSL instance

```
wsl --list
Debian (Standard)
Alpine
Ubuntu
wsl --export Alpine alpine.tar
wsl --export Alpine alpine.tar && gzip -9 alpine.tar
docker import alpine.tar alpine:wsl
docker import -c "CMD /bin/sh" -c "ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin" alpine.tar alpine:wsl
docker run -it alpine:wsl
docker tag alpine:wsl d3vone/alpine:wsl
docker login -u d3vone
docker push d3vone/alpine:wsl
docker run -it d3vone/alpine:wsl
```