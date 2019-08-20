# haskell-note

## IDE

### HIE
- **Function Type Check**: Ensure hie ghc version is the same as project ghc version (hie should be install via nix, and can be switch version via hie-wrapper)

- **Import module type**: Ensure hie hoogle is install
  - cd into `haskell-ide-engine` project that you have cloned from github(when you install hie for the first time)
  - Install hoogle for particular ghc version (ex: 8.4.3): 
    `stack --stack-yaml=stack-8.4.3.yaml install hoogle`
  - Generate hoogle for that ghc version:
    `stack --stack-yaml=stack-8.4.3.yaml exec hoogle generate`
