# LosGram

LosGram is an independent Android Telegram client based on the ShuzaGram Mod source code and the open-source Telegram for Android project.

This repository preserves the upstream ShuzaGram functionality while beginning the LosGram rebrand. It includes the original plugin system and the features documented in the source project.

LosGram is not affiliated with Telegram FZ-LLC, ShuzaGram, or exteraGram. This project is licensed under **GPL-2.0**; see [LICENSE](LICENSE). Keep all required upstream copyright and license notices when modifying or redistributing the source.

## Building

1. Initialize native dependencies: `git submodule update --init --recursive`.
2. Obtain your own Telegram `api_id` and `api_hash` from <https://my.telegram.org> and configure them in `TMessagesProj/src/main/java/org/telegram/messenger/BuildVars.java`.
3. Configure your own signing keystore and any required Google/Firebase configuration.
4. Build a debug APK with `./gradlew :TMessagesProj_App:assembleAfatDebug`, or a release APK with `./gradlew :TMessagesProj_App:assembleAfatRelease`.

## Plugins

The upstream plugin system supports exteraGram-compatible `.plugin` files. Its settings entry is available under Settings → LosGram → Plugins.

## Upstream

Based on [ShuzaGram Mod](https://github.com/shuzq-sh/shuzagram-mod) and [Telegram for Android](https://github.com/DrKLO/Telegram).