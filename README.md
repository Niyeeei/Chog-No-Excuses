# Chog: No Excuses

An unofficial fan game for Chogathon 2026. Your Chog Genesis NFT is the character: its traits decide your stats, perks and signature move.

## How the NFT is essential
- Connect a wallet (read-only) and the game scans the Chog Genesis contract on Monad mainnet for your tokens, or look up any token number to preview it.
- Token metadata and art are loaded live from IPFS. Nothing is copied or stored.
- Traits become stats:
  - Body + Base -> might (tray width, speed)
  - Eyes + Accessory -> cunning (loot magnet, how fast your move charges)
  - Head + Mouth -> charm (score multiplier)
  - Tier (Common to Legendary) -> bonus to every stat, starting shield from Epic. Three lives per run; a heart brings back a lost life (max 3)
  - Head trait picks the signature move (Chaos Burst, Slow Moon, Order Shield, Coin Rain)
  - Some trait names add perks (visors, wizard hat, dollar cap, heart eyes, dead eyes, fwog)
- Alter egos (picked before each run): Reckless, Paper Hands, Whale (needs an accessory), Sneaky Bandit (needs shades, glasses or a visor). Tier scales their strength from x1.0 (Common) to x2.0 (Legendary). Optional dares (Coin Hater, Combo Addict, Sharpshooter) add a score bonus.
- Fireball (Fire button or F): burns Rug Wraiths for points. Recharge time comes from might and tier. A wizard hat makes fireballs pierce. Reckless fires faster.
- Easy start: the home screen has four clear choices (Play now, Use my Chog, Pick a sample chog, Create a chog). The chog page has a Start button at the top and a how-to-play box. Quit is available during a run.
- Challenges: after a run, "Copy challenge link" makes a link like https://your-site/#c=CHOG-1462-840-K7. Opening it shows a "can you beat it?" banner. Pasting a link or a code into the compare box also works.
- When the last life ends, Chog dances on the game-over screen (an original shuffle; no official Chog dance was found).
- The play screen hides the page header and sizes itself to the window height so the whole game fits without scrolling.
- Guest players can build a Common-tier demo Chog with the "Create a chog" screen. Demo runs (sample Chogs, custom Chogs, token previews) are not saved.
- Verified owners (a connected wallet that holds the Chog) keep XP, level, best score, the daily quest and the "still here?" streak on their device, and get the real-art score card.
- Without a Chog Genesis you can only try the demo. The NFT supplies the stats, the move, the real art and the saved progress.

## Contract facts (checked against Monad mainnet)
- Chain id 143, RPC https://rpc.monad.xyz
- Chog Genesis: 0xc96d31F8626c6D03Fae5dCD3d61e3FB9F4a73763, supply 1,969
- The contract is not enumerable, so finding a wallet's tokens scans ownerOf in small batches.

## Safety
- Read-only. No signing, no transactions, no token spend.
- Unofficial. Chog and Chog Genesis belong to the Chog team. Supporting characters are original.

## Change the name
Edit `GAME_NAME` near the top of the script in `index.html`, and the `<title>`.

## Publish it (about 10 minutes)
1. Create a free account at github.com.
2. New repository -> name it `chog-catcher` -> Public -> Create.
3. "uploading an existing file" -> drag in `index.html` and `README.md` -> Commit.
4. Go to vercel.com -> Sign up with GitHub -> Add New Project -> pick `chog-catcher` -> Deploy.
5. Vercel gives you a link like `https://chog-catcher.vercel.app`. Open it on your phone and your computer.

(GitHub Pages also works: repository Settings -> Pages -> Deploy from branch -> main.)

## Submission checklist
- [ ] Project name and banner
- [ ] Description (up to 8,000 characters)
- [ ] Demo video, 3 minutes or less (YouTube unlisted or Google Drive)
- [ ] App link (Vercel link)
- [ ] GitHub repo link and tech stack (plain HTML, CSS, JavaScript, canvas, Monad JSON-RPC)
- [ ] Contact email and judge access instructions (say: the demo needs no wallet; look up any token number to preview a real Chog; owners connect a wallet for saved progress)
- [ ] Submit before 23 October 2026, 15:00 UTC (confirm on the official page)
