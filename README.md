# seed-rand
Generate random number with seed.

# Usage

## Install
```
npm install seed-rand
```

## Init
```
var SeedRand = require('seed-rand');
```

## Generate numbers
// Create instance with a seed.
var sr = new SeedRand(88);

// Generator a random number.
sr.rand(); // 0.21312132134
sr.rand(); // 0.12312414124
sr.rand(); // 0.34757745432
```

## Generate numbers in specified scope
```
var sr = new SeedRand(8, 100);
sr.rand(); // 82
sr.rand(); // 45
sr.rand(); // 67
```

## Generate a batch of numbers
```
sr.batch(5); // [24, 65, 11, 73, 11], reduplicate numbers are allowed
sr.batch(5, true); // [24, 65, 11, 73, 13], reduplicate numbers are NOT allowed
```
