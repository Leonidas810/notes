#Problem 
## Solutions

### My first solution (Two pointer -  O(h * n) time - O(1) space)

```
function strStr(haystack: string, needle: string): number {

    const h = haystack.length;
    const n = needle.length;

    for (let i = 0; i <= h - n; i++) {
        let j = 0;
        while (j < n && haystack[i + j] === needle[j]) j++;
        if (j === n) return i
    }
    return -1

};
```

### Real algorithmic improvement: **KMP** (O(h + n))