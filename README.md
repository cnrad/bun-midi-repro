# bun-midi-repro

Steps taken:
`bun i midi`
`bun i --save-dev @types/midi`
`bun run index.ts`

Error:
```zsh
➜  bun-midi-repro git:(master) ✗ bun run index.ts
121 |         throw e;
122 |       }
123 |     }
124 |   }
125 |
126 |   err = new Error(
              ^
error: Could not locate the bindings file. Tried:
 → /Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/build/midi.node
 → /Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/build/Debug/midi.node
 → /Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/build/Release/midi.node
 → /Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/out/Debug/midi.node
 → /Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/Debug/midi.node
 → /Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/out/Release/midi.node
 → /Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/Release/midi.node
 → /Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/build/default/midi.node
 → /Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/compiled/22.6.0/darwin/arm64/midi.node
 → /Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/addon-build/release/install-root/midi.node
 → /Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/addon-build/debug/install-root/midi.node
 → /Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/addon-build/default/install-root/midi.node
 → /Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/lib/binding/node-v127-darwin-arm64/midi.node
 tries: [
  "/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/build/midi.node",
  "/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/build/Debug/midi.node",
  "/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/build/Release/midi.node",
  "/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/out/Debug/midi.node",
  "/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/Debug/midi.node",
  "/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/out/Release/midi.node",
  "/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/Release/midi.node",
  "/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/build/default/midi.node",
  "/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/compiled/22.6.0/darwin/arm64/midi.node",
  "/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/addon-build/release/install-root/midi.node",
  "/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/addon-build/debug/install-root/midi.node",
  "/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/addon-build/default/install-root/midi.node",
  "/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/lib/binding/node-v127-darwin-arm64/midi.node"
],

      at bindings (/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/bindings/bindings.js:126:9)
      at <anonymous> (/Users/conrad/Desktop/cnrad GitHub/bun-midi-repro/node_modules/midi/midi.js:1:5)

Bun v1.2.13 (macOS arm64)
```
