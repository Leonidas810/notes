#Problem 

## Solutions

### My first solution (One pointer -  O(n) time - O(n) space)

```
function removeDuplicates(nums: number[]): number { 
	const set = new Set<number>(); 
	nums.map((n) =>{ 
		if(!set.has(n)){ 
			nums[set.size] = n; 
			set.add(n) 
		} 
	});
	return set.size; 
};
```

### Best / canonical solution (Two pointers - O(n) time -  O(1) space)

#### How it works

- *i* scans the array
- *k* tracks where the next unique value should go
- Because the array is **sorted**, duplicates are adjacent

```
function removeDuplicates(nums: number[]): number {
    if (nums.length === 0) return 0;

    let k = 1; // index for unique elements

    for (let i = 1; i < nums.length; i++) {
        if (nums[i] !== nums[i - 1]) {
            nums[k] = nums[i];
            k++;
        }
    }

    return k;
}
```