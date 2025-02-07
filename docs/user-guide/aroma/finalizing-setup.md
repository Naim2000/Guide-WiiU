# Aroma {docsify-ignore-all}

## Finalizing Setup

Now that PayloadLoader, Environment Loader and Aroma are installed, we are going to finalize the setup.

We are going to make the Aroma environment start automatically when your console autoboots the Health and Safety Information app (or when manually launching it if you chose not to autoboot it) and select Wii U Menu as default as well as getting additional homebrew apps. Please note that the following steps assumes you are autobooting the Health and Safety Information app.

### Setting up PayloadLoader, Environment Loader and Aroma

1. Launch the EnvironmentLoader.
    - If you are autobooting the PayloadLoader, simply turn on your Wii U.
    - If you skipped the autobooting steps, launch the Health and Safety Information app.
1. Using the D-Pad, navigate to `aroma` and press Y to set this to your default environment, then press A to launch into Aroma.
    - You might get a red warning screen telling you that updates aren't blocked properly. Press A to continue anyway. We're going to block updates in the "Blocking Updates" section below.
    - To open the Environment Loader in the future, you have to hold X while your Wii U is booting or loading the Health and Safety Information app.
1. On the Aroma Boot Selector, the `Wii U Menu` should already be selected, press Y to set this to your default autobooting option, then press A to launch into the Wii U Menu.
    - To open the Aroma Boot Selector in the future, you have hold START (+) while the console is booting or loading the Health and Safety Information app.

### Blocking Updates
While Aroma's PayloadLoader already has built-in update blocking functionality, it is recommended to delete the update folder to effectively block system updates.
If you get a red warning screen while booting into Tiramisu, the update folder still exists and it is recommended to delete it using [this guide](../block-updates).

### Additional Homebrew Apps

?> All Homebrew applications are loaded from the Wii U Menu on Aroma.

- **SaveMii Mod WUT Port** is a homebrew app that lets you manage your Wii U and vWii save data.
- **Bloopair** is an Aroma module that lets you wirelessly connect most popular Bluetooth capable controllers. See [this page](https://gbatemp.net/threads/bloopair-connect-controllers-from-other-consoles-natively.594289/) for more details.
- The **Homebrew Appstore** lets you browse and download homebrew apps directly from your Wii U.

### Additional Homebrew Apps - What You Need

- The latest version of [SaveMii Mod WUT Port](https://wiiubru.com/appstore/zips/SaveMiiModWUTPort.zip).
- `wiiu-extracttosd.zip` of the [HB Appstore](https://github.com/fortheusers/hb-appstore/releases/).

### Additional Homebrew Apps - Extracting Files to the SD Card

1. Copy the contents of the newly downloaded `SaveMiiModWUTPort.zip` file to the root of your SD Card.
1. Copy the contents of the newly downloaded `wiiu-extracttosd.zip` file to the root of your SD Card.

### Recommended Plugins

| Name | Description | Installation Instructions |
| ---- | ----------- | ------------ |
| [FTPiiU Plugin](https://github.com/wiiu-env/ftpiiu_plugin/) ([Download](https://github.com/wiiu-env/ftpiiu_plugin/releases)) | Runs a FTP server in the background. | 1. Extract the downloaded `ftpiiu_vX_X.zip` file. <br> 2. Copy the `ftpiiu.wps` to the `wiiu/environments/aroma/plugins` folder on the root of your SD Card. |
| [SDCafiine](https://github.com/wiiu-env/sdcafiine_plugin/) ([Download](https://github.com/wiiu-env/sdcafiine_plugin/releases)) | Allows you to mod games by redirecting files to the SD Card. | 1. Extract the downloaded `sdcafiine_vX_X_X.zip` file. <br> 2. Copy the `sdcafiine.wps` to the `wiiu/environments/aroma/plugins` folder on the root of your SD Card. |
| [Bloopair](https://github.com/GaryOderNichts/Bloopair/) ([Download](https://github.com/GaryOderNichts/Bloopair/releases)) | Allows wirelessly connecting most popular Bluetooth capable controllers. | 1. Extract the contents of the newly downloaded `Bloopair_vX.X.X.zip` file. <br> 2. Copy the `30_bloopair.rpx` to the `wiiu/environments/aroma/modules/setup/` folder on the root of your SD Card. <br> 3. Copy the `wiiu` folder to the root of your SD Card. |
| [Screenshot Plugin](https://github.com/wiiu-env/ScreenshotWUPS/) ([Download](https://github.com/wiiu-env/ScreenshotWUPS/releases)) | Allows taking screenshots directly to the SD Card. | 1. Extract the downloaded `screenshot_plugin_vX_X.zip` file. <br> 2. Copy the `screenshot.wps` to the `wiiu/environments/aroma/plugins` folder on the root of your SD Card. |

### Booting Tiramisu

If you find the need to boot into Tiramisu, for example, to use a legacy Homebrew app, do the following:

1. Download the latest files from [Tiramisu for your café](https://tiramisu.foryour.cafe).
1. Copy the `wiiu` folder to the root of your SD Card.
    - The folder should merge with the existing `wiiu` folder if not done automatically.
1. Take the SD Card out of your computer and plug it into your Wii U console.
1. Start the EnvironmentLoader.
    - If you're autobooting into it, this can be done by powering on your console and holding X.
1. Highlight the entry called `tiramisu` using the D-Pad.
1. Launch Tiramisu by pressing A.
1. Launch the Wii U Menu by pressing A.
    - To make the console autoboot the Wii U Menu when loading the Tiramisu environment, press Y.
1. Homebrew Launcher can be loaded by launching the Mii Maker app.
