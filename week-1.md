# Week 1

## String

### [Disemvowel trolls 7 kyu](https://www.codewars.com/kata/disemvowel-trolls/)

https://www.codewars.com/kata/reviews/52fba700adcd10b182000980/groups/60349f2f9505080001664ad6

### [Mumbling 7 kyu](https://www.codewars.com/kata/mumbling/)

(has another solution) https://www.codewars.com/kata/reviews/5667eafcfde9ebbd5100002e/groups/5cdb25b2efd18d0001b668aa

### [Highest and lowest 7 kyu](https://www.codewars.com/kata/highest-and-lowest/)

(has another solution) https://www.codewars.com/kata/reviews/55565cd093eb1235210000a0/groups/56324433aa1cb7915e000017

### [Isograms 7 kyu](https://www.codewars.com/kata/isograms/)

_(can't get link)_

```javascript
function isIsogram(str) {
  return str
    .toLowerCase()
    .split("")
    .reduce(function(result, element, index) {
      return result && str.toLowerCase().lastIndexOf(element) === index;
    }, true);
}
```

### [Char code calculation 7 kyu](https://www.codewars.com/kata/char-code-calculation)

_(can't get link)_

```javascript
function calc(x) {
  let asciiX = 0;
  let asciiY = 0;

  x.split("").forEach((symb) => {
    asciiX += ("" + symb.charCodeAt(0)).split("").reduce((sum, num) => {
      return sum + 1 * num;
    }, 0);

    asciiY += ("" + symb.charCodeAt(0))
      .replace(/7/g, "1")
      .split("")
      .reduce((sum, num) => {
        return sum + 1 * num;
      }, 0);
  });

  return asciiX - asciiY;
}
```

### [Cat and mouse 2d version 7 kyu](https://www.codewars.com/kata/cat-and-mouse-2d-version/)

### [Duplicate-encoder 6 kyu](https://www.codewars.com/kata/duplicate-encoder)

_(can't get link)_

```javascript
function duplicateEncode(word) {
  let result = "";
  let _word = word.toLowerCase();

  for (let i = 0; i < word.length; i++) {
    let letter = _word[i];
    result += _word.indexOf(letter) === _word.lastIndexOf(letter) ? "(" : ")";
  }

  return result;
}
```

## Number

### [Squares sequence 7 kyu](https://www.codewars.com/kata/squares-sequence)

https://www.codewars.com/kata/reviews/55461869bd94d02501000157/groups/603ddc4ddbbde300015d19de

### [Concatenated sum 7 kyu](https://www.codewars.com/kata/concatenated-sum)

https://www.codewars.com/kata/reviews/59a1f797ce67ef20b300051d/groups/603de42c8f820e00015db448

### [Filter the number 7 kyu](https://www.codewars.com/kata/filter-the-number)

https://www.codewars.com/kata/reviews/55b05294b76b61d1f300004d/groups/603de938dbbde300015d1af2

### [N-th fibonacci 6 kyu](https://www.codewars.com/kata/n-th-fibonacci)

https://www.codewars.com/kata/reviews/522551eee9abb932420004a3/groups/603df590bd84900001f0f151

## Array

### [Playing with sets intersection 7 kyu](https://www.codewars.com/kata/playing-with-sets-intersection)

https://www.codewars.com/kata/reviews/5884e01f7987a27f6900004b/groups/6048a3b250f8fe000184f920

### [Divide and conquer 7 kyu](https://www.codewars.com/kata/divide-and-conquer)

https://www.codewars.com/kata/reviews/57eaeea678748fe4cb000016/groups/6048a6262faf5b0001d5fa38

### [Find the odd int 6 kyu](https://www.codewars.com/kata/find-the-odd-int/)

_(can't get link)_

```javascript
function findOdd(A) {
  return A.sort().reduce((oddNum, element) => {
    return (A.lastIndexOf(element) - A.indexOf(element) + 1) % 2 !== 0
      ? element
      : oddNum;
  });
}
```

### [Find the parity outlier 6 kyu](https://www.codewars.com/kata/find-the-parity-outlier)

_(can't get link)_

```javascript
function findOutlier(integers) {
  for (let i = 1; i < integers.length; i++) {
    if (Math.abs(integers[i]) % 2 !== Math.abs(integers[i - 1]) % 2) {
      if (
        i - 1 === 0 &&
        Math.abs(integers[0]) % 2 !== Math.abs(integers[i + 1]) % 2
      ) {
        return integers[0];
      }

      return integers[i];
    }
  }
}
```

### [ZipWith 6 kyu](https://www.codewars.com/kata/zipwith)

https://www.codewars.com/kata/reviews/58257cfc6620ec730b000067/groups/603e0f145abf6700018dfd81

## Date

### [It is written in the stars 7 kyu](https://www.codewars.com/kata/it-is-written-in-the-stars)

https://www.codewars.com/kata/reviews/5888ac9e5c4ffe5e2d000542/groups/6049ba10fd2be600015706e2

### [Friday the 13ths 6 kyu](https://www.codewars.com/kata/friday-the-13ths)

https://www.codewars.com/kata/reviews/540954dddd70268885000006/groups/6049bd50d224ba0001e438e8

## Object

### [Counting array elements 7 kyu](https://www.codewars.com/kata/counting-array-elements)

https://www.codewars.com/kata/reviews/556a4e15d44ca75d15000037/groups/603e1b0a77e5840001f905a9

### [Who is the killer-1 7 kyu](https://www.codewars.com/kata/who-is-the-killer-1)

https://www.codewars.com/kata/reviews/5f91ab3be4dc32000159c9bc/groups/6049c402c33f340001061619

## Regular expression

### [Simple validation of a username with regex 8 kyu](https://www.codewars.com/kata/simple-validation-of-a-username-with-regex)

---

### [Validate my password 6 kyu](https://www.codewars.com/kata/validate-my-password)

---
