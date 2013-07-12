# EZ crypto: Cryptography should be easy!

This is a guide (in development) for easy, practical crypto --
I want a complete newbie to be able to get up and running
with a new keypair and various apps in just an hour or so
(and without being intimidated.)

My plan is to publish it as a sub-site on brainonfire.net.

## Development

Pull requests welcome, but check with me first before doing a lot of work.

Work to be done:

- UI
  - Sidebars
  - Expandable inline notes and icons? Types:
    - "Good enough for now" - things that aren't perfectly secure,
      but serve most people's uses.
    - "This is a white lie" - with footnote
    - "Glossary term" - with link and/or inline bubble
    - "Trade-off"
  - Fancy UI with all sorts of expanding and collapsing divs
    for different operating systems oh my goodness
- Content
  - Key generation
  - Key distribution
  - Encryption and decryption
  - Key signing
  - Conceptual overview (*very* high level)
  - Glossary
  - Pitfalls

- Backing up private key
  - This doesn't work: gpg --symmetric --armor <(gpg --export-secret-keys --armor )
  - "could not open MIME-encoded message" -- just open from a text editor
- encrypt to self

"There is a small security glitch in the OpenPGP (and therefore GnuPG) system; to avoid this you should always sign and encrypt a message instead of only encrypting it."

## License

© 2013 Tim McCormack, free-licensed under the CC-BY-SA 3.0.
