---
title: Using the Recorder
layout: en
permalink: docs/guides/recorder/
---

In this guide you will get to know the components of the CONTINUOUS Recorder. It consists of

<ul>
	<li>The device in the middle.</li>
	<li>The script editor on the right.</li>
	<li>The operations bar on the left.</li>
</ul>

<img src="/img/guides/recorder/recorder-01.png">


<h3>Step 1: Start Recording</h3>

On the right above the editor you'll find the recorder controls to enable the recording or replay mode. To record your first test, hit <em>Record</em>.

<img src="/img/guides/recorder/recorder-02.png">


<h3>Step 2: Use Your App</h3>

In the middle of the screen you'll find the testing device. It gives you access to the emulator which had been selected when creating the new test. You can use it just as a user of your app would.

When recording is enabled the actions you perform on the device are recorded. This means, the respective steps are added to the script on the right side of the screen.


<h3>Step 3: Adjust Locator</h3>

Now try out adjusting your newly created step by clicking the settings icon in the respective script line.

<img src="/img/guides/recorder/recorder-03.png">

This will open the settings dialog. In the <em>Adjust Locator</em> tab you can modify the locator. Just enable either the <em>Move and Resize</em> or the <em>Draw New</em> mode. In order to set the precise click position use the <em>Set Offset</em> mode. This will set the click coordinates relative to the locator box. Alterntively, you can also switch the <em>click strategy</em> to <em>click on position</em> to click on an absolute position on the screen. <a href="/docs/references/recorder/action-settings#locator">Read more...</a>

<img src="/img/guides/recorder/recorder-04.png">


<h3>Step 4: Set Timeout</h3>

In the <em>Set Timeout</em> tab you can specify how long the system should look for your locator on the screen. The timeout is the maximum amount of time it will try matching the locator. <a href="/docs/references/recorder/action-settings#timeout">Read more...</a>

<img src="/img/guides/recorder/recorder-05.png">


<h3>Step 5: Fine-tune Matching</h3>

In the <em>Fine-tune Matching</em> tab you can adjust the sensitivity of the image matcher. With a high value the locator must always look very similar and appear in a almost in the same position on the screen, with a low value both can deviate more from the original. Adjusting the matching precision is usually very handy when a warning or an error occurs during replay. <a href="/docs/references/recorder/action-settings#matching">Read more...</a>

Now click <em>Save</em> to close the dialog. Notice how the line has been updated in the script.


<h3>Step 6: Add Assertions</h3>

In most test cases you don't only want to validate the click execution but also check the presence of some graphical elements. With assertions you can make sure that certain elements vanish from or appear on the screen. To add assertions for an action, press the plus icon in the respective script line. <a href="/docs/references/recorder/assertion-builder">Read more...</a>

<img src="/img/guides/recorder/recorder-06.png">

This will open the assertion builder. In the <em>Appearing Locators</em> tab pick elements which you expect to appear after an action was performed. The system gives you a few suggestions that you can you can modify in the <em>Move and Resize</em> mode. You can also draw your own in the <em>Draw New</em> mode.

<img src="/img/guides/recorder/recorder-07.png">

Switch to the <em>Vanishing Locators</em> tab to pick locators that you expect to vanish after the action was performed.

Now click <em>Insert Assertions</em> to close the dialog. Notice the new lines that have been added to the script.

<img src="/img/guides/recorder/recorder-08.png">


<h3>Step 7: Add Sensor Actions</h3>

Input actions and assertions can also be added using the operations bar on the left side. You will then see the settings dialog from above with a screenshot of the current device screen.

The operations bar offers you additional functionality. For example try out the <em>Sensor</em> actions to rotate the device or set the GPS coordinates. <a href="/docs/references/scripting-api/sensor">Read more...</a>

<img src="/img/guides/recorder/recorder-09.png">


<h3>Step 9: Stop Recording</h3>

Leave the recording mode by hitting <em>Stop</em>.

<img src="/img/guides/recorder/recorder-10.png">


<h3>Step 10: Replay Your Test</h3>

You can now replay your test. To do so press the <em>Play</em> button.

<img src="/img/guides/recorder/recorder-11.png">

You will then get a fresh device so that the replay starts in a clean state. The editor, the device and the operations bar are locked during replay. You can now follow the execution of your test.

<img src="/img/guides/recorder/recorder-12.png">


<h3>Step 11: View Report</h3>

As soon as the replay has finished, the result is shown at the top. It includes a link to the detailed report about this replay.

<img src="/img/guides/recorder/recorder-13.png">

In the report the executed steps are listed with two screenshots. The first was taken during recording and the second during replay. Like that you can easily compare if your app was behaving differently after replaying for example on a different version of your app or a another Android version.

<img src="/img/guides/recorder/recorder-14.png">


<h3>Step 12: Stop Replay</h3>

Leave the replay mode by clicking the close icon. 

<img src="/img/guides/recorder/recorder-15.png">