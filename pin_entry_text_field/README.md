# 👏 PinEntryTextField

A fully customizable Pin Entry TextField.

The source code is **100% Dart**, and everything resides in the [/lib](https://github.com/prestigegodson/pin-entry-text-field/tree/master/pin_entry_text_field/lib) folder.


### Show some :heart: and star the repo to support the project

### GIF
<img src="https://user-images.githubusercontent.com/15202781/45807904-650ca080-bcbc-11e8-87de-2b9c76b3a05f.jpg" height="400" width="400"/>
<img src="https://user-images.githubusercontent.com/15202781/45807939-79e93400-bcbc-11e8-8bef-808c5459d6dd.jpg" height="400" width="400"/>

## 💻 Installation
In the `dependencies:` section of your `pubspec.yaml`, add the following line:

```
pin_entry_text_field: <latest_version>
```
`Current Version : ^0.1.3`

## ❔ Usage

### Import this class
```
import 'package:pin_entry_text_field/pin_entry_text_field.dart';
```

### use the widget anywhere you need to retrieve PIN or OTP, the only required attribute is the onSubmit callback
```
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: PinEntryTextField(
            onSubmit: (String pin){
              showDialog(
                context: context,
                builder: (context){
                  return AlertDialog(
                    title: Text("Pin"),
                    content: Text('Pin entered is $pin'),
                  );
                }
              ); //end showDialog()

            }, // end onSubmit
          ),
    );
  }
```

## 🎨 Customization and Attributes

All customizable attributes for PinEntryTextField
<table>
    <th>Attribute Name</th>
    <th>Example Value</th>
    <th>Description</th>
    <tr>
        <td>fields</td>
        <td>4</td>
        <td>Specifies the number of TextField to generate, the default is 4</td>
    </tr>
    <tr>
        <td>onSubmit</td>
        <td>(String returnedPin){}</td>
        <td>The onSubmit callback returns the entered pin, where the user types in the last pin or hit done key</td>
    </tr>
    <tr>
        <td>fieldWidth</td>
        <td>40.0</td>
        <td>The size of each TextField, the default is 40.0</td>
    </tr>
    <tr>
        <td>fontSize</td>
        <td>20.0</td>
        <td>TextField font size, the default is 20.0</td>
    </tr>
    <tr>
        <td>isTextObscure</td>
        <td>false</td>
        <td>Determines if the text in the PinEntryTextField is bbscured or not. The default is false </td>
    </tr>
    <tr>
        <td>showFieldAsBox</td>
        <td>false</td>
        <td>Determines if the TextField should have an OutlineInputBorder at the 4 edges, or just a bottom underline</td>
    </tr>
    
</table>


# 👍 How to Contribute
1. Fork it
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create new Pull Request

# 📃 License

    Copyright (c) 2018 Godson Ositadinma
    
    Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
    
    The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
    
    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Getting Started

For help getting started with Flutter, view our online [documentation](https://flutter.io/).

For help on editing package code, view the [documentation](https://flutter.io/developing-packages/).