# Changelog

## \[0.2.2]

- Added support for opening Android Studio installed by JetBrains Toolbox
  - [448fa99](https://github.com/tauri-apps/tauri-mobile/commit/448fa9993de3a1312ee3076a5b8ed607738932ba) feat: add support for android studio which installed by jetbrains toolbox ([#88](https://github.com/tauri-apps/tauri-mobile/pull/88)) on 2023-02-08
- Increased minimum iOS version from 9 to 13
  - [ae11564](https://github.com/tauri-apps/tauri-mobile/commit/ae115647e7c80f1b03b678c3cf76b202f9f5324f) Update minimum iOS version to 13 ([#93](https://github.com/tauri-apps/tauri-mobile/pull/93)) on 2023-02-12
- Fixed ADB and xcodebuild execution on environments like Node-API.
  - [6ce6e1f](https://github.com/tauri-apps/tauri-mobile/commit/6ce6e1f2d1f4128938ddf366c41834b78873be61) fix: command execution in tauri's Node.js CLI ([#97](https://github.com/tauri-apps/tauri-mobile/pull/97)) on 2023-02-17
  - [2f7d7a0](https://github.com/tauri-apps/tauri-mobile/commit/2f7d7a0c1136da2596d7614538411b333cddeda2) fix(apple): use duct to run xcodebuild ([#98](https://github.com/tauri-apps/tauri-mobile/pull/98)) on 2023-02-17

## \[0.2.1]

- Fix `cargo mobile update` target branch and enabled `cli` feature when update.
  - [b5791ed](https://github.com/tauri-apps/tauri-mobile/commit/b5791ed37000b92db0f5beaa50d1f6c4af52a479) fix: enable cli feature when cargo mobile update, closes [#84](https://github.com/tauri-apps/tauri-mobile/pull/84) ([#86](https://github.com/tauri-apps/tauri-mobile/pull/86)) on 2023-02-02
- Fix content assignment in ios template.
  - [81b642d](https://github.com/tauri-apps/tauri-mobile/commit/81b642de9bd0c96b124ad9bca9edfbabe78f71d4) fix(template): fix variable assignment in wry's ios template ([#82](https://github.com/tauri-apps/tauri-mobile/pull/82)) on 2023-01-30

## \[0.2.0]

- Bump minor version as `0.1.5` add a new feature which was incompatible with `0.1.4`
  - [969e8ef](https://github.com/tauri-apps/tauri-mobile/commit/969e8ef41ec6f5c51086b4971cb74318ed5fa0c3) chore: bump minor for urgent release on 2023-01-15

## \[0.1.5]

- Add support for `CARGO_TARGET_DIR` and `CARGO_BUILD_TARGET_DIR` env vars.
  - [e66a6ab](https://github.com/tauri-apps/tauri-mobile/commit/e66a6ab0e5dc3b474dad6793621c499974953915) feat: improvements for lib name and cargo target dir env vars ([#73](https://github.com/tauri-apps/tauri-mobile/pull/73)) on 2023-01-06
- Allow specifying `lib_name` in `mobile.toml` file. This useful if you set `[lib].name` in `Cargo.toml`.
  - [e66a6ab](https://github.com/tauri-apps/tauri-mobile/commit/e66a6ab0e5dc3b474dad6793621c499974953915) feat: improvements for lib name and cargo target dir env vars ([#73](https://github.com/tauri-apps/tauri-mobile/pull/73)) on 2023-01-06
- Adjust `wry` template for desktop usage also.
  - [3978774](https://github.com/tauri-apps/tauri-mobile/commit/3978774e1b5e7810f3fa6833c328e3032d744e7e) Update wry template to work on desktop as well ([#76](https://github.com/tauri-apps/tauri-mobile/pull/76)) on 2023-01-13
- Update `wry` template to use the new `wry` env vars.
  - [0113d1f](https://github.com/tauri-apps/tauri-mobile/commit/0113d1fc5fcc976a8c5c9016ae55e94fcc182ea6) feat: update wry template to use the new env vars on 2022-12-30

## \[0.1.4]

- Improve error message for missing library artifact.
  - [807861a](https://github.com/tauri-apps/tauri-mobile/commit/807861acfedf50e31086db62e56d296a62638194) feat: validate library artifact existence on 2022-12-28

## \[0.1.3]

- Allow specifying an app target dir resolver via `config::App::with_target_dir_resolver`.
  - [74c150a](https://github.com/tauri-apps/tauri-mobile/commit/74c150a7ad84db516fa39a6e9c7a4454de1d5d83) feat: allow setting a custom target dir resolver ([#68](https://github.com/tauri-apps/tauri-mobile/pull/68)) on 2022-12-28

## \[0.1.2]

- Fix `android_binding!` macro usage in the `wry` template.
  - [fd68c94](https://github.com/tauri-apps/tauri-mobile/commit/fd68c9435cdac5d591e22ff92ec2b7d36f07d8a7) fix: fix android_binding! usage in wry template on 2022-12-27

## \[0.1.1]

- Show all application logs on iOS noninteractive mode.
  - [eb071b6](https://github.com/tauri-apps/tauri-mobile/commit/eb071b65c49c4bd20abbc917fa47c75273977b4f) feat(apple): show app logs, simulator noninteractive mode ([#63](https://github.com/tauri-apps/tauri-mobile/pull/63)) on 2022-12-23
- Implement noninteractive mode on iOS simulators.
  - [eb071b6](https://github.com/tauri-apps/tauri-mobile/commit/eb071b65c49c4bd20abbc917fa47c75273977b4f) feat(apple): show app logs, simulator noninteractive mode ([#63](https://github.com/tauri-apps/tauri-mobile/pull/63)) on 2022-12-23
- Fix `cargo apple run` can't work on real device.
  - [89bbe2b](https://github.com/tauri-apps/tauri-mobile/commit/89bbe2bdd30b55d5e4af91aced779d88997cfec7) Fix `cargo apple run` can't work on real device ([#59](https://github.com/tauri-apps/tauri-mobile/pull/59)) on 2022-12-26
- Added the `openssl-vendored` Cargo feature.
  - [f76d8db](https://github.com/tauri-apps/tauri-mobile/commit/f76d8db3ca8ca472aeab8d28c0e7b41c8348de9a) feat: add `openssl-vendored` feature ([#57](https://github.com/tauri-apps/tauri-mobile/pull/57)) on 2022-12-10

## \[0.1.0]

- Initial release!
  - [4f2b4f6](https://github.com/tauri-apps/tauri-mobile/commit/4f2b4f65ddd36252ee979f88ae76855ff5c5923f) feat: prepare initial release ([#54](https://github.com/tauri-apps/tauri-mobile/pull/54)) on 2022-12-06
