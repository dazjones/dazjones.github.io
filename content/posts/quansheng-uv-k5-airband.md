---
title: "Can a £20 Radio Really Track Air Traffic? (Yes, If You Tweak It)"
date: 2025-12-19
description: "For the price of a takeaway, the Quansheng UV-K5(8) can track air traffic across the UK. Discover how to flash the Egzumer firmware to unlock hidden features and why disabling transmission is critical for staying legal."
tags: ["radio","tinkering"]
---


Did you know that dedicated airband scanners used to cost upwards of £150? For less than the price of a standard takeaway, you can now own a device capable of monitoring the communications of the 2.2 million flights that traverse UK airspace every year.

I’ve always had a fascination with radio and aircraft. There is something undeniably cool about looking up and incoming flight on flightradar, tuning a dial, and hearing the pilot speak to the tower. But until recently, the hardware required to do that was either expensive or bulky.

Enter the Quansheng UV-K5(8). It’s cheap, it’s cheerful, and with a bit of tinkering, it’s brilliant.

### The "Baofeng Killer"?

Out of the box, the UV-K5(8) is a standard dual-band handheld transceiver. It’s fine, but it’s nothing special. However, the reason this specific radio has blown up in the community isn't what it does stock. It is what it can do when you replace the software.

The chip inside this radio is capable of much more than the factory allows. The community has cracked it wide open, and the best firmware out there right now for aviation enthusiasts is [Egzumer](https://github.com/egzumer/uv-k5-firmware-custom/releases).

### The Setup: A "Click" of Confidence

Updating the firmware is surprisingly easy (it is done via a web browser) but I did hit a snag that nearly made me give up before I started.

To flash the firmware, you need a programming cable. The standard K-type used for Baofengs works fine. When I first plugged it in, the computer wouldn't see the radio. I spent ages messing with drivers, thinking I’d bought a dud.

**Here is the trick:** You really have to force that cable in.

The waterproofing rubber on the side creates a lot of resistance. I had to push the connector harder than felt comfortable until I felt a distinct, solid *click*. Once it was seated properly, the flash took seconds. If you don't feel that click, you aren't connected.

### Why Egzumer?

Once I flashed the Egzumer firmware, the radio transformed. The biggest change is the AM handling. Aircraft communicate using Amplitude Modulation (AM) in the 108 MHz to 137 MHz range. The stock firmware tries to fake this, and the audio is usually garbled. Egzumer fixes the demodulation, making the audio crisp.

It also adds a Spectrum Analyser This is a visual graph on the screen that shows you spikes in radio activity. Instead of blindly scanning, you can *see* a signal on a nearby frequency and tune right to it.

The result? I immediately tuned into my local airport's tower and approach frequency. The clarity was shocking for a radio this cheap.

### The Legal Reality: Listen, Don't Talk

This is the most important part of this post, especially for us in the UK.

The Quansheng UV-K5(8) is a transceiver, meaning it can transmit. However, transmitting on airband frequencies is **strictly illegal** and incredibly dangerous. You are interfering with safety-of-life communications. Even if you have an Amateur Radio (Ham) licence, you cannot transmit on airband.

Furthermore, because this radio wasn't designed to transmit on these frequencies, the hardware lacks the necessary filters. If you try to TX (transmit), you will likely spew "harmonics" (radio interference) all over other bands, annoying everyone from the MoD to your neighbour trying to watch Freeview.

**The Fix:**
Egzumer makes this easy. In the hidden menus, you can set specific frequency ranges to **TX DISABLE**.
* Go to the menu.
* Find the airband range.
* Select **TX DISABLE**.

This effectively turns your £20 talkie into a dedicated scanner. It keeps you legal, it keeps the airwaves safe, and it stops you from accidentally keying the mic when you’re just trying to listen to the approach into Heathrow or Edinburgh.


If you are interested in radio, there has never been a better time to jump in. The Quansheng UV-K5(8) isn't perfect, but for the price, it’s an incredible tool for learning how the airwaves work. Just remember: push that cable in until it clicks, flash Egzumer, and **disable that TX**.

***

> **Recommended Watch:** If you want a visual guide on the Egzumer menus, this video is excellent: [Quansheng UV-K5(8) tutorial video: How to best use it for the Airband](https://www.youtube.com/watch?v=zt0p0RHaSAA).