# A Timer/Stopwatch for OBS Studio

This is an easy to use stopwatch/timer script for your OBS Studio.

## How to integrate into your OBS Studio?
You have 2 ways to use this stopwatch. 

#### 1 - Use online version
This version can be customized with URL parameters and you do not need to download any file.
However, you cannot modify the design with the online version.

1. Copy the following URL: `https://raw.githack.com/brainfoolong/obs-stopwatch/master/stopwatch.html`
2. In OBS Studio add a new "Browser" source. Paste the URL into the "URL" field.
3. Done. It should look like the bellow demonstration GIF. 

#### 2 - Use local version (Modifyable)
With this version, you download the `stopwatch.html` and you can modify things to your needs. You can change the style and behaviour to what you like. It requires some knowledge of Html, Css and Javascript.

1. Download `stopwatch.html` and copy it to your disk.
2. In OBS Studio add a new "Browser" source. Check the checkbox `Local File` and point it to the `stopwatch.html`
3. Modify the file if required. Configuration is at the top of the file.

## Configuration parameters

* `MODE` 
  * Possible Values
    * `count_up` - default - Count up
    * `count_down` - Count down instead of count_up
* `START_TIME` 
  * Possible Values
    * `00:00:00` - default - Any number in this format

If you use installation method 1, than you can append some URL parameters to the URL to modify the behaviour.

Examples:

    // countdown from 00:10:00 instead of countup from 00:00:00
    https://raw.githack.com/brainfoolong/obs-stopwatch/master/stopwatch.html?MODE=count_down&START_TIME=00:10:00   
    // countup with custom starting time
    https://raw.githack.com/brainfoolong/obs-stopwatch/master/stopwatch.html?START_TIME=00:10:00

If you use method 2, there is a configuration part at the top of the file where you can modify the parameters.

## How does it look like ?
![Demo](https://rawcdn.githack.com/brainfoolong/obs-stopwatch/80b76d279bf326c9029514e56f69b44e2dddcb20/demo-images/demonstration.gif)
