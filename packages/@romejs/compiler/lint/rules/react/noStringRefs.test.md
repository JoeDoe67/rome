# `noStringRefs.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test packages/@romejs/compiler/lint/rules/react/noStringRefs.test.ts --update-snapshots` to update.

## `react no string refs`

### `0`

```

 unknown:4:25 lint/react/noStringRefs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Using this.refs is a deprecated pattern.

    2 │      class Hello extends React.Component {
    3 │       componentDidMount() {
  > 4 │        const component = this.refs.hello;
      │                          ^^^^^^^^^
    5 │       }

  ℹ See https://reactjs.org/docs/refs-and-the-dom.html#legacy-api-string-refs for more information.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `0: formatted`

```
class Hello extends React.Component {
	componentDidMount() {
		const component = this.refs.hello;
	}

	render() {
		return <div>Hello {this.props.name}</div>;
	}
}

```

### `1`

```

 unknown:4:19 lint/react/noStringRefs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Using string literals in ref attributes is a deprecated pattern.

    2 │      class Hello extends React.Component {
    3 │       render() {
  > 4 │        return <div ref="hello">Hello {this.props.name}</div>;
      │                    ^^^^^^^^^^^
    5 │       }
    6 │      }

  ℹ See https://reactjs.org/docs/refs-and-the-dom.html#legacy-api-string-refs for more information.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `1: formatted`

```
class Hello extends React.Component {
	render() {
		return <div ref='hello'>Hello {this.props.name}</div>;
	}
}

```

### `2`

```

 unknown:4:19 lint/react/noStringRefs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Using string literals in ref attributes is a deprecated pattern.

    2 │      class Hello extends React.Component {
    3 │       render() {
  > 4 │        return <div ref={`hello`}>Hello {this.props.name}</div>;
      │                    ^^^^^^^^^^^^^
    5 │       }
    6 │      }

  ℹ See https://reactjs.org/docs/refs-and-the-dom.html#legacy-api-string-refs for more information.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `2: formatted`

```
class Hello extends React.Component {
	render() {
		return <div ref={`hello`}>Hello {this.props.name}</div>;
	}
}

```

### `3`

```

 unknown:4:19 lint/react/noStringRefs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Using string literals in ref attributes is a deprecated pattern.

    2 │      class Hello extends React.Component {
    3 │       render() {
  > 4 │        return <div ref={'hello'}>Hello {this.props.name}</div>;
      │                    ^^^^^^^^^^^^^
    5 │       }
    6 │      }

  ℹ See https://reactjs.org/docs/refs-and-the-dom.html#legacy-api-string-refs for more information.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `3: formatted`

```
class Hello extends React.Component {
	render() {
		return <div ref={"hello"}>Hello {this.props.name}</div>;
	}
}

```

### `4`

```

 unknown:4:21 lint/react/noStringRefs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Using string literals in ref attributes is a deprecated pattern.

    2 │      class Hello extends React.Component {
    3 │        render() {
  > 4 │          return <div ref={`hello${index}`}>Hello {this.props.name}</div>;
      │                      ^^^^^^^^^^^^^^^^^^^^^
    5 │        }
    6 │      }

  ℹ See https://reactjs.org/docs/refs-and-the-dom.html#legacy-api-string-refs for more information.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `4: formatted`

```
class Hello extends React.Component {
	render() {
		return <div ref={`hello${index}`}>Hello {this.props.name}</div>;
	}
}

```

### `5`

```

 unknown:4:25 lint/react/noStringRefs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Using this.refs is a deprecated pattern.

    2 │      class Hello extends React.Component {
    3 │       componentDidMount() {
  > 4 │        const component = this.refs.hello;
      │                          ^^^^^^^^^
    5 │       }

  ℹ See https://reactjs.org/docs/refs-and-the-dom.html#legacy-api-string-refs for more information.

 unknown:8:19 lint/react/noStringRefs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Using string literals in ref attributes is a deprecated pattern.

     7 │       render() {
   > 8 │        return <div ref="hello">Hello {this.props.name}</div>;
       │                    ^^^^^^^^^^^
     9 │       }
    10 │      }

  ℹ See https://reactjs.org/docs/refs-and-the-dom.html#legacy-api-string-refs for more information.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 2 problems

```

### `5: formatted`

```
class Hello extends React.Component {
	componentDidMount() {
		const component = this.refs.hello;
	}

	render() {
		return <div ref='hello'>Hello {this.props.name}</div>;
	}
}

```

### `6`

```
✔ No known problems!

```

### `6: formatted`

```
class Hello extends React.Component {
	componentDidMount() {
		const component = this.hello;
	}

	render() {
		return <div ref={(c) => this.hello = c}>Hello {this.props.name}</div>;
	}
}

```
