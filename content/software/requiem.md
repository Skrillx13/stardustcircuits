---
layout: page
---

[Stardust & Circuits](/stardustcircuits/index.html) / [Software](/) / [Requiem](./requiem.html)

# Requiem: Pythonic Common Games

`Requiem` is a Python Library for creating common games. It gives you tools to help you make your games easier It also provides a bit of web framework for you to play your created games in the browser.

## Features

- Supports multiple games, and if requried, you can declare your own components!
- Works smoothly with GitHub workflows, CI/CD, and pipelines.
- Includes some web framework, so you can run your game on a local server.
- Host your Project anywhere, thanks to said web framework.

This wasn't meant to be an extensive game library like [KaplayJS](https://kaplayjs.com) or the like, just meant to be a little fun something. It's aim is just to help people create fun projects with Python, especially for newcomers.

## Getting Started

You can install this project with `pip`, through invoking the following command:

``` console
pip install requiem
```

Here's a simpe example on how you can use this library to create a chess game:

``` python
import chess

board = chess.Board()

board.legal_moves  
<LegalMoveGenerator at ... (Nh3, Nf3, Nc3, Na3, h3, g3, f3, e3, d3, c3, ...)>
chess.Move.from_uci("a8a1") in board.legal_moves
False

board.push_san("e4")
Move.from_uci('e2e4')
board.push_san("e5")
Move.from_uci('e7e5')
board.push_san("Qh5")
Move.from_uci('d1h5')
board.push_san("Nc6")
Move.from_uci('b8c6')
board.push_san("Bc4")
Move.from_uci('f1c4')
board.push_san("Nf6")
Move.from_uci('g8f6')
board.push_san("Qxf7")
Move.from_uci('h5f7')

board.is_checkmate()
True

board
Board('r1bqkb1r/pppp1Qpp/2n2n2/4p3/2B1P3/8/PPPP1PPP/RNB1K1NR b KQkq - 0 4')
```

### Resources

This Project isn't really "actively maintained", but still has some support. I would recommend using a JS library for actual game devlopment though.

- GitHub Repo: [https://github.com/Skrillx13/Requiem](https://github.com/Skrillx13/Requiem)
- Documentation: [https://requiem.readthedocs.io](https://requiem.readthedocs.io)