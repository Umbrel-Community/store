<p align="center">
<img alt="UmbrelScape logo" src="https://i.imgur.com/draS8cZ.png" width="180">
</p>
<h2 align="center">Umbrelscape Store</h2>
<h5 align="center">Community store for your umbrel.</h5>
<br>

This repository is the home for various apps for your [umbrel](https://getumbrel.com), powered by the [`Community App Store`](https://github.com/getumbrel/umbrel-community-app-store) feature.

### Get started
To use our community app store, you can add this repository through the Umbrel user interface similar to the demo *(Thanks umbrel for the video!)*:


https://user-images.githubusercontent.com/10330103/197889452-e5cd7e96-3233-4a09-b475-94b754adc7a3.mp4


Alternatively, you can use the Umbrel CLI as described below.

To add the store:
```sh
sudo ~/umbrel/scripts/repo add https://github.com/UmbrelScape/store.git

sudo ~/umbrel/scripts/repo update
```

To install an app from the app store
```sh
sudo ~/umbrel/scripts/app install umbrelscape-hello-world
```

To remove the store:
```sh
sudo ~/umbrel/scripts/repo remove https://github.com/UmbrelScape/store.git
```


### Apps in the store
***Warning!: This store installs a separate instance of apps, seperate from the apps provided by the Official umbrel store.***
* Nextcloud `25.0.1`
* Pi-Hole `5.14.1-hotfix-1`


### Technical Details
The `umbrel-app-store.yml` file defines two important properties:
- `id` - This is used as a prefix for all apps within the community app store. You **MUST** prefix your application id with your app store ID. For example, this template defines `sparkles` as a community app store ID and we have a `hello world` app. The app ID therefore should be: `sparkles-hello-world`
- `name` - This name appears within the Umbrel user interface when users explore apps within these community app stores.


