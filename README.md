&nbsp;

<div align="center">
<img src="docs/images/demo.gif" width="550" />
</div>

&nbsp;

<div align="center">

**✨ Write stunning mobile+desktop apps in Python.**

***In closed beta, join source-access waitlist: https://docs.google.com/forms/d/1rck6wvNUfwbMTl8aM9jSb7G5Poh7nQBWnObDX0-yq-Q

<img src="docs/images/capybara.jpeg">
<hr>



</div>

## ⚡️ 1. Works on your any screen with your exisitng tools

Capy is *not* a new UI framework for writing apps; it is a Python library for a unified API. Whether you are working with SwiftUI for iOS or XML for Android, start replacing small cmoponents using Capy today!

## ⚡️ 2. 30+ stunning, accessible components

Capy offers 30+ commonly used components that are stunning and accessible. Build a complex apps with fewest lines of code.

## 🥳 3. Built for developers

Capy is completely hackable and open-source. If you can write it with SwiftUI, UIKit, Jetpack Compose, Fluter, or XML, you can build it in Capy in Python!

## ⚡️ 4. Insanely performant

Capy is powered by platform-native code, and allows you to write super performant apps. For example apps written with Capy is runs significantly faster than React-Native. 

## 🫧 Example

Let's creat an image caption generator that accept an image upload:

This is all done in one Python file in a Flask project and stop writing templates.

```python
import capy as ca

class MyView(ca.View):
    @ca.StateObject
    class State:
        number = 1

        def decrement(self):
            self.number -= 1
        def increment(self):
             self.number += 1

    def body(self):
        return ca.VStack(
            ca.Heading(f'Count: {self.state.number} '),
            ca.HStack(
                ca.Button("lower", bg='red', on_click=self.State.decrement),
                ca.Button("higher", on_click=self.State.increment)
            )
        )

view = MyView()

```

## License

Capy is licensed under the [Apache License 2.0](LICENSE).