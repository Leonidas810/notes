#Problem

## Solutions

### My first solution (Two pointer -  O(n) time - O(1) space)

```
function removeElement(nums: number[], val: number): number {

    let k = 0;
    for (let i = 0; i < nums.length; i++) {
        if (nums[i] === val) k++
	    else nums[i - k] = nums[i];
    }
    return nums.length-k

};
```

### Best / canonical solution (Two pointers - O(n) time -  O(1) space)

#### How it works

- *i* scans the array
- *k* tracks where the next element of the array

```
function removeElement(nums: number[], val: number): number {
    let k = 0;

    for (let i = 0; i < nums.length; i++) {
        if (nums[i] !== val) {
            nums[k] = nums[i];
            k++;
        }
    }

    return k;
}
```

### Slight optimization (when order does NOT matter)
#### How it works

- *i* scans the array
- When you find "val", you change i with n-1, fewer writes

```
function removeElement(nums: number[], val: number): number {
    let i = 0;
    let n = nums.length;

    while (i < n) {
        if (nums[i] === val) {
            nums[i] = nums[n - 1];
            n--;
        } else {
            i++;
        }
    }

    return n;
}

```