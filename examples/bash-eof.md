>bash code:
>```bash
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
>output:
>```bash
>❯ ./test.sh
>        line1
>        line2 one
>```

&nbsp;

>bash code:
>```bash
>display_lines() {
>    foo="one"
>    cat > /dev/stdout <<- EOF
>    line1
>    line2 $foo
>	EOF
>}
>display_lines
>```
>
>output:
>```bash
>❯ ./test.sh
>line1
>line2 one
>```

&nbsp;

>bash code:
>```bash
>display_lines() {
>    foo="one"
>    cat > /dev/stdout <<- 'EOF'
>    line1
>    line2 $foo
>	EOF
>}
>display_lines
>```
>
>output:
>```bash
>❯ ./test.sh
>line1
>line2 $foo
>```
