## 2025.11.19

<details>
<summary>Blog Post 1</summary>
<p>This is the content of the first post.</p>


bash code:
```bash
display_lines() {
    foo="one"
    cat > /dev/stdout << EOF
    line1
    line2 $foo
EOF
display_lines
}
```

output:
```bash
❯ ./test.sh
        line1
        line2 one
```
---

bash code:
```bash
display_lines() {
    foo="one"
    cat > /dev/stdout <<- EOF
    line1
    line2 $foo
	EOF
}
display_lines
```

output:
```bash
❯ ./test.sh
line1
line2 one
```

---

bash code:
```bash
display_lines() {
    foo="one"
    cat > /dev/stdout <<- 'EOF'
    line1
    line2 $foo
	EOF
}
display_lines
```

output:
```bash
❯ ./test.sh
line1
line2 $foo
```

</details>

---


<details>
<summary>Blog Post 1</summary>
<p>This is the content of the first post.</p>
</details>

<details>
<summary>Blog Post 2</summary>
<p>This is the content of the second post.</p>
</details>


---
