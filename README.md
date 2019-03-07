# XMR-stak
XMR-Stak is a universal Stratum pool miner. This miner supports CPUs, AMD and NVIDIA GPUs and can be used to mine the crypto currencies Monero, Aeon and many more Cryptonight coins.
<h2>Features</h2>

* support all common backends (CPU/x86, AMD-GPU and NVIDIA-GPU)
* support all common OS (Linux, Windows and macOS)
* supports algorithm cryptonight for Monero (XMR) and cryptonight-light (AEON)
* easy to use
* guided start (no need to edit a config file for the first start)
* auto-configuration for each backend
* open source software (GPLv3)
* TLS support
* HTML statistics
* JSON API for monitoring
<h2>Necessary prerequisites for Windows</h2>

If the application does not start properly, please make sure that Visual Studio libraries are installed.
You can download them from https://go.microsoft.com/fwlink/?LinkId=746572

<h2>Anti-virus detection</h2>

All miners are detected as viruses. Please add the binary as an exception.


>**More information about miner you can find on official developer's  [github](https://github.com/fireice-uk/xmr-stak)**
  
<h2>Usage:</h2>

```
  -h, --help                 show this help
  -v, --version              show version number
  -V, --version-long         show long version number
  -c, --config FILE          common miner configuration file
  -C, --poolconf FILE        pool configuration file
  --noUAC                    disable the UAC dialog
  --benchmark BLOCKVERSION   ONLY do a benchmark and exit
  --benchwait WAIT_SEC             ... benchmark wait time
  --benchwork WORK_SEC             ... benchmark work time
  --noCPU                    disable the CPU miner backend
  --cpu FILE                 CPU backend miner config file
  --noAMD                    disable the AMD miner backend
  --noAMDCache               disable the AMD(OpenCL) cache for precompiled binaries
  --openCLVendor VENDOR      use OpenCL driver of VENDOR and devices [AMD,NVIDIA]
                             default: AMD
  --amd FILE                 AMD backend miner config file
  --noNVIDIA                 disable the NVIDIA miner backend
  --nvidia FILE              NVIDIA backend miner config file
  -i --httpd HTTP_PORT       HTTP interface port
```
The following options can be used for automatic start without a guided config,
If config exists then this pool will be top priority.
```
  -o, --url URL              pool url and port, e.g. pool.usxmrpool.com:3333
  -O, --tls-url URL          TLS pool url and port, e.g. pool.usxmrpool.com:10443
  -u, --user USERNAME        pool user name or wallet address
  -r, --rigid RIGID          rig identifier for pool-side statistics (needs pool support)
  -p, --pass PASSWD          pool password, in the most cases x or empty ""
  --use-nicehash             the pool should run in nicehash mode
  --currency NAME            currency to mine
```
<h2>Examples:</h2>

**For Windows**

```xmr-stak.exe -O xmr-eu1.nanopool.org:14433 -u YOUR_XMR_ADDRESS.YOUR_WORKER/YOUR_EMAIL --currency monero -i 0 -p "" -r ""```

**For Linux**

```./xmr-stak -O xmr-eu1.nanopool.org:14433 -u YOUR_XMR_ADDRESS.YOUR_WORKER/YOUR_EMAIL --currency monero -i 0 -p "" -r ""```


