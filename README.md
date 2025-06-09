## Dependencies 

To build this resume you need to install [typst](https://github.com/typst/typst). At the time of 
writing this, I had installed `typst` using nix-darwin by adding it to my system packages list 

```
  let
    configuration = { pkgs, config, ... }: {
      environment.systemPackages =
        [ 
            # other packages here ...
            pkgs.typst 
        ]
    }; 
```

### Alternative 

```bash
brew install typst
```

## Building

Use typst to build your source into a pdf by running 

```bash
typst compile resume.typ
```

