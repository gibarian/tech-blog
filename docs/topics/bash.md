---
title: '- Bash'
---

## Bash shell shortcuts

![Bash Shortcuts](../assets/pages/bash_shortcuts.png)


## EOF - three scenarios

Tabs must be used instead of spaces for indentations

=== "<< EOF"

    >```bash title="code" linenums="1" hl_lines="3"
    >display_lines() {
    >    foo="one"
    >    cat > /dev/stdout << EOF
    >    line1
    >    line2 $foo
    >EOF
    >display_lines
    >}
    >```
    >
    >```bash title="output" linenums="1"
    >❯ ./test.sh
    >        line1
    >        line2 one
    >```

=== "<<- EOF"

    >```bash title="code" linenums="1" hl_lines="3"
    >display_lines() {
    >    foo="one"
    >    cat > /dev/stdout <<- EOF
    >    line1
    >    line2 $foo
    >	 EOF
    >}
    >display_lines
    >```
    >
    >```bash title="output" linenums="1"
    >❯ ./test.sh
    >line1
    >line2 one
    >```

=== "<<- 'EOF'"

    >```bash title="code" linenums="1" hl_lines="3"
    >display_lines() {
    >    foo="one"
    >    cat > /dev/stdout <<- 'EOF'
    >    line1
    >    line2 $foo
    >	 EOF
    >}
    >display_lines
    >```
    >
    >```bash title="output" linenums="1"
    >❯ ./test.sh
    >line1
    >line2 $foo
    >```