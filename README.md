# Banana Picker

A small web app that reads banana ripeness live from the phone camera and says whether a banana is a Today, Tomorrow or Day-after pick, or a skip.

Everything runs in the browser. The camera video is analyzed on the device and is never uploaded. Training samples are kept in the browser's local storage on that device. The only file the app ever fetches is its own `starter-training.json`, and only when you tap Load photo-based values. It uses no analytics, accounts or third-party scripts.

`starter-training.json` holds numbers only (green and brown shares and a label) measured from 80 photos in github.com/psolymos/bananas (MIT License, Copyright 2022 Peter Solymos). No images are included.

Add it to the iPhone Home Screen from Safari (Share, then Add to Home Screen) and open it from there.

The stem and tip of each banana are dark by nature, so the app finds the long axis of the banana and ignores the outer 12% at each end before measuring green and brown. An end that runs off the edge of the box is not trimmed.
