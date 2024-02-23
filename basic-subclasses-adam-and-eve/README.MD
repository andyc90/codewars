**Task:** Basic subclasses - Adam and Eve

**Category:** Object-oriented Programming

**Description:** The code provided defines JavaScript classes for creating instances of `Man`, `Woman`, and a static `God` class. The `Man` and `Woman` classes extend a common base class `Human` and initialize the gender property accordingly.

**Original Code:**

```js
class God {
  /**
   * @returns Human[]
   */
  static create() {
    // code
  }
}
// code
```

**Step 1:**

Include a common base class `Human` that both `Man` and `Woman` extend. Assume `Human` has a constructor that sets the `name` property.

```js
class Human {
  constructor(name) {
    this.name = name;
  }
}

class Man extends Human {
  constructor(name) {
    super(name);
    this.gender = "male";
  }
}

class Woman extends Human {
  constructor(name) {
    super(name);
    this.gender = "female";
  }
}
```

**Step 2:**

Use the `God` class to create instances of `Man` and `Woman` (Adam and Eve).

```js
class Human {
  constructor(name) {
    this.name = name;
  }
}

class Man extends Human {
  constructor(name) {
    super(name);
    this.gender = "male";
  }
}

class Woman extends Human {
  constructor(name) {
    super(name);
    this.gender = "female";
  }
}

class God {
  static create() {
    const adam = new Man("Adam");
    const eve = new Woman("Eve");
    return [adam, eve];
  }
}
```

**Conclusion**

**Final working code:**

```js
class Human {
  constructor(name) {
    this.name = name;
  }
}

class Man extends Human {
  constructor(name) {
    super(name);
    this.gender = "male";
  }
}

class Woman extends Human {
  constructor(name) {
    super(name);
    this.gender = "female";
  }
}

class God {
  static create() {
    const adam = new Man("Adam");
    const eve = new Woman("Eve");
    return [adam, eve];
  }
}
```

The `God` class can now be used to create instances of `Man` and `Woman`, representing Adam and Eve.
