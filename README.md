![Capture d’écran 2024-03-03 à 18 37 48](https://github.com/EloWord/raveos/assets/155255722/07ece88c-1e1a-47f9-b2c6-64b2b0e11113)

### RaveOs

Version 1.8.6

- Enhanced support for QUBIC GPU and CPU Mining on RaveOS 
*since RaveOS does not support CPU mining, I employed a clever workaround to display CPU it/s as a 2nd box under GPU#0*
- Support for QUBIC GPU Only mining on Raveos

Use now in "custom mining": https://github.com/EloWord/raveos/releases/download/v1.8.6/eloword-v1.8.6.zip

<br>

## :star2: Support My Work and Contribute to its Growth :star2:

If you appreciate my work and want to contribute to its ongoing development, consider leaving a tip. Every contribution, big or small, makes a huge difference and motivates me to continue creating and improving.

- **To support me, use Qubic:** `QYGPXYBKNIDKVFFUWMMJFPWNMPXAPAVFEFEJOTUEIALMQZEFNKXOUUQEWBOM`

*Support received since this version: 620,240,488 Qubic - Thank you for your future support!*

[<img src="https://github.com/EloWord/hiveos/assets/155255722/dedb996d-c517-4059-a55a-d9adea9a21f1" alt="discord" width="200">](https://discord.gg/bWHcuuyQBf)

Thank you for being part of this journey!
<br>

## :warning: Mandatory Installation Instructions
- The CPU where you run the Client must support AVX2 or AVX512 CPU instructions
`cat /proc/cpuinfo | grep avx2`(check if `avx2` is in the result)
- RAM >= 16Go improves CPU it/s
- Do not overload your CPUs with threads, instead, aim to find the sweetpoint

*Only NVIDIA GPU compatible*
<br>

## :wrench: Settings

- it's an all-in-one miner (CPU+GPU / GPU only), check out settings below for seamless setup

- Recommended GPU overclocks :
**Medium**
3000 series ```nvidia-smi -lmc 5001 && nvidia-smi -lgc 1500```
4000 series ```nvidia-smi -lmc 5001 && nvidia-smi -lgc 2400```
**High**
3000 series ```nvidia-smi -lmc 5001 && nvidia-smi -lgc 1600```
4000 series ```nvidia-smi -lmc 7000 && nvidia-smi -lgc 2900```
<br>

- Extra config arguments Box (options):

| Setting | Description |
| ---- | --------- |
| ```"accessToken":``` | This is you personal JWT Token which you can obtain from the Control Panel at qubic.li |
| ```"payoutId":``` |  This is the ID you want to get token payout for your found solutions. |
|  ```"overwrites": {"AVX512": false}``` |  Disable AVX512 and enforce AVX2 (AVX Intel CPU not working) |
| ```"overwrites": {"SKYLAKE": true}```  |  Enforce SKYLAKE (AVX Intel CPU not working)  |
<br>

## ✈️ Rave OS Settings


#### I/ Download and *Add* custom zip file here: https://github.com/EloWord/raveos/releases/download/v1.8.6/eloword-v1.8.6.zip

![Capture d’écran 2024-03-03 à 20 36 09](https://github.com/EloWord/raveos/assets/155255722/928d8aaa-2da9-4223-8315-44ba2b38c9ce)


#### II/ Add Wallet 
![Capture d’écran 2024-03-03 à 21 46 07](https://github.com/EloWord/raveos/assets/155255722/508e5ca7-fe90-4916-9155-296ab4232cd7)

#### III/ Set Miner Param
- *** GPU + CPU Mining ***

```
"amountOfThreads":12
"accessToken":"YOUROWNTOKEN"
```
![Capture d’écran 2024-03-03 à 20 43 40](https://github.com/EloWord/raveos/assets/155255722/deab08e2-58ef-43da-b71b-42093e3da154) 

- *** GPU Only Mining ***

```
"accessToken":"YOUROWNTOKEN"
```
![Capture d’écran 2024-03-03 à 20 43 21](https://github.com/EloWord/raveos/assets/155255722/7a60c27d-a750-4417-b2e0-91d12dcb1a42)

#### IV Run Miner

![Capture d’écran 2024-03-03 à 21 53 31](https://github.com/EloWord/raveos/assets/155255722/fdbff527-0731-4b3f-9044-6e8bb55fae73)
