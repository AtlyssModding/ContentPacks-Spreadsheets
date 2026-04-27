- Information gathered by Vale (Discord: valefor_m) on April 26th.
- Reformatting complete by ZeinaKC (Discord: kittycatto) on April 28th.
### Test Machine Specs
```
Windows 11 (modified)
Intel(R) Core(TM) i5-14400F (2.50 GHz)
32.0 GB 6000MT/z RAM (2x 16GB)
Nvidia GeForce RTX 4070 (Driver 32.0.15.7680)
OS and Game on NVME SSD (Kingston SNVV2S1000G)
```
### Testing Method
1. Launched game via R2MM, started timer an same time as pressing start. 
2. Stopped timer when main menu appeared and was stable, checked RAM and CPU via Resource Monitor. 
3. Loaded single player, checked RAM and CPU via Resource monitor, FPS vis steam overlay. 
4. Alt+F4, waited until game was cleared from ram to start next test.

# Resource Usage & Test Results
## Regular Hosting
<details><summary><b>Vanilla</b></summary>

- **Time to Main Menu from start**
  - `17.27s`
  - `14.89s`
  - `14.19s`
  - `14.75s`
  - `14.71s`
- **RAM Usage: Main Menu**
  - `648MB`
  - `649MB`
  - `651MB`
  - `646MB`
  - `648MB`
- **CPU 60s Average: Main Menu**
  - `8.62%`
  - `8.18%`
  - `8.26%`
  - `8.2%`
  - `8.16%`
- **RAM Usage: Sanctum**
  - `818MB`
  - `848MB`
  - `840MB`
  - `841MB`
  - `839MB`
- **CPU 60s Average: Sanctum**
  - `10.15%`
  - `22.5%`
  - `16.07%`
  - `21.44%`
  - `18.35%`
- **60s Average FPS**
  - `144` X5
</details>

<details><summary><b>Vorny Modpack</b></summary>

Cold Start: First test hard hundreds of memory hard faults on starting, kept results but added an additional test to compensate.
- **BepInEx Console Initilize Time**
  - `3:09.691`
  - `0:44.318`
  - `0:39.750`
  - `0:41.527`
  - `0:43.943`
  - `0:42.086`
- **Time to Main Menu from start**
  - `3:28.56`
  - `0:57.12`
  - `0:53.02`
  - `0:55.8`
  - `0:56.61`
  - `0:54.69`
- **RAM Usage: Main Menu**
  - `3.1GB`
  - `3.12GB`
  - `3.13GB`
  - `3.17GB`
  - `3.2GB`
  - `3.28GB`
- **CPU 60s Average: Main Menu**
  - `12%`
  - `12.2%`
  - `11.89%`
  - `12.23%`
  - `12.66%`
  - `12.65%`
- **RAM Usage: Sanctum**
  - `3.17GB`
  - `3.26GB`
  - `3.27GB`
  - `3.32GB`
  - `3.35GB`
  - `3.29GB`
- **CPU 60s Average: Sanctum**
  - `25.18%`
  - `17.73%`
  - `24%`
  - `18.34%`
  - `20.89%`
  - `17.83%`
- **60s Average FPS**
  - `95`
  - `109`
  - `104`
  - `92`
  - `103`
  - `106`
</details>

<details><summary><b>Vorny Hostpack</b></summary>

Cold Start: First test had hundreds of memory hard faults, added 6th test to compensate.\
FPS seems a lot more stable too, highs are higher but lows are not nearly as low as base Vorny pack, didnt notice until 4th test so no hard data collected.
- **BepInEx Console Initilize Time**
  - `2:31.926`
  - `0:34.151`
  - `0:34.305`
  - `0:33.405`
  - `0:32.826`
  - `0:33.961`
- **Time to Main Menu from start**
  - `2:53.27`
  - `0:49.22`
  - `0:48.5`
  - `0:46.57`
  - `0:45.63`
  - `0:46.73`
- **RAM Usage: Main Menu
  - `3.04GB`
  - `2.944GB`
  - `2.89GB`
  - `2.91GB`
  - `2.93GB`
  - `2.87GB`
- **CPU 60s Average: Main Menu**
  - `13.56%`
  - `14.00%`
  - `12.75%`
  - `13.49%`
  - `14.06%`
  - `13.13%`
- **RAM Usage: Sanctum**
  - `3.19GB`
  - `3.09GB`
  - `3.04GB`
  - `3.06GB`
  - `3.07GB`
  - `3.03GB`
- **CPU 60s Average: Sanctum**
  - `19.21%`
  - `18.67%`
  - `18.77%`
  - `18.91%`
  - `18.42%`
  - `18.48%`
- **60s Average FPS**
  - `113`
  - `115`
  - `114`
  - `113`
  - `114`
  - `113`
</details>

#
## Headless Hosting
Headless loads Sanctum and places a ghost character there so CPU/RAM usage is comprable to above Sanctum results.\
Headless ARGs: `-batchmode -nographics -server -hostsave 0 -password "Pass"`
<details><summary><b>Vorny Modpack</b></summary>

Cold start: First test had a lot of memory hard faults added 6th test to compensate. Only about half as much as the other cold starts.
- BepInEx Console Initilize Time
  - `1:44.222`
  - `0:39.596`
  - `0:39.183`
  - `0:38.889`
  - `0:38.697`
  - `0:39.071`
- **Time for server to go live from start**
  - `2:12.31`
  - `0:59.61`
  - `0:58.98`
  - `0:58.78`
  - `0:58.31`
  - `0:58.89`
- **RAM Usage 60s Average**
  - `2.55GB`
  - `2.61GB`
  - `2.63GB`
  - `2.55GB`
  - `2.60GB`
  - `2.60GB`
- **CPU Usage**
  - `9.55%`
  - `9.82%`
  - `10.29%`
  - `9.86%`
  - `9.19%`
  - `9.73%`
</details>

<details><summary><b>Vorny Hostpack</b></summary>

Cold start first trail so 6 tests intstead.
- **BepInEx Console Initilize Time**
  - `0:30.912`
  - `0:31.392`
  - `0:30.633`
  - `0:31.213`
  - `0:31.538`
- **Time for server to go live from start**
  - `0:52.2`
  - `0:51.74`
  - `0:50.76`
  - `0:51.37`
  - `0:52.35`
- **RAM Usage 60s Average**
  - `2.39GB`
  - `2.37GB`
  - `2.38GB`
  - `2.37GB`
  - `2.38GB`
- **CPU Usage**
  - `8.61%`
  - `10.55%`
  - `9.57%`
  - `9.06%`
  - `8.88%`
</details>

#
## The Brutaliser™
Brutaliser removes all `.PNG`, `.MP3`, `.OGG`, `.WAV`, `.LUA`, `.GLB` (3D Meshes), Skins, and more leaving files in the most minimal state to operate stabily as possible. Removes mod specific files not in use like CustomQuest files and .PropBundles.

<details><summary><b>Brutalised™ Vorny Modpack</b></summary>

ModAudio prevented launching while Brutalised™ so the mod was removed.
- **BepInEx Console Initilize Time**
  - `0:11.674`
  - `0:11.758`
  - `0:11.917`
  - `0:12.567`
  - `0:12.171`
- **Time for server to go live from start**
  - `0:31.74`
  - `0:31.46`
  - `0:31.82`
  - `0:32.75`
  - `0:32.59`
- **RAM Usage 60s Average**
  - `828MB`
  - `812MB`
  - `808MB`
  - `816MB`
  - `813MB`
- **CPU Usage**
  - `7.1%`
  - `6.92%`
  - `7.1%`
  - `7.16%`
  - `7.08%`
</details>

<details><summary><b>Brutalised™ Vorny Hostpack</b></summary>

- **BepInEx Console Initilize Time**
  - `0:50.519`
  - `0:10.632`
  - `0:10.476`
  - `0:10.230`
  - `0:09.981`
  - `0:09.948`
- **Time for server to go live from start**
  - `1:18.94`
  - `0:30.66`
  - `0:30.49`
  - `0:34.61` (Took longer from pressing "Start" for the console to show up.)
  - `0:33.97` (Took longer from pressing "Start" for the console to show up.)
  - `0:30.37`
- **RAM Usage 60s Average**
  - `784MB`
  - `792MB`
  - `792MB`
  - `777MB`
  - `778MB`
  - `778MB`
- **CPU Usage**
  - `6.72%`
  - `6.81%`
  - `6.51%`
  - `7.3%`
  - `6.79%`
  - `6.73%`
</details>
