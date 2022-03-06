<p align="center">
  <h2 align="center">📄 Docs</h2>
</p>

<h6 align="center">
  <a href="https://github.com/Pocco81/koy-lang/blob/main/docs/specs.md">Specs</a>
  ·
  <a href="https://github.com/Pocco81/koy-lang/blob/main/docs/conventions.md">Conventions</a>
  ·
  <a href="https://github.com/Pocco81/koy-lang/tree/main/docs#-cheat-sheet">Cheat-sheets</a>
</h6>

<p align="center">
	Documentation for Koy, the human-friendly data serialization language
</p>

&nbsp;

### 🎏 Koy Lang

Koy is designed to be a minimal, simple and intuitive data serialization language; easy for you, your dog and your average 5 year-old. It has a small set of symbols, not too many rules and only one singular statement. Its lack of complexity makes it the perfect language for your project! easy to implement, debug and modularize.

Go ahead and check out the [Conventions](https://github.com/Pocco81/koy-lang/blob/main/docs/conventions.md) to learn about the generalities of the language! if you end up liking it, consider checking out the [Specs sheet](https://github.com/Pocco81/koy-lang/blob/main/docs/specs.md) and the [Style Guide](https://github.com/Pocco81/koy-lang/blob/main/docs/style-guide.md).

&nbsp;

### 📚 Cheat sheet

<details>
    <summary><i>Cheat sheet for symbols</i></summary>
&nbsp;

<table>
<tr>
<td> Symbols </td> <td> Function </td> <td> Example </td>

</tr>
<tr>
<td> <code>//</code> </td>
<td> Single-line comment </td>
<td>

```
// hello world!
```

</td>
</tr>

<tr>
<td> <code>/**/</code> </td>
<td> Multi-line comment </td>
<td>

```
/*
	This is a multi-line comment and
	you are watcing Disney channel!
*/
```

</td>
</tr>

</tr>
<tr>
<td> <code>${}</code> </td>
<td> Call a variable </td>
<td>

```
// simple usage
name: "Michael Theodor Mouse"
hello: "Good evening ${name}"

// with arrays (using the `.` notation)
user: {
	name: "Michael",
	surnames: "Theodor Mouse"
}
hi: "Good morning ${user.name}"
```

</td>
</tr>

</tr>
<tr>
<td> <code>""</code> </td>
<td> Define a normal string </td>
<td>

```
hello: "world"
```

</td>
</tr>

</tr>
<tr>
<td> <code>""" """</code> </td>
<td> Define a multi-line string </td>
<td>

```
hello: """My name is
	Michael Theodor Mouse, but
	you can call me Peter.
"""
```

</td>
</tr>

</tr>
<tr>
<td> <code>``</code> </td>
<td> Define a literal key </td>
<td>

```
`mainland!tv.קום`: "value"
```

</td>
</tr>

</tr>
<tr>
<td> <code>''</code> </td>
<td> Define a literal value </td>
<td>

```
weird_path: 'pc/\fds!fd/\&24324%!@'
```

</td>
</tr>

</tr>
<tr>
<td> <code>{}</code> </td>
<td> Define an array </td>
<td>

```
metadata: {
	OS: "Arch Linux",
	Kernel: "linux-hardened"
}
```

</td>
</tr>

</tr>
<tr>
<td> <code>[]</code> </td>
<td> Define an object </td>
<td>

```
user: [
	name: "Michael Theodor Mouse",
	age: 92
]
```

</td>
</tr>

</tr>
<tr>
<td> <code>import</code> </td>
<td> Import other <code>.koy</code> files </td>
<td>

```
// single import
import "./directory/settings.koy"

// multiple imports
import {
	"./directory/user0.koy",
	"./directory/user1.koy",
	"./directory/user2.koy"
}
```

</td>
</tr>

</tr>
<tr>
<td> <code><<</code> </td>
<td> Overwrite values </td>
<td>

```
// normal variables
hello: "world"
another_hello: ${hello} << "momma!"

// arrays
user: {
	name: "Michael Theodor Mouse",
	age: 93
}

laptop: {
	name: "Lenovo Thinkpad",
	owner: ${user} << {
		name: "Dominic Toretto"
	}
}
```

</td>
</tr>

</table>

<br />
</details>

<details>
    <summary><i>Cheat sheet for rules</i></summary>
&nbsp;

<br />
</details>

<details>
    <summary><i>Example <code>.koy</code> file using every feature</i></summary>
&nbsp;

<br />
</details>

&nbsp;
