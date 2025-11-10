# dfaRunner
Run words through a DFA specified in a given toml file.
## toml Format
The format is fairly simple, here's an example of it.
```toml
states = ["s", "q", "r"]
accept = ["q"]
start = "s"
language = ["a", "b"]
transitions = ["s-(a)->s", "s-(b)->q", "q-(a)->r", "q-(b)->q", "r-(a)->r", "r-(b)->r"]
```

## Installation
Run `pip install git+https://github.com/chrispo-git/dfa-runner`

## Usage
`dfaRunner "TOML" "WORD"`
