# Custom macOS keyboard layouts

The following keyboard layouts offer practical functionality to Dvorak typists and users of small keyboards on macOS.

Since these layouts run on your macOS machine, they can be used simultaneously to any custom firmware you've installed on an external keyboard, no configuration necessary.

## Installation

First, bundles need to be placed in the `/Library/Keyboard Layouts` directory. 

Restart your machine.

Then install the layout by navigating to `System Settings > Keyboard > Keyboard layouts`. Click on the `+` button to add a new input source, then locate custom layouts in the `Others` category.


## Dvorak International

`Dvorak International` makes it easier to type a number of diacritics and accents used in French, Spanish, and other languages. It does this by imitating the same system of dead-keys which many QWERTY users know thanks to the `U.S. International - PC` layout. These include the following:

- `'` for acute accent (`é`) and cedilla (`ç`)
- `` ` `` for grave accent (`è`)
- `^` for circumflex (`ê`)
- `"` for dieresis (`ë`)
- `~` for tilde diacritic (`ñ`)

The layout also includes QWERTY commands.


## 30% International

`30% International` is a diacritics-focused layout based on `U.S. International` with small keyboards in mind (e.g. 30% or 40%). Its key features are the following:

- The layout offers the option to exclusively use alpha-block inputs for dead keys. This makes diacritics more accessible than in `U.S. International`, where characters like caret `^` and tilde `~` are used.
- `30% International` also includes additional inputs not included in `U.S. International` in order to simplify typing guillemets and non-braking spaces.

The layout is meant to be used with external keyboards, and as such it is QWERTY; any alternate layouts can be implemented directly on the external keyboard's controller.

### 30% diacritics

All regular international diacritics dead-keys remain; only additional alternatives are added. The following are the regular international dead-keys:

- `'` for acute accent (`é`) and cedilla (`ç`)
- `` ` `` for grave accent (`è`)
- `^` for circumflex (`ê`)
- `"` for dieresis (`ë`)
- `~` for tilde diacritic (`ñ`)

New 30% dead-key alternatives for hard-to-access keys:

- `;` for circumflex (`ê`).
- `,` for grave accent (`è`).
- `<` (`shift-comma`) for tilde diacritic (`ñ`)

Using punctuation symbols like `;` and `,` as dead keys should not impact the usual flow of writing since a space is automatically inserted behind them when they are terminated (spaces aren't added when others dead keys are terminated). This avoids having to hit the space bar twice in a row.


## 30% International+

`30% International+` includes a few extra features not in `30% International`. The two layouts are separate not only because not all users will find the additional features helpful, but also because dead keys can sometimes cause issues, especially in input fields on the web. It's therefore often best to keep them to a minimum in order to avoid scenarios like incorrectly entering a password.

Perhaps ideally, these additional features should be implemented using text replacement software rather than directly in the layout. That said, installing `30% International+` is an easier option.

Additional features:

- The apostrophe key `'` produces a typographic apostrophe `’` (`U+2019`, or right single quotation mark) when terminated with the space bar. In order to obtain a regular apostrophe (`U+0027`), terminate with the escape key or some other letter. (`30% International` will also input a typographical apostrophe if the apostrophe is hit twice).
- In French, narrow non-breaking spaces (`U+202F`) are regularly used alongside of punctuation, preceding question marks, exclamation points, colons, and semi-colons. To facilitate typing these narrow non-breaking spaces, the aforementioned punctuation marks are turned into dead keys. When tapped once, they output their expected character; when tapped twice, they output a narrow non-breaking space followed by the character.
- Two additional dead-keys are added for other international characters: right angled bracket and left angled bracket. This simplifies the task of typing guillemets, or Spanish and French quotation marks. A double left angled bracket will output a left guillemet `«` followed by a (full-width) non-breaking space; a double right angled bracket will output a right guillemet `»` preceded by a non-breaking space.


## Dvorak FR numbers

As an alternate approach for typing French accents on Dvorak, this layouts replaces the Dvorak number row with an AZERTY number row — or very nearly.

![](images/dvorak-fr-numbers.svg)

A few modifications have been made in order to make the number row more Dvorak compatible.

- Redundant characters are replaced (faded on the diagram above)
- An additional layer is added for more inputs and is activated with a dead key. Among other things, this layer makes typing uppercase accented letters more practical than in AZERTY.


## Dvorak to QWERTY

`Dvorak to QWERTY` allows an external Dvorak keyboard to be used as a QWERTY keyboard even if the QWERTY layout is not included in its firmware.

The layout achieves this conversion by mapping a QWERTY key's position to the QWERTY letter which occupies the position of that same key in the Dvorak layout.
