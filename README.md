## 2025.11.19

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


<div style="border: 2px solid #4CAF50; padding: 15px; margin-bottom: 20px; background-color: #f9f9f9;">
<h3>Blog Post 1</h3>
<p>This is the content of the first post.</p>
</div>

<div style="border: 2px solid #2196F3; padding: 15px; margin-bottom: 20px; background-color: #eef7ff;">
<h3>Blog Post 2</h3>
<p>This is the content of the second post.</p>
</div>
