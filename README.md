[README.md](https://github.com/user-attachments/files/34031051/README.md)
# Randomfella: Free Random Wheel, Coin Flip, Dice, Number Generator & Bingo Caller

**[Randomfella](https://randomfella.com/)** is a set of free online random tools that are fair, secure and quick to use. There is no sign-up and no app to install. Everything works in your browser on phones, tablets and computers, in English, Spanish, French and Arabic.

**Live site: [randomfella.com](https://randomfella.com/)**

## The tools

| Tool | What it does | Link |
| --- | --- | --- |
| **Spin the Wheel** | Random wheel spinner. Add names or options, set weights, pick colours and sounds, and spin to choose a winner. Share a wheel with a link. | [randomfella.com/spin-the-wheel](https://randomfella.com/spin-the-wheel/) |
| **Random Name Picker** | Pick a random name from a list for giveaways, raffles and draws. | [randomfella.com/random-name-picker](https://randomfella.com/random-name-picker/) |
| **Classroom Name Picker** | Choose students fairly in class, without repeats. | [randomfella.com/classroom-name-picker](https://randomfella.com/classroom-name-picker/) |
| **Flip a Coin** | Online coin toss with a 3D coin, heads or tails history and an embed option for other sites. | [randomfella.com/flip-a-coin](https://randomfella.com/flip-a-coin/) |
| **Roll a Dice** | Roll one or many dice of different sizes, with totals and history. | [randomfella.com/roll-a-dice](https://randomfella.com/roll-a-dice/) |
| **Random Number Generator** | Generate random numbers in any range, with or without repeats. Includes an embed option. | [randomfella.com/random-number-generator](https://randomfella.com/random-number-generator/) |
| **Bingo Caller** | Call bingo numbers with a ball animation, a Hall mode for big screens and a record of called numbers. | [randomfella.com/bingo-caller](https://randomfella.com/bingo-caller/) |

## Why people use Randomfella

- **Fair.** Results come from the browser's Web Crypto generator (`crypto.getRandomValues`), a cryptographically secure source, not a simple `Math.random()` shortcut.
- **Honest.** In the default Natural End mode the winner is not decided until the wheel has stopped. Read how it works in [Is This Wheel Actually Random?](https://randomfella.com/guides/is-the-wheel-actually-random/).
- **Private.** No account is needed. Your lists and settings stay in your browser unless you choose to share a link.
- **Free and fast.** No sign-up, light pages, and it works on any modern device.
- **Multilingual.** English, Spanish, French and Arabic (right-to-left supported).

## Guides

Practical articles on randomness, giveaways, games and classroom use:

- [Is This Wheel Actually Random? How the Spin Is Generated](https://randomfella.com/guides/is-the-wheel-actually-random/)
- [The Fairest Way to Pick a Raffle Winner Online](https://randomfella.com/guides/fair-raffle-winner-online/)
- [Weighted vs. Equal-Odds Wheels: When to Use Each](https://randomfella.com/guides/weighted-vs-equal-odds-wheels/)
- [Running a Prize Wheel Giveaway on Twitch or YouTube Live](https://randomfella.com/guides/prize-wheel-twitch-giveaway/)
- [Prize Wheel Ideas for Kids' Birthday Parties](https://randomfella.com/guides/prize-wheel-kids-birthday-party/)
- [Team Standup Roulette: Picking Who Goes First (Fairly)](https://randomfella.com/guides/team-standup-picker-order/)
- [Top 10 Bingo Variants You Can Play Anywhere](https://randomfella.com/guides/top-10-bingo-variants/)
- [Every Die Explained: From d2 Coins to the 100-Sided Zocchihedron](https://randomfella.com/guides/every-die-explained/)
- [Famous Coin Flips in History](https://randomfella.com/guides/famous-coin-flips-in-history/)

All guides: [randomfella.com/guides](https://randomfella.com/guides/)

## Common uses

Choosing a winner for a giveaway or raffle, picking who goes first, settling a decision with a coin toss, rolling dice for board games and tabletop RPGs, drawing a random number for a game or lottery-style draw, picking a student in class, running a bingo night, and choosing what to eat.

## Embed on your own site

The Flip a Coin and Random Number Generator tools can be embedded with one line:

```html
<script src="https://randomfella.com/flip-a-coin/embed.js" async></script>
<script src="https://randomfella.com/random-number-generator/embed.js" async></script>
```

See the embed pages on the site for options.

## Built with

React 18, Vite, and Netlify (static hosting plus a small serverless function for share links). Each tool is its own app in this repository and shares common code.

| Folder | Contents |
| --- | --- |
| `src/` | Spin the Wheel (main app) |
| `coin/`, `dice/`, `number/`, `bingo/` | Flip a Coin, Roll a Dice, Random Number Generator, Bingo Caller |
| `shared/` | Code used by more than one tool (top bar, language handling, secure random, share pictures) |
| `content/articles/` | Guides, written in Markdown |
| `scripts/` | Build scripts, including the guides and home page generators |
| `netlify/functions/` | Share-link function |

## Run it locally

Requires Node 20 or newer.

```bash
npm install
npm run dev       # Spin the Wheel at http://localhost:5173
npm run build     # builds every tool into dist/
npm run preview   # serves the full built site
npm test          # runs the test suite
```

More detail, including testing, deployment and project notes, is in [docs/DEVELOPMENT.md](docs/DEVELOPMENT.md).

## Contributing and feedback

Found a bug or have an idea for a new random tool? [Open an issue](../../issues). Translation corrections for Spanish, French and Arabic are especially welcome.

---

**Randomfella** · [randomfella.com](https://randomfella.com/) · Free random wheel, coin flip, dice roller, random number generator and bingo caller.
