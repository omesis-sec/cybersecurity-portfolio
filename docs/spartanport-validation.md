# Testing SpartanPort on Intel UHD Graphics

I tested the fix proposed in [PR #1037](https://github.com/FelipePrado0/SpartanPort/pull/1037) after encountering crashes on my Intel UHD laptop. I recorded the results, shared logs, and wrote instructions to help other users apply it.

## Test setup

- Intel Core i5-12450H and Intel UHD Graphics.
- Windows 11, graphics driver 32.0.101.7088.
- SpartanPort 2.7.0 with fix commit `11f90626fa7c55bffdcab045ab6c3133807cb89a`.
- God of War III Remastered, CUSA01623, update 01.02.

## Results

The logged session lasted about 1 hour and 9 minutes, including menus and pauses. I passed areas that had previously crashed. The log showed nine oversized operations being split into smaller dispatches, with no `VK_ERROR_DEVICE_LOST` recorded. I later completed the game.

Diagnostic collection affected performance on my machine, so I clarified how to launch the game normally and keep diagnostics optional. This was not a controlled FPS benchmark.

## My contribution

My work covered testing, log analysis, documentation, and helping other players. kawanwagnner documented the earlier approach; Tara1903 adapted it into the PR.

- [My test report](https://github.com/FelipePrado0/SpartanPort/issues/334#issuecomment-6391722086).
- [Tara1903's acknowledgement](https://github.com/FelipePrado0/SpartanPort/issues/334#issuecomment-6400333786).
