# AI Net Profit™ Demos
I have been workig a free AI Neural Network Accounting aplication called AINetProfit™ that I am getting ready to release. This repository will include aarts of that app broken up into smaller pieces the code for creating various Neural Networks for accounting and managing a variety of things from media buying to security can be more eaasily examined for how ML.NET can be used to create and train those networks.

# Background
My background is in Theoretical Physics and Medicine. But after fuinishing medical school I decided to sell products I created on National Television instead of practicing. I wrote educational software I sold on national television and later I wrote software to manage my companies. Many years ago I used C++ and Bayesian Optimization and an early forms of neural networks to determine which television stations to buy half hour infomercial time on. I was able to determine which television stations to buy by matching the demographics of a product with that of the zip code census data against the zip codes that fell within the broadcast radius of each television station. And I was able to calculate the maximum amount to bid on each station for each half hor of infomercial time to maximize my net profit on each media buy. The results of each media buy were feed baack using Bayesian Optimization and that system was so successful that it enabled me to make a large fortune.

Later I applied those same techniques to all forms of advertising to determine what ad media to buy and the maximum to pay for each buy by calculating the probality of turning a net profit over the cost of media.

This series of articles will demonstrate the techniques I developed in AI, Neural Networks and Bayesian Op[timization.



AI Neural Networks &amp; Bayesian Optimization for Media Buying
## AIDemos Electron.NET ASP.NET 8 CORE 8 Web App (Model-View-Controller)

## Explanation of CORE Naming
In November 2020, Microsoft released .NET 5.0, dropping the "Core” branding so all 
versions of .NET after 5.0 are "Core" apps. Commonly you will see .NET 8 applications 
refrred to as a "Core 8" applications because .NET 8 is a Core application.

- ### Install These Packages
- Microsoft.AspNetCore.Mvc.NewtonsoftJson (Version="8.0.10")
- xMicrosoft.DotNet.UpgradeAssistant.Extensions.Default.Analyzers (Version="0.4.421302")
- Microsoft.Extensions.Hosting (Version="8.0.1") 
- Microsoft.Extensions.Logging (Version="8.0.1")
- Microsoft.VisualStudio.Web.CodeGeneration.Design (Version="8.0.6")
- Newtonsoft.Json (Version="13.0.3")
- Microsoft.Data.Sqlite.Core (Version="8.0.10")

- ### Install SQLite Packages
- SQLitePCLRaw.bundle_e_sqlite3 (Version="2.1.10")  
- SQLitePCLRaw.bundle_green (Version="2.1.10")
- SQLitePCLRaw.core (Version="2.1.10")
- SQLitePCLRaw.provider.dynamic_cdecl (Version="2.1.10")

- ### Install ML.NET Packages
- Microsoft.ML (Version="3.0.1")

- ### Install Electron.NET
- ElectronNET.API (Version="23.6.2")

- ### Other Packages You Can Add
- ExcelDataReader (Version="3.7.0")
- Markdig (Version="0.37.0")

•	Initialize Electron.NET Project
Open in Visual Studio and Build Project
Open Tools > NuGet Package Manager > Package Manager Console
This opens in the project directory, and you run:
To initialize Electron.NET and create an electron.manifest.json file run:
    > electronize init

•	Run the Application
 In the directory where the .proj file is located there is a .bat file called “zrun.bat”
 Run this bat file as Administrator.
 You can customize this bat file for debugging and logging:
@echo off
REM run bat file from directory it is in
cd /d "%~dp0"
REM start the application
             electronize start
    		REM To create a log file for debugging
    		; electronize start /watch > electronize_output.txt 2>&1




## IMAGES & EMOJIS SYMBOLS: ™, ®, ©, 

Here are some emojis you can use directly in html:
https://unicode.org/emoji/charts/full-emoji-list.html
https://emojipedia.org/travel-places/
https://emojihub.org/
https://emoji-copy-paste.com/

## PDF & Word Export Formatting

    var today = new Date();
    var formattedDate = today.getFullYear() + '/' + (today.getMonth() + 1) + '/' + today.getDate();
    var r_header_title = 'Date: ' + formattedDate;
    var r_main_title = 'Sample Report';
    var r_messageTop = 'Whatever you want here';
    var r_footer_text = '©1992 - 2024 All Rights Reserved Worldwide';

    // Generates a random number between 0 and 9999
    var randNumber = Math.floor(Math.random() * 10000);  

    // Set r_filename to include today's date and the random number
    var r_filename = 'pdf_' + formattedDate + '_' + randNumber;


## Fonts - Use calc

Use the `calc()` function to dynamically calculate the font size based on the width of the viewport (`vw`). This technique is often used to create fluid typography on web pages, making the font size responsive to the screen size without the need for media queries. Here's a breakdown of how it works:

```css
font-size: calc(13px + (15 - 13) * ((100vw - 300px) / (1600 - 300)));
```

1. **Base Font Size**: The calculation starts with a base font size of `13px`. This is the minimum font size that will be applied.
2. **Font Size Range**: The next part, `(15 - 13)`, calculates the range within which the font size can grow. In this case, the font size can increase by up to `2px` (from `13px` to `15px`).
3. **Viewport Width Adjustment**: `100vw` represents 100% of the viewport width. The expression `(100vw - 300px)` calculates the difference between the current viewport width and `300px`. This difference will be used to adjust the font size based on the screen width.
4. **Scaling Range**: `(1600 - 300)` calculates the total scaling range for the viewport width, which in this case is `1300px` (from `300px` to `1600px`). This defines the range over which the font size will adjust.
5. **Final Calculation**: The entire `calc()` function calculates the font size by starting with the base size (`13px`), then adds an increment that scales based on the viewport width. The increment is proportionally scaled within the range defined by `(15 - 13) * ((100vw - 300px) / (1600 - 300))`. This means as the viewport width increases from `300px` to `1600px`, the font size will linearly increase from `13px` to `15px`.

In summary, this CSS rule makes the font size start at `13px` when the viewport width is `300px` or less. 
As the viewport width grows, the font size increases linearly, reaching `15px` when the viewport width hits `1600px`. 
For viewport widths between `300px` and `1600px`, the font size will be somewhere between `13px` and `15px`, calculated 
based on the formula provided. This approach provides a smooth transition of font sizes across different screen widths, 
enhancing readability and user experience on a variety of devices.

