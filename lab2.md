## Part 1


## Part 2
This is the code block for a failure-inducing bug as a Junit test for the reverseInPlace method in ArrayExamples.java.
```
@Test
public void testReverseInPlace2() {
  int[] input = {1, 2, 3};
  ArrayExamples.reverseInPlace(input);
  assertArrayEquals(new int[] {3, 2, 1}, input);
}
```

This is a code block for an input that doesn't induce a failure as a Junit test for the reverseInPlace method in ArrayExamples.java.
```
@Test 
public void testReverseInPlace() {
  int[] input1 = { 3 };
  ArrayExamples.reverseInPlace(input1);
  assertArrayEquals(new int[]{ 3 }, input1);
}
```

This is the symptom, or the output of running the 2 Junit tests above.
Buggy input:
![image](buggy_testReversed.png)

Correct input:
![image](correct_testReversed.png)

These are the before and after code blocks of the bug for the reverseInPlace method.
Before (buggy):
```
static void reverseInPlace(int[] arr) {
  for(int i = 0; i < arr.length; i += 1) {
    arr[i] = arr[arr.length - i - 1];
  }
}
```

After (fixed):
```
static void reverseInPlace(int[] arr) {
  for(int i = 0; i < arr.length/2; i += 1) {
    int temp = arr[i];
    arr[i] = arr[arr.length - i - 1];
    arr[arr.length - i - 1] = temp;
  }
}
```

## Part 3
From both last week's and this week's lab, I learned how to fork a page from Github and how to use Github Desktop to clone a repository. Prior to this class, I didn't really have much experience with using Github Desktop or Github Pages, so I enjoyed getting hands on experience with this through this class.
