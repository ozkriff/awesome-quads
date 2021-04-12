# Awesome Quads

A curated list of links to miniquad/macroquad-related code & resources.

## Game engines

- [miniquad](https://github.com/not-fl3/miniquad) - main crate, engines below build on top of it. Supports WASM. Therefore everything build on top of it supports WASM too.
- [macroquad](https://github.com/not-fl3/macroquad) - simple to use library from author of `miniquad`.
- [good-web-game](https://github.com/not-fl3/good-web-game) - crate to easily port your [ggez](https://github.com/ggez/ggez) to WASM. You shouldn't use this crate when you creating new project.
- [emerald](https://github.com/Bombfuse/emerald) - game engine with physics, audio, graphics, ECS.
- [nonaquad](https://github.com/nokola/nonaquad) - vector anti-aliased graphics renderer.

## Games

- [Rusty Demon Attack](https://github.com/TanTanDev/rusty_demon_attack) - A game inspired by the classic atari game: demon attack.
- [Fermi Paradox](https://github.com/tversteeg/ld46) - arcanoid-like game with moving enemies in space.
- [Zemeroth](https://github.com/ozkriff/zemeroth) - turn-based hexagonal tactical game.
- [Dig Escape](https://github.com/TanTanDev/DigEscape) - simple puzzle game about digging.
- [Fish Game](https://github.com/heroiclabs/fishgame-macroquad) - online multiplayer game, created as a demonstration of [Nakama](https://heroiclabs.com/), an open-source scalable game server.
- [Crate Before Attack](https://cratebeforeattack.com) - worms-like multiplayer game where frogs combat their friends while navigating a landscape with their sticky tongue. It is a hybrid of a realtime and turn-based game. 
- [Vollmond](https://puppetmaster.itch.io/vollmond) - small non violent adventure in the style of Zelda 2.
- [rymd](https://profan.itch.io/rymd) - space shooter game prototype.
- [Scream mr. Jack](https://kakoeimon.itch.io/scream-mr-jack) - ???.
- [Power Kick](https://kakoeimon.itch.io/power-kick) - platformer fighting game.
- [Soldank](https://github.com/smokku/soldank) - a remake of Soldat game, made using macroquad and laminar

## Visualizations

- [Portal Explorer](https://github.com/optozorax/portal) - web visualizator of mind-blowing portals.
- [Rusty Aquarium](https://github.com/ollej/rusty-aquarium) - a monitoring visualization as an aquarium.

## Apps

- [Particles editor](https://github.com/not-fl3/particles-editor) for your games in macroquad.
- [bema](https://github.com/yazgoo/bema) - slideshow DSL.
- [Rusty Slider](https://github.com/ollej/rusty-slider) - markdown slideshow viewer.

## Docs

- [Platformer book](https://github.com/not-fl3/platformer-book) - WIP book about creating your platformer game in macroquad.

## Publications

- [Rust Gamedev Podcast 4: Interview with Fedor Logachev](https://rustgamedev.com/episodes/interview-with-fedor-logachev)
- Video: [I learnt OpenGL in 7 days using Rust](https://youtube.com/watch?v=KEQIWqSq42k) by [@TanTanDev](https://github.com/TanTanDev/).

## Example usage

- [With naia](https://github.com/naia-rs/naia-macroquad-example) - a cross-platform (including Wasm!) networking engine built in Rust.
- [With nakama](https://github.com/heroiclabs/fishgame-macroquad) - open-source scalable game server.
- [JS interop](https://github.com/not-fl3/miniquad-js-interop-demo) for writing your plugins.
- [wasm-bindgen interop](https://github.com/smokku/gwg-bindgen) - GWG + wasm-bindgen example

## Libraries

- [bevy_miniquad](https://github.com/smokku/bevy_miniquad) - [Bevy engine](https://github.com/bevyengine/bevy) + miniquad render plugin.
- [gesture-recogrizer](https://github.com/optozorax/gesture-recognizer) - library for recognizing simple touch gestures.
- [sapp-console-log](https://github.com/canadaduane/sapp-console-log) - [log-rs](https://github.com/rust-lang/log) compatible logging for sapp-wasm.
- [egui-miniquad](https://github.com/not-fl3/egui-miniquad) - [egui](https://github.com/emilk/egui) in [miniquad](https://github.com/not-fl3/miniquad).
- [egui-macroquad](https://github.com/optozorax/egui-macroquad) - [egui](https://github.com/emilk/egui) in [macroquad](https://github.com/not-fl3/macroquad).
- [miniquad_text_rusttype](https://github.com/not-fl3/miniquad_text_rusttype) - [rusttype](https://github.com/redox-os/rusttype) in [miniquad](https://github.com/not-fl3/miniquad).
- [quad-rand](https://github.com/not-fl3/quad-rand) - wasm-friendly random number generator for quads.
- [imgui miniquad](https://github.com/not-fl3/imgui-miniquad-render) - [imgui-rs](https://github.com/imgui-rs/imgui-rs) in [miniquad].
- [circle2D](https://github.com/koalefant/circle2d) - little physics library with only circles, used in [Crate Before Attack](https://cratebeforeattack.com).

## Plugins

Plugin has additional `.js` file, so to use it, you need to do extra work. Before deploying of your project on WASM, you could look at your dependencies using `cargo tree` and find these crates.

* [`sapp-jsutils`](https://github.com/not-fl3/sapp-jsutils/) - to build plugins. If you want to send/receive string or arbitrary object to JS, you should look at this.
* [`quad-snd`](https://github.com/not-fl3/quad-snd) - to play sound.
* [`quad-net`](https://github.com/not-fl3/quad-net) - to use network.
* [`quad-url`](https://github.com/optozorax/quad-url) - to change current url, and open links.
