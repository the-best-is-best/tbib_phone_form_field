## About
  this library with phone form field but add some future like add icon dropdown after country code.
## Demo

Demo available at https://cedvdb.github.io/phone_form_field/


## Usage
 * Alert this library widget with phone form field see this library in https://pub.dev/packages/phone_form_field

 ## Example

 ```dart
     PhoneFormField(
           // new attribute
           showDropDownIcon: true, // Default : false
           dropDownIcon: Icons.arrow_drop_down, // Default
           dropDownIconSize: 16, // Default

          key: inputKey,
          // controller: controller,
          shouldFormat: shouldFormat,
          autofocus: true,
          initialValue: PhoneNumber.fromRaw('+336787678'),
          autofillHints: const [AutofillHints.telephoneNumber],
          countrySelectorNavigator: selectorNavigator,
          defaultCountry: IsoCode.US,
          decoration: InputDecoration(
            label: withLabel ? const Text('Phone') : null,
            border: outlineBorder
                ? const OutlineInputBorder()
                : const UnderlineInputBorder(),
            hintText: withLabel ? '' : 'Phone',
          ),
          enabled: true,
          showFlagInInput: true,
          validator: _getValidator(),
          autovalidateMode: AutovalidateMode.onUserInteraction,
          cursorColor: Theme.of(context).colorScheme.primary,
          // ignore: avoid_print
          onSaved: (p) => print('saved $p'),
          // ignore: avoid_print
          onChanged: (p) => print('changed $p'),
        ),
```

* please us it in pubspec to use translation phone form field

``` dart
 flutter_localizations: #Add this line
    sdk: flutter
```