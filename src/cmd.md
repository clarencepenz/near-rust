near create-account crossword.ogenienis.testnet --masterAccount ogenienis.testnet

near state crossword.ogenienis.testnet

near deploy crossword.ogenienis.testnet --wasmFile res/near_rust.wasm


near view crossword.ogenienis.testnet get_puzzle_number

near call crossword.ogenienis.testnet set_solution '{"solution": "near nomicon ref finance"}' --accountId ogenienis.testnet

near call crossword.ogenienis.testnet guess_solution '{"solution": "near nomicon ref finance"}' --accountId ogenienis.testnet

near call crossword.ogenienis.testnet guess_solution '{"solution": "ce"}' --accountId ogenienis.testnet

near delete crossword.ogenienis.testnet ogenienis.testnet


near call crossword.ogenienis.testnet new '{"solution": "69c2feb084439956193f4c21936025f14a5a5a78979d67ae34762e18a7206a0f"}' --accountId crossword.ogenienis.testnet

near deploy crossword.ogenienis.testnet --wasmFile res/near_rust.wasm \
  --initFunction 'new' \
  --initArgs '{"solution": "69c2feb084439956193f4c21936025f14a5a5a78979d67ae34762e18a7206a0f"}'

near view crossword.ogenienis.testnet get_solution