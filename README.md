<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:050505,50:050505,100:d8f96a&height=240&section=header&text=NoTrace&fontSize=88&fontColor=ffffff&fontAlignY=38&desc=stealth%20addresses%20on%20solana&descAlignY=62&descSize=18&animation=fadeIn" width="100%" alt="banner"/>

<a href="https://github.com/NoTraceSol">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=1000&color=d8f96a&center=true&vCenter=true&width=860&lines=publish+one+meta-key.;receive+at+infinite+one-time+addresses.;ECDH+on+ed25519+%E2%80%94+ERC-5564+ported+home.;self-custodial.+no+relayer.+no+mixer." alt="typing"/>
</a>

<br/><br/>

<a href="https://notracesol.xyz"><img src="https://img.shields.io/badge/website-notracesol.xyz-d8f96a?style=flat-square&labelColor=050505" alt="site"/></a>
<a href="https://github.com/NoTraceSol/notrace-app/stargazers"><img src="https://img.shields.io/github/stars/NoTraceSol/notrace-app?style=flat-square&color=d8f96a&labelColor=050505&label=stars" alt="stars"/></a>
<a href="https://github.com/NoTraceSol?tab=followers"><img src="https://img.shields.io/github/followers/NoTraceSol?style=flat-square&color=d8f96a&labelColor=050505&label=followers" alt="followers"/></a>
<a href="https://github.com/NoTraceSol"><img src="https://komarev.com/ghpvc/?username=NoTraceSol&label=views&color=d8f96a&style=flat-square" alt="views"/></a>

</div>

<br/>

```ts
// publish your meta-key once. receive forever.
const meta = generateMetaKey()            // your stealth identity
const link = `https://notracesol.xyz/pay#m=${bs58encode(meta.pub)}`

// senders derive a fresh one-time address from your link
// — every payment lands somewhere new on chain
// — only your view-key can find them
// — no mixer, no relayer, no contract
```

<br/>

<!-- contribution snake -->
<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/NoTraceSol/NoTraceSol/output/github-contribution-grid-snake-dark.svg">
  <img alt="snake" src="https://raw.githubusercontent.com/NoTraceSol/NoTraceSol/output/github-contribution-grid-snake.svg" width="100%"/>
</picture>
</div>

<br/>

## ⌬ &nbsp; stats

<div align="center">
<img height="170" src="https://github-readme-stats.vercel.app/api?username=NoTraceSol&show_icons=true&theme=transparent&hide_border=true&bg_color=050505&title_color=d8f96a&icon_color=d8f96a&text_color=c9d1d9&include_all_commits=true&rank_icon=github"/>
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=NoTraceSol&layout=compact&theme=transparent&hide_border=true&bg_color=050505&title_color=d8f96a&text_color=c9d1d9&langs_count=6"/>
</div>

<div align="center">
<img src="https://github-readme-streak-stats.herokuapp.com/?user=NoTraceSol&theme=transparent&hide_border=true&background=050505&stroke=d8f96a&ring=d8f96a&fire=d8f96a&currStreakLabel=d8f96a"/>
</div>

<br/>

## ⌬ &nbsp; the protocol

<table>
<tr>
<td width="33%" valign="top">

#### [notrace-app](https://github.com/NoTraceSol/notrace-app)
<a href="https://github.com/NoTraceSol/notrace-app">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=NoTraceSol&repo=notrace-app&theme=transparent&hide_border=true&title_color=d8f96a&icon_color=d8f96a&text_color=c9d1d9&bg_color=050505"/>
</a>

</td>
<td width="33%" valign="top">

#### [stealth-core](https://github.com/NoTraceSol/stealth-core)
<a href="https://github.com/NoTraceSol/stealth-core">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=NoTraceSol&repo=stealth-core&theme=transparent&hide_border=true&title_color=d8f96a&icon_color=d8f96a&text_color=c9d1d9&bg_color=050505"/>
</a>

</td>
<td width="33%" valign="top">

#### [stealth-sdk](https://github.com/NoTraceSol/stealth-sdk)
<a href="https://github.com/NoTraceSol/stealth-sdk">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=NoTraceSol&repo=stealth-sdk&theme=transparent&hide_border=true&title_color=d8f96a&icon_color=d8f96a&text_color=c9d1d9&bg_color=050505"/>
</a>

</td>
</tr>
</table>

<br/>

## ⌬ &nbsp; how stealth on solana works

```
1.  recipient generates meta-keypair in browser
2.  meta-pub published as URL fragment — notracesol.xyz/pay#m=<base58>
3.  sender opens link, derives one-time stealth_addr via ECDH on ed25519
4.  sender transfers SOL to stealth_addr + memo "nt1:<ephemeral_pub>"
5.  recipient's scanner reads memo, applies ECDH with their meta-priv
6.  on match: derives the spending scalar, sweeps to main wallet

       no contract.  no relayer.  no mixer.  no custody.
       just math from 1976 — ported to solana's native curve.
```

<br/>

## ⌬ &nbsp; references

- [ERC-5564 — Stealth Address Standard](https://eips.ethereum.org/EIPS/eip-5564)
- [Umbra Cash — Stealth on Ethereum](https://app.umbra.cash)
- [Monero stealth addresses](https://www.getmonero.org/resources/moneropedia/stealthaddress.html)
- [@noble/curves — audited curve crypto](https://github.com/paulmillr/noble-curves)

<br/>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:d8f96a,50:050505,100:050505&height=120&section=footer&animation=fadeIn" width="100%" alt="footer"/>

</div>
