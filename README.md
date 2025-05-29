# `Meet Rust` @ ADC 2024

This is the slideshow code for the presentation I gave at the [Atlanta Developers' Conference](https://www.atldevcon.com/index.html) in 2024 titled `Meet Rust: Getting Started, What's Special, and Why You Should Care`.

Please note that this is not a script, nor does it necessarily contain any portion of my exact talk. It's simply the slides I used for the presentation.

### Viewing the slides

I used `presenterm` for my slides, which is a Markdown-based terminal slideshow tool written purely in Rust, which I felt was appropriate given the subject matter.

You can find more detailed installation instructions in [`presenterm`'s documentation](https://mfontanini.github.io/presenterm/), but if you have the Rust toolchain installed on your device, you should be able to install `presenterm` using the following command:

```shell
cargo install --locked presenterm
```

Once you've installed `presenterm`, you can use the CLI to run any properly-formatted Markdown document as a presentation. For example, to run the slides in this repository, you'd run:

```shell
presenterm meet-rust-adc2024
```

There are also a number of helpful options you can pass in as well, such as `-x` to enable code snippet execution, which allows you to actually run the code you see on the slides (one of my favorite features), or `-e`, which exports the presentation to a PDF file instead of displaying it.

> [!IMPORTANT]
> Not all terminals support the necessary protocols that `presenterm` uses to do things like show images, so you may need to use a different terminal for things to display properly. I ran the presentation on macOS using the [iTerm2](https://iterm2.com/) terminal.

If you want to learn more about `presenterm`, you can check out [the GitHub repository](https://github.com/mfontanini/presenterm) or [their documentation](https://mfontanini.github.io/presenterm/).

## License

Licensed under either of

 * Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.

## Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted for inclusion in the work by you, as defined in the Apache-2.0 license, shall be dual licensed as above, without any additional terms or conditions.