{\rtf1\ansi\ansicpg932\cocoartf2822
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;\f1\fnil\fcharset0 .SFNS-Semibold;\f2\fnil\fcharset0 .SFNS-Regular;
\f3\fnil\fcharset0 .AppleSystemUIFontMonospaced-Regular;\f4\fnil\fcharset0 HelveticaNeue-Bold;}
{\colortbl;\red255\green255\blue255;\red14\green14\blue14;}
{\*\expandedcolortbl;;\cssrgb\c6700\c6700\c6700;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 # Auto Linker for Obsidian\
\
**English**  \
An Obsidian community plugin that automatically converts keywords in your notes into `[[internal links]]` based on a custom dictionary note.  \
Originally created together with AI (Codex CLI) as an experiment in co-creation, it now helps your vault \'93grow beautifully\'94 by turning repeated words into consistent links.\
\
**\uc0\u26085 \u26412 \u35486 **  \
Obsidian\uc0\u12398 \u12494 \u12540 \u12488 \u20869 \u12391 \u12424 \u12367 \u20351 \u12358 \u12461 \u12540 \u12527 \u12540 \u12489 \u12434 \u12289 \u36766 \u26360 \u12494 \u12540 \u12488 \u12395 \u22522 \u12389 \u12356 \u12390 \u33258 \u21205 \u30340 \u12395  `[[\u20869 \u37096 \u12522 \u12531 \u12463 ]]` \u12395 \u22793 \u25563 \u12377 \u12427 \u12503 \u12521 \u12464 \u12452 \u12531 \u12391 \u12377 \u12290   \
\uc0\u12418 \u12392 \u12418 \u12392 \u12399 AI\u65288 Codex CLI\u65289 \u12392 \u19968 \u32210 \u12395 \u23455 \u39443 \u30340 \u12395 \u20316 \u12387 \u12383 \u12418 \u12398 \u12391 \u12377 \u12364 \u12289 \u20170 \u12391 \u12399 \u12494 \u12540 \u12488 \u12434 \u20445 \u23384 \u12377 \u12427 \u12384 \u12369 \u12391 \u12522 \u12531 \u12463 \u12364 \u25972 \u12356 \u12289 Vault\u12364 \u12300 \u32654 \u12375 \u12367 \u32946 \u12388 \u12301 \u20307 \u39443 \u12434 \u27005 \u12375 \u12417 \u12414 \u12377 \u12290 \
\
---\
\
## \uc0\u10024  Features / \u29305 \u24500 \
- Automatically convert keywords into `[[internal links]]`\
- Dictionary-based mapping (pattern \uc0\u8594  target)\
- Optional `display` names\
- Runs on save (or manually via command palette)\
\
---\
\
## \uc0\u9881 \u65039  Installation / \u23566 \u20837 \u26041 \u27861 \
1. Download or clone this repository.  \
2. Copy the `auto-linker` folder into your Vault\'92s `.obsidian/plugins/`.  \
3. Restart Obsidian.  \
4. Enable **Community plugins** in Obsidian settings.  \
5. Configure the dictionary note path (default: `Meta/Link Dictionary.md`).  \
\
---\
\
## \uc0\u55357 \u56541  Example Dictionary / \u36766 \u26360 \u12494 \u12540 \u12488 \u20363 \
\
```markdown\
| pattern | target            | display  | note |\
|---------|------------------|----------|------|\
| \uc0\u35036 \u21161 \u37329   | [[\u35036 \u21161 \u37329 \u21161 \u25104 \u37329 ]] | \u35036 \u21161 \u37329    | \u35036 \u21161 \u37329 \u31995 \u20840 \u33324    |\
| AI\uc0\u39015 \u21839  | [[AI\u39015 \u21839 ]]       |          | \u39015 \u21839 \u12469 \u12540 \u12499 \u12473 \u29992  |\
| \uc0\u31070 \u25144    | [[\u31070 \u25144 ]]          |          | \u22320 \u21517            |\
\
\pard\tx560\tx1120\tx1680\tx2240\tx2800\tx3360\tx3920\tx4480\tx5040\tx5600\tx6160\tx6720\sl324\slmult1\pardirnatural\partightenfactor0

\f1\b\fs34 \cf2 \uc0\u55357 \u57056 \u65039  Notes / \u27880 \u24847 \u28857 
\f2\b0\fs28 \
\pard\tqr\tx100\tx260\li260\fi-260\sl324\slmult1\sb240\partightenfactor0
\cf2 	\'95	The dictionary note itself is ignored (to prevent self-replacement).\
	\'95	
\f3 target
\f2  must always be written in 
\f3 [[...]]
\f2  format.\
	\'95	If you want to test before saving, enable \'93dry-run\'94 mode in plugin settings.\
\pard\tx560\tx1120\tx1680\tx2240\tx2800\tx3360\tx3920\tx4480\tx5040\tx5600\tx6160\tx6720\pardirnatural\partightenfactor0

\f0\fs24 \cf0 \
\uc0\u11835 \
\pard\tx560\tx1120\tx1680\tx2240\tx2800\tx3360\tx3920\tx4480\tx5040\tx5600\tx6160\tx6720\sl324\slmult1\pardirnatural\partightenfactor0

\f2\fs28 \cf2 \

\f1\b\fs34 \uc0\u55357 \u56420  Author / \u20316 \u32773 
\f2\b0\fs28 \
\
Created by 
\f4\b Hiro (\uc0\u12402 \u12429 )
\f2\b0  + Codex AI\
2025, Kobe, Japan\
\
X account https://x.com/bonds_ai}