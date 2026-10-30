# MEDIA\_UTILS\_LITE<a name="EN-US_TOPIC_0000001127127417"></a>

- [MEDIA\_UTILS\_LITE<a name="EN-US_TOPIC_0000001127127417"></a>](#media_utils_lite)
  - [Introduction<a name="section11660541593"></a>](#introduction)
  - [Directory Structure<a name="section8685144625320"></a>](#directory-structure)
  - [Usage<a name="section1648194512427"></a>](#usage)
  - [Constraints<a name="section161941989596"></a>](#constraints)
  - [Changes in This Release<a name="section_changes_en"></a>](#changes-in-this-release)
  - [Repositories Involved<a name="section105062051111614"></a>](#repositories-involved)

## Introduction<a name="section11660541593"></a>

This repository defines common information such as media error codes and data types required for audio and video recording and playback.

Data types

-   **SourceType**: type of the media source to play
-   **BufferFlags**: flags of the data carried in the buffer
-   **AudioSourceType**: enumeration of audio input source types
-   **AudioCodecFormat**: enumeration of audio data formats
-   **AudioStreamType**: enumeration of audio stream types
-   **AudioBitWidth**: enumeration of sampling bit width

The following table lists the error codes.

<a name="table7158151314620"></a>
<table><thead align="left"><tr id="row1722018139620"><th class="cellrowborder" valign="top" width="24.95%" id="mcps1.1.4.1.1"><p id="p172202131066"><a name="p172202131066"></a><a name="p172202131066"></a>Code</p>
</th>
<th class="cellrowborder" valign="top" width="42.91%" id="mcps1.1.4.1.2"><p id="p5220913569"><a name="p5220913569"></a><a name="p5220913569"></a>Macro</p>
</th>
<th class="cellrowborder" valign="top" width="32.14%" id="mcps1.1.4.1.3"><p id="p1722061317617"><a name="p1722061317617"></a><a name="p1722061317617"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1422020137612"><td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.1.4.1.1 "><p id="p202201213562"><a name="p202201213562"></a><a name="p202201213562"></a>0xffffffff</p>
</td>
<td class="cellrowborder" valign="top" width="42.91%" headers="mcps1.1.4.1.2 "><p id="p0220171317612"><a name="p0220171317612"></a><a name="p0220171317612"></a>ERR_INVALID_READ</p>
</td>
<td class="cellrowborder" valign="top" width="32.14%" headers="mcps1.1.4.1.3 "><p id="p82208133618"><a name="p82208133618"></a><a name="p82208133618"></a>Data reading failed.</p>
</td>
</tr>
<tr id="row82203139620"><td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.1.4.1.1 "><p id="p1122013131168"><a name="p1122013131168"></a><a name="p1122013131168"></a>0x0</p>
</td>
<td class="cellrowborder" valign="top" width="42.91%" headers="mcps1.1.4.1.2 "><p id="p1322011315617"><a name="p1322011315617"></a><a name="p1322011315617"></a>SUCCESS</p>
</td>
<td class="cellrowborder" valign="top" width="32.14%" headers="mcps1.1.4.1.3 "><p id="p142207137613"><a name="p142207137613"></a><a name="p142207137613"></a>Operation succeeded.</p>
</td>
</tr>
<tr id="row15220213066"><td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.1.4.1.1 "><p id="p14220131313612"><a name="p14220131313612"></a><a name="p14220131313612"></a>0x3c10000</p>
</td>
<td class="cellrowborder" valign="top" width="42.91%" headers="mcps1.1.4.1.2 "><p id="p1822016133612"><a name="p1822016133612"></a><a name="p1822016133612"></a>ERROR</p>
</td>
<td class="cellrowborder" valign="top" width="32.14%" headers="mcps1.1.4.1.3 "><p id="p1422071317614"><a name="p1422071317614"></a><a name="p1422071317614"></a>Operation failed.</p>
</td>
</tr>
<tr id="row3220191311619"><td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.1.4.1.1 "><p id="p22201013865"><a name="p22201013865"></a><a name="p22201013865"></a>0x3c10001</p>
</td>
<td class="cellrowborder" valign="top" width="42.91%" headers="mcps1.1.4.1.2 "><p id="p52211813262"><a name="p52211813262"></a><a name="p52211813262"></a>ERR_ILLEGAL_STATE</p>
</td>
<td class="cellrowborder" valign="top" width="32.14%" headers="mcps1.1.4.1.3 "><p id="p102211913669"><a name="p102211913669"></a><a name="p102211913669"></a>Invalid status.</p>
</td>
</tr>
<tr id="row1222119131064"><td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.1.4.1.1 "><p id="p152211413962"><a name="p152211413962"></a><a name="p152211413962"></a>0x2A05</p>
</td>
<td class="cellrowborder" valign="top" width="42.91%" headers="mcps1.1.4.1.2 "><p id="p7221113864"><a name="p7221113864"></a><a name="p7221113864"></a>ERR_INVALID_PARAM</p>
</td>
<td class="cellrowborder" valign="top" width="32.14%" headers="mcps1.1.4.1.3 "><p id="p12211813968"><a name="p12211813968"></a><a name="p12211813968"></a>Invalid parameter.</p>
</td>
</tr>
<tr id="row1122110131163"><td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.1.4.1.1 "><p id="p1222111131761"><a name="p1222111131761"></a><a name="p1222111131761"></a>0x3c10003</p>
</td>
<td class="cellrowborder" valign="top" width="42.91%" headers="mcps1.1.4.1.2 "><p id="p1622171317617"><a name="p1622171317617"></a><a name="p1622171317617"></a>ERR_EARLY_PREPARE</p>
</td>
<td class="cellrowborder" valign="top" width="32.14%" headers="mcps1.1.4.1.3 "><p id="p1722117131610"><a name="p1722117131610"></a><a name="p1722117131610"></a>Early start.</p>
</td>
</tr>
<tr id="row1322191310611"><td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.1.4.1.1 "><p id="p2221713569"><a name="p2221713569"></a><a name="p2221713569"></a>0x3c10004</p>
</td>
<td class="cellrowborder" valign="top" width="42.91%" headers="mcps1.1.4.1.2 "><p id="p1422115131164"><a name="p1422115131164"></a><a name="p1422115131164"></a>ERR_SOURCE_NOT_SET</p>
</td>
<td class="cellrowborder" valign="top" width="32.14%" headers="mcps1.1.4.1.3 "><p id="p1722119131068"><a name="p1722119131068"></a><a name="p1722119131068"></a>Media source not set.</p>
</td>
</tr>
<tr id="row62216139614"><td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.1.4.1.1 "><p id="p182218133619"><a name="p182218133619"></a><a name="p182218133619"></a>0x3c10005</p>
</td>
<td class="cellrowborder" valign="top" width="42.91%" headers="mcps1.1.4.1.2 "><p id="p72211813061"><a name="p72211813061"></a><a name="p72211813061"></a>ERR_INVALID_OPERATION</p>
</td>
<td class="cellrowborder" valign="top" width="32.14%" headers="mcps1.1.4.1.3 "><p id="p2221161310618"><a name="p2221161310618"></a><a name="p2221161310618"></a>Invalid operation.</p>
</td>
</tr>
<tr id="row2022111312610"><td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.1.4.1.1 "><p id="p1722111139618"><a name="p1722111139618"></a><a name="p1722111139618"></a>0x2A09</p>
</td>
<td class="cellrowborder" valign="top" width="42.91%" headers="mcps1.1.4.1.2 "><p id="p12211713767"><a name="p12211713767"></a><a name="p12211713767"></a>ERR_NOFREE_CHANNEL</p>
</td>
<td class="cellrowborder" valign="top" width="32.14%" headers="mcps1.1.4.1.3 "><p id="p1622115137617"><a name="p1622115137617"></a><a name="p1622115137617"></a>No free channel.</p>
</td>
</tr>
<tr id="row8221201314611"><td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.1.4.1.1 "><p id="p122217138616"><a name="p122217138616"></a><a name="p122217138616"></a>0x3c10007</p>
</td>
<td class="cellrowborder" valign="top" width="42.91%" headers="mcps1.1.4.1.2 "><p id="p1022110130620"><a name="p1022110130620"></a><a name="p1022110130620"></a>ERR_READ_BUFFER</p>
</td>
<td class="cellrowborder" valign="top" width="32.14%" headers="mcps1.1.4.1.3 "><p id="p1322116131064"><a name="p1322116131064"></a><a name="p1322116131064"></a>Error occurred during buffer reading.</p>
</td>
</tr>
<tr id="row142221813263"><td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.1.4.1.1 "><p id="p32221713964"><a name="p32221713964"></a><a name="p32221713964"></a>0x3c10008</p>
</td>
<td class="cellrowborder" valign="top" width="42.91%" headers="mcps1.1.4.1.2 "><p id="p1622221317615"><a name="p1622221317615"></a><a name="p1622221317615"></a>ERR_NOT_STARTED</p>
</td>
<td class="cellrowborder" valign="top" width="32.14%" headers="mcps1.1.4.1.3 "><p id="p11222413963"><a name="p11222413963"></a><a name="p11222413963"></a>Device not started.</p>
</td>
</tr>
<tr id="row1922217130615"><td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.1.4.1.1 "><p id="p19222213267"><a name="p19222213267"></a><a name="p19222213267"></a>0x3c100c8</p>
</td>
<td class="cellrowborder" valign="top" width="42.91%" headers="mcps1.1.4.1.2 "><p id="p32221213768"><a name="p32221213768"></a><a name="p32221213768"></a>ERR_UNKNOWN</p>
</td>
<td class="cellrowborder" valign="top" width="32.14%" headers="mcps1.1.4.1.3 "><p id="p20222171320618"><a name="p20222171320618"></a><a name="p20222171320618"></a>Unknown error.</p>
</td>
</tr>
</tbody>
</table>

**Figure  1**  Position of this repository \(in the dotted blue box\) in the multimedia subsystem<a name="fig9521193714117"></a>  
![](figures/position-of-this-repository-(in-the-dotted-blue-box)-in-the-multimedia-subsystem.png "position-of-this-repository-(in-the-dotted-blue-box)-in-the-multimedia-subsystem")

## Directory Structure<a name="section8685144625320"></a>

```
foundation/multimedia/media_utils_lite
├── interfaces    # Header file of the data types and media formats
└── hals       # HAL adaptation APIs
└── src        # Implementation of the data types and media formats
```

## Usage<a name="section1648194512427"></a>

Build a single repository in the root directory.

```
# Select the development board.
hb set  
# Build this repository.
hb build media_service
```

## Constraints<a name="section161941989596"></a>

C++ 11 or later

# Changes in This Release<a name="section_changes_en"></a>

This repository is adapted for the HiSpark AiFly (Hi3403V100) development board. For clarity, the changes are described in two parts: **Added Features** and **Enhanced Existing Features**.

## Added Features

1. Added the camera HAL manager interface
    -   `hals/hal_camera.h` adds the `HalCameraManager` function-pointer table with `GetHalCameraFuncs`/`GetHalDistributedCameraFuncs` under `MEDIA_INTERFACE_V1_0`: the camera ID changes from a number to a string, and distributed camera management APIs are added (`HalCameraAddCameraDevice`/`HalCameraRemoveCameraDevice`/`HalCameraAcquireBuffer`/`HalCameraShutterBuffer`/`HalCameraOnSettingsResult`/`HalCameraNotify`, etc.), while the original APIs are kept for the legacy path.

2. Added the audio device info model
    -   `interfaces/kits/media_info.h` adds `AudioSystemDeviceType` (local/virtual microphones and speakers), `DeviceConnectStatus` and `AudioDeviceInfo` (with `dhId`, device name, device type and connection status), providing data structures for audio device management and device-change callbacks.

3. Added the media log module
    -   Added `src/media_log.cpp`: provides `MediaLogPrintf`/`MediaDfxLogPrintf`/`SetMediaLogLevel`/`GetMediaLogLevel`, with log-level gating (atomic variable, ERROR level by default under NDEBUG), hilog output under `HI_LOG_ENABLE`, and the `DECORATOR_LOG` macro wrapper carrying the function name and line number.

4. Added the DFX statistics utility
    -   Added `interfaces/kits/media_utils.h` and `src/media_utils.cpp`: under `ENABLE_DFX`, provides audio receive-time recording (`MediaRecordAudioRecvTime`) and sync time-difference printing (`MediaPrintSyncTimeDiffUs`), with clock retrieval and multiplication overflow protection.

5. Added build arguments and configuration items
    -   `config.gni` adds the `enable_distributed_hardware`, `enable_distributed_dfx` and `drivers_peripheral_display_4K_support` switches.

6. Added the Format key and error code
    -   `interfaces/kits/format.h` adds the `LAYER_PRIORITY` key (for the player layer priority setting); `interfaces/kits/media_errors.h` adds the `ERR_AUDIO_READ_DATA_TIME_OUT` error code.

## Enhanced Existing Features

1. The existing video stream attribute structure is enhanced
    -   Original functionality: `StreamAttr` contained only width, height and frame rate information.
    -   Enhancement: the `displayWidth`/`displayHeight` fields are added under `MEDIA_INTERFACE_V1_0`.

2. The existing camera detect callback signatures are enhanced
    -   Original functionality: `CameraDetectCb`/`CameraResultCb` used `uint32_t` camera IDs.
    -   Enhancement: under `MEDIA_INTERFACE_V1_0`, string camera IDs (`const char *`) are used, consistent with the camera HAL manager interface.

3. The existing position info structure is enhanced
    -   Original functionality: `PosInfo` contained only the x and y coordinates.
    -   Enhancement: the width and height fields (w/h) are added under `MEDIA_INTERFACE_V1_0`.

4. The existing log macros are enhanced
    -   Original functionality: the `MEDIA_*_LOG` macros chose whether to carry the function name, file name and line number based on `OHOS_DEBUG`.
    -   Enhancement: they uniformly go through `DECORATOR_LOG` (function name + line number); level filtering and the output backend are handled inside `media_log.cpp`, making the macro definitions simpler.

5. The existing build configuration is enhanced
    -   Original functionality: `media_common` compiled only `format.cpp` and `source.cpp`.
    -   Enhancement: `media_log.cpp` and `media_utils.cpp` are added; the `HI_LOG_ENABLE`/`ENABLE_DFX` macros are defined; the `hilog_shared` dependency is added for non-liteos_m kernels.

6. The existing open-source compliance configuration is enhanced
    -   Original functionality: `OAT.xml` configures open-source compliance scanning.
    -   Enhancement: a policyitem is added, registering the HiSilicon copyright.

## Repositories Involved<a name="section105062051111614"></a>

[Multimedia subsystem](https://gitee.com/openharmony/docs/blob/master/en/readme/multimedia.md)

[camera\_lite](https://gitee.com/openharmony/multimedia_camera_lite)

[camera\_sample\_lite](https://gitee.com/openharmony/applications_sample_camera)

[audio\_lite](https://gitee.com/openharmony/multimedia_audio_lite)

[media\_lite](https://gitee.com/openharmony/multimedia_media_lite)

[media\_utils\_lite](https://gitee.com/openharmony/multimedia_utils_lite)

