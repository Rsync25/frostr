# FROSTR

Use `Flexible Round Optimized Schnorr Threshold` (FROST) signatures to create a threshold multisignature (`t-of-n`) nostr account with your friends.

To make a post/event, you require `t-of-n` parties to individually sign.

**Extremely unsafe and violently untested**

Please do not add this to any nostr client list.

## Usage
```
git clone https://github.com/nickfarrow/frostr
```
then `cargo run` or
```
cargo install --path .
frostr
```
Choose menu options 0-1, copy-paste and share things between participants. Take care of only sharing "secrets" with the intended recipient!

## More about FROST
[FROST Paper](https://eprint.iacr.org/2020/852.pdf)
[Docs for our implementation & some important notes](https://docs.rs/schnorr_fun/latest/schnorr_fun/frost/index.html)

## todo (you?)
- [x] Sign a valid nostr event using FROST
- [ ] Refactor requests for input, buffers, and whitespace
- [ ] Proper CLI
- [ ] Colorful terminal
- [ ] Allow users to sign more arbitrary events (e.g. change profile)
- [ ] Allow users to sign non-nostr related messages
- [ ] Remove unwraps everywhere
- [ ] Show list of available frost keys