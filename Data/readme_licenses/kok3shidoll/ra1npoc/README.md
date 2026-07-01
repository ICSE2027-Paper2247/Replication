# ra1npoc  
checkra1n dump and poc for iOS  
A tool for re-jailbreak devices jailbroken by checkra1n/odysseyra1n on iOS/iPadOS/macOS platforms.  

## Notes  
This is the demonstration code for running checkra1n on iOS, based on the Payload dumped from checkra1n 0.1337.x.  
Please do not run on normal devices.  


## Support  
### iOS device you want to Jailbreak  
| chip | name |
|---------|----------|
| S5L8960 | Apple A7 |
| T7000 | Apple A8 |
| T7001 | Apple A8X |
| S8000 | Apple A9 |
| S8003 | Apple A9 |
| S8001 | Apple A9X |
| T8010 | Apple A10 |
| T8011 | Apple A10X |
| T8012 | Apple T2 |
| T8015 | Apple A11 |


### Host-side device (device to run this software)  
- iOS 12 - 17  
    - via lightning to USB camera adapter  

- iOS 9 - 17  
    - via lightning to USB camera adapter + power supply  


## Build  
```
git submodule update --init --recursive
make
```


## Run  
```
Usage: ./ra1npoc15 [-r] [-hcyEsv] [-e <boot-args>] [-k <override_pongo>]
  mode:
	-r, --ra1npoc			    : start with legacy ra1npoc mode

  options:
	-c, --cleandfu			    : use clean dfu
	-y, --yolodfu			    : use download mode (yoloDFU)
	-E, --early-exit		    : exit after uploading Pongo
	-k, --override-pongo <path>	: override Pongo image
	-e, --extra-bootargs <args>	: replace bootargs
	-s, --safemode			    : enable safe mode
	-v, --verbose-boot		    : enable verbose boot

  help:
	-h, --help			: show usage
```
- `--ra1npoc` mode is compatible with the old build.  
- iOS 15+ only support boot pongoOS. Plase be sure to add the `-E` flag.  

### Example
- Boot pongoOS from DFU mode  
```
./ra1npoc15 -rE
```

- Boot any `pongoOS.bin` from DFU mode  
```
./ra1npoc15 -rEk <Pongo.bin>
```

- Jailbreak iOS 12 - 14 devices already jailbroken with checkra1n from Recovery mode  
```
./ra1npoc15 -rc
```


## How to use  
[ra1npoc - How to use](https://kok3shidoll.github.io/info/ra1npoc/usage.html)  


## Credit  
checkra1n team: checkra1n  
axi0mX: checkm8 exploit  

license: MIT  
