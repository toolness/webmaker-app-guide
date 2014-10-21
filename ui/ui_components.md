# UI Components

## Alerts

#### Usage

```html
<div v-component="alert" type="error" message="someMessage"></div>
```

#### Attributes

* `type`: Can be `error` or `success`. Defaults to `error`.
* `message`: Message to display. Note this will be run through the `i18n` (i.e. translation) filter as a key. Defaults to `errorDefault`.

## Input error messages

This is not really a component so much as a set of styles. See `static/styles/forms.less`.

#### Usage

You should put a `div` with the class `form-error` directly following an input. For a checkbox input, it should directly follow the `label`.

```html
<input type="text">
<div class="form-error">This is my error!</div>

<div class="checkbox">
    <label>
        <input type="checkbox">
    </label>
    <div class="form-error">This is my error!</div>
</div>
```
