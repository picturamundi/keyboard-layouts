# Custom macOS keyboard layouts

The following keyboard layouts offer practical functionality to Dvorak typists, Arabic typists, and users of small keyboards on macOS.

Since these layouts run on your machine, they can be used simultaneously to any custom firmware you've installed on an external keyboard, no configuration necessary.

All layouts were made with (and can be edited with) [Ukelele](https://software.sil.org/ukelele/).

Documentation quick-links: 

- [Dvorak International](#dvorak-international)
- [30% International](#30-international)
- [Dvorak FR numbers](#dvorak-fr-numbers)
- [Dvorak to QWERTY](#dvorak-to-qwerty)
- [Arabic – Vowelized](#arabic--vowelized)

## Installation

Select the layout you wish to install from the list of `.zip` files above or by clicking on the relevant heading in this document, then click the download button on the top right or the `view raw` link. Unzipping the downloaded archive will reveal a file with the `.bundle`extension.

Bundles need to be placed in the `/Library/Keyboard Layouts` directory.

Restart your machine.

Then install the layout by navigating to `System Settings > Keyboard > Keyboard layouts`. Click on the `+` button to add a new input source, then locate and select custom layouts in the bottommost `Others` category. Once this is done, you should be able to switch to the custom layout by clicking on the keyboard input icon in the menubar.

To visualize a layout after installing, click the keyboard input icon in the menubar and select  `Show Keyboard Viewer` from the dropdown menu.

## [Dvorak International](https://github.com/picturamundi/keyboard-layouts/blob/main/Dvorak%20International.bundle.zip)

`Dvorak International` makes it easier to type a number of diacritics and accents used in French, Spanish, and other languages. It does this by imitating the same system of dead-keys which many QWERTY users know thanks to the `U.S. International - PC` layout. These include the following:

- `'` for acute accent (`é`) and cedilla (`ç`)
- `` ` `` for grave accent (`è`)
- `^` for circumflex (`ê`)
- `"` for dieresis (`ë`)
- `~` for tilde diacritic (`ñ`)

The layout also includes QWERTY commands.


## [30% International](https://github.com/picturamundi/keyboard-layouts/blob/main/30%25%20International.bundle.zip)

`30% International` is a diacritics-focused layout based on `U.S. International` with small keyboards in mind (e.g. 30% or 40%). Its key features are the following:

- The layout offers the option to exclusively use alpha-block inputs for dead keys. This makes diacritics more accessible than in `U.S. International`, where characters like caret `^` and tilde `~` are used.
- `30% International` also includes one additional input not included in `U.S. International` in order to simplify typing typographic apostrophes[^1].

[^1]: This layout originally included a number of other additional features for typing tricky characters from various European languages, such as guillemets, non-breaking spaces, and narrow non-breaking spaces following certain punctuation marks. For various reasons, I now believe it is preferable to implement these features using text-replacement software, rather than baking them into keyboard firmware itself.

The layout is meant to be used with external keyboards, and as such it is QWERTY; any alternate layouts can be implemented directly on the external keyboard's controller.

### 30% diacritics

All regular international diacritics dead-keys remain; only additional alternatives are added. The following are the regular international dead-keys:

- `'` for acute accent (`é`) and cedilla (`ç`)
- `` ` `` for grave accent (`è`)
- `^` for circumflex (`ê`)
- `"` for dieresis (`ë`)
- `~` for tilde diacritic (`ñ`)

New dead-key alternatives for hard-to-access keys include:

- `,` for grave accent (`è`)
- `;` for circumflex (`ê`)
- `:` for tilde diacritic (`ñ`)

Using punctuation symbols like comma, semi-colon, and colon as dead keys does not impact the usual flow of writing since a space is automatically inserted behind them when they are terminated (spaces aren't added when others dead keys are terminated). This avoids needing to hit the space bar twice in a row: once to terminate and again in order to insert the space character.

Additional features:

- The apostrophe key `'` produces a typographic apostrophe `’` (`U+2019`, or right single quotation mark) when tapped twice.

<!-- Perhaps ideally, these additional features should be implemented using text replacement software rather than directly in the layout:

- In French, narrow non-breaking spaces (`U+202F`) are regularly used alongside of punctuation, preceding question marks, exclamation points, colons, and semi-colons. To facilitate typing these narrow non-breaking spaces, the aforementioned punctuation marks are turned into dead keys. When tapped once, they output their expected character; when tapped twice, they output a narrow non-breaking space followed by the character.
- Two additional dead-keys are added for other international characters: right angled bracket and left angled bracket. This simplifies the task of typing guillemets, or Spanish and French quotation marks. A double left angled bracket will output a left guillemet `«` followed by a (full-width) non-breaking space; a double right angled bracket will output a right guillemet `»` preceded by a non-breaking space. -->


## [Dvorak FR numbers](https://github.com/picturamundi/keyboard-layouts/blob/main/Dvorak%20FR%20numbers.bundle.zip)

As an alternate approach for typing French accents on Dvorak, this layouts replaces the Dvorak number row with an AZERTY number row — or very nearly.

![](images/dvorak-fr-numbers.svg)

A few modifications have been made in order to make the number row more Dvorak compatible.

- Redundant characters are replaced (faded on the diagram above)
- An additional layer is added for more inputs and is activated with a dead key. Among other things, this layer makes typing uppercase accented letters more practical than in AZERTY.


## [Dvorak to QWERTY](https://github.com/picturamundi/keyboard-layouts/blob/main/Dvorak%20to%20QWERTY.bundle.zip)

`Dvorak to QWERTY` allows an external Dvorak keyboard to be used as a QWERTY keyboard even if the QWERTY layout is not included in its firmware.

The layout achieves this conversion by mapping a QWERTY key's position to the QWERTY letter which occupies the position of that same key in the Dvorak layout.

## [Arabic – Vowelized](https://github.com/picturamundi/keyboard-layouts/blob/main/Arabic%20%E2%80%93%20Vowelized.bundle.zip)

`Arabic - Vowelized` facilitates typing vowelized Arabic text on a QWERTY keyboard. Below is a summary of its 3 core features: 

1. Based on QWERTY 
    - The QWERTY `s` key outputs `س`, `n` key outputs `ن`, etc.
    - Also includes QWERTY commands: shortcuts like `Cmd-c` and `Cmd-v` still work.
2. Reduces the use of modifier keys for vowels and other diacritics.
    - Vowels are accessible without mods: `a` key outputs _fatha_ ` ـَ`, `i` key outputs _kasra_ `ـِ`, etc.
    - Typing a _hamza_ `ء` before letters _alif_ `ا`, _alif maqsura_ `ى`, or _waw_ `و`, will produce the corresponding characters with a _hamza_ diacritic: `أ` `ئ` `ؤ`.
    - Modifiers continue to be used for nuntation `ـً` `ـٍ` `ـٌ` (`Opt-a`, `Opt-i`, `Opt-u`)and `إ` (`Shift-i`). There is also the option to use `Shift-o` (i.e. `Shift-ء`) for `أ`.
3. Aims to be phonetically and ergonomically intuitive in how long vowels, double consonants, and pharyngeal consonants are typed.
    - Long vowels: typing `aa` will output a long a vowel `ـَا`, typing `AA` will output long vowel `آ`, typing `oo` will output a long o vowel `ـَوْ`, etc. 
    - Double consonants: typing `tt` will output `تّ`, etc.
    - Pharyngeal consonants: while lowercase `h` will output `ه`, uppercase `H` will output  `ح`, etc.

Keep in mind that this layout was created with the Shuwa dialect of Arabic in mind. Among other things, this explains why the letter `ق` is mapped to `g` instead of `q`, or why there are long o and long e vowels.
