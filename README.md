# EZ crypto: Cryptography should be easy!

This is a guide (in development) for easy, practical crypto --
I want a complete newbie to be able to get up and running
with a new keypair and various apps in just an hour or so
(and without being intimidated.)

My plan is to publish it as a sub-site on brainonfire.net.

## Philosophy

### Roadblocks

Casual cryptography has two main limitations:

- Tooling: Our current tools *suck*, and not just for the
  inexperienced. How many times have you encrypted an email and
  neglected to encrypt-to-self as well? That should never happen by
  accident.
- Network effect: The more contacts you have who are using crypto for
  communications, the more attractive it becomes for you to
  use. Inversely, if none of your friends are using it, why should
  you?

### Perfection is the enemy of adoption

If you tell someone who has never used GPG that they need to use a
completely random passphrase, they'll never create a key. If you tell
them that they need to verify all key fingerprints before trusting
signatures, they won't bother with signatures.

Most people will not be the subject of targeted surveillance; most
people do not (as of mid-2013) have to worry about man-in-the-middle
attacks; most people do not, in fact, have anything to hide. They'll
be fine using mostly unverified signatures and just-passable
passphrases for now.

Journalists, activists, dissidents, and people working in
high-security industries will be motivated to use more advanced
privacy techniques; the average citizen cannot be -- and need not be.

### Gradual adoption

The bar to entry needs to be extremely low, perhaps even negative. You
can't get most people to change their ways without an obvious and
immediate gain to themselves, so any solution needs to be dead easy --
and possibly even fun. However, once people are using a system, they
can be enticed into using more advanced features. This also allows for
an agile approach: Advanced features and documentation may be
developed after the initial release.

### Standards, etc.

It hardly bears mentioning, but any solution must rely on open-source,
free-licensed technologies. It is also important, although not
essential, that these technologies adhere to formal standards so that
user data is as freely manipulable as the source code of the programs
they are using.

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
