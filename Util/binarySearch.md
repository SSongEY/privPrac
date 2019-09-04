이진검색
========

```java
public int binarySearch(int target, int arr[]) {
    int mid;
    int left = 0;
    int right = arr.length - 1;

    while (right >= left) {
        mid = (right+left) / 2;

        if (target == arr[mid]) return mid;
        else if (target < arr[mid])  right = mid - 1;
        else left = mid + 1;
    }

    return -1;
}
```
