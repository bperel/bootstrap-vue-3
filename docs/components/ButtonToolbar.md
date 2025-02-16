# Button Toolbar

> Group a series of button-groups and/or input-groups together on a single line

**Example 1:** with button groups

<ClientOnly>
  <b-card>
    <div>
      <b-button-toolbar key-nav aria-label="Toolbar with button groups">
        <b-button-group class="mx-1">
          <b-button>&laquo;</b-button>
          <b-button>&lsaquo;</b-button>
        </b-button-group>
        <b-button-group class="mx-1">
          <b-button>Edit</b-button>
          <b-button>Undo</b-button>
          <b-button>Redo</b-button>
        </b-button-group>
        <b-button-group class="mx-1">
          <b-button>&rsaquo;</b-button>
          <b-button>&raquo;</b-button>
        </b-button-group>
      </b-button-toolbar>
    </div>
  </b-card>
</ClientOnly>

```html
<div>
  <b-button-toolbar key-nav aria-label="Toolbar with button groups">
    <b-button-group class="mx-1">
      <b-button>&laquo;</b-button>
      <b-button>&lsaquo;</b-button>
    </b-button-group>
    <b-button-group class="mx-1">
      <b-button>Edit</b-button>
      <b-button>Undo</b-button>
      <b-button>Redo</b-button>
    </b-button-group>
    <b-button-group class="mx-1">
      <b-button>&rsaquo;</b-button>
      <b-button>&raquo;</b-button>
    </b-button-group>
  </b-button-toolbar>
</div>
```

**Example 2:** with mixture of small button group and small input group

<ClientOnly>
  <b-card>
    <div>
      <b-button-toolbar aria-label="Toolbar with button groups and input groups">
        <b-button-group size="sm" class="mr-1">
          <b-button>Save</b-button>
          <b-button>Cancel</b-button>
        </b-button-group>
        <b-input-group size="sm" prepend="$" append=".00">
          <b-form-input value="100" class="text-right"></b-form-input>
        </b-input-group>
      </b-button-toolbar>
    </div>
  </b-card>
</ClientOnly>

```html
<div>
  <b-button-toolbar aria-label="Toolbar with button groups and input groups">
    <b-button-group size="sm" class="mr-1">
      <b-button>Save</b-button>
      <b-button>Cancel</b-button>
    </b-button-group>
    <b-input-group size="sm" prepend="$" append=".00">
      <b-form-input value="100" class="text-right"></b-form-input>
    </b-input-group>
  </b-button-toolbar>
</div>
```

**Example 3:** with button groups and dropdown menu

<ClientOnly>
  <b-card>
    <div>
      <b-button-toolbar aria-label="Toolbar with button groups and dropdown menu">
        <b-button-group class="mx-1">
          <b-button>New</b-button>
          <b-button>Edit</b-button>
          <b-button>Undo</b-button>
        </b-button-group>
        <b-dropdown class="mx-1" right text="menu">
          <b-dropdown-item>Item 1</b-dropdown-item>
          <b-dropdown-item>Item 2</b-dropdown-item>
          <b-dropdown-item>Item 3</b-dropdown-item>
        </b-dropdown>
        <b-button-group class="mx-1">
          <b-button>Save</b-button>
          <b-button>Cancel</b-button>
        </b-button-group>
      </b-button-toolbar>
    </div>
  </b-card>
</ClientOnly>

```html
<div>
  <b-button-toolbar aria-label="Toolbar with button groups and dropdown menu">
    <b-button-group class="mx-1">
      <b-button>New</b-button>
      <b-button>Edit</b-button>
      <b-button>Undo</b-button>
    </b-button-group>
    <b-dropdown class="mx-1" right text="menu">
      <b-dropdown-item>Item 1</b-dropdown-item>
      <b-dropdown-item>Item 2</b-dropdown-item>
      <b-dropdown-item>Item 3</b-dropdown-item>
    </b-dropdown>
    <b-button-group class="mx-1">
      <b-button>Save</b-button>
      <b-button>Cancel</b-button>
    </b-button-group>
  </b-button-toolbar>
</div>
```

## Usage

Feel free to mix input groups and dropdowns with button groups in your toolbars. Similar to the
example above, you'll likely need some utility classes though to space things properly.

## Sizing

Note, if you want smaller or larger buttons or controls, set the `size` prop directly on the
`<b-button-group>`, `<b-input-group>`, and `<b-dropdown>` components.

<ClientOnly>
  <b-card>
    <div>
      <b-button-toolbar aria-label="Toolbar with size sm">
        <b-button-group size="sm" class="mx-1">
          <b-button>New</b-button>
          <b-button>Edit</b-button>
          <b-button>Undo</b-button>
        </b-button-group>
      </b-button-toolbar>
    </div>
    <div class="mt-2">
      <b-button-toolbar aria-label="Toolbar with dropdown size sm">
          <b-dropdown size="sm" class="mx-1" right text="menu">
            <b-dropdown-item>Item 1</b-dropdown-item>
            <b-dropdown-item>Item 2</b-dropdown-item>
            <b-dropdown-item>Item 3</b-dropdown-item>
          </b-dropdown>
      </b-button-toolbar>
    </div>
    <div class="mt-2">
      <b-button-toolbar aria-label="Toolbar with size lg">
        <b-button-group size="lg" class="mx-1">
          <b-button>New</b-button>
          <b-button>Edit</b-button>
          <b-button>Undo</b-button>
        </b-button-group>
      </b-button-toolbar>
    </div>
    <div class="mt-2">
      <b-button-toolbar aria-label="Toolbar with dropdown size lg">
        <b-dropdown size="lg" class="mx-1" right text="menu">
          <b-dropdown-item>Item 1</b-dropdown-item>
          <b-dropdown-item>Item 2</b-dropdown-item>
          <b-dropdown-item>Item 3</b-dropdown-item>
        </b-dropdown>
      </b-button-toolbar>
    </div>
  </b-card>
</ClientOnly>

```html
<b-card>
  <div>
    <b-button-toolbar aria-label="Toolbar with size sm">
      <b-button-group size="sm" class="mx-1">
        <b-button>New</b-button>
        <b-button>Edit</b-button>
        <b-button>Undo</b-button>
      </b-button-group>
    </b-button-toolbar>
  </div>
  <div class="mt-2">
    <b-button-toolbar aria-label="Toolbar with dropdown size sm">
      <b-dropdown size="sm" class="mx-1" right text="menu">
        <b-dropdown-item>Item 1</b-dropdown-item>
        <b-dropdown-item>Item 2</b-dropdown-item>
        <b-dropdown-item>Item 3</b-dropdown-item>
      </b-dropdown>
    </b-button-toolbar>
  </div>
  <div class="mt-2">
    <b-button-toolbar aria-label="Toolbar with size lg">
      <b-button-group size="lg" class="mx-1">
        <b-button>New</b-button>
        <b-button>Edit</b-button>
        <b-button>Undo</b-button>
      </b-button-group>
    </b-button-toolbar>
  </div>
  <div class="mt-2">
    <b-button-toolbar aria-label="Toolbar with dropdown size lg">
      <b-dropdown size="lg" class="mx-1" right text="menu">
        <b-dropdown-item>Item 1</b-dropdown-item>
        <b-dropdown-item>Item 2</b-dropdown-item>
        <b-dropdown-item>Item 3</b-dropdown-item>
      </b-dropdown>
    </b-button-toolbar>
  </div>
</b-card>
```

## Justify

Make the toolbar span the maximum available width, by increasing spacing between the button groups,
input groups and dropdowns, by setting the prop `justify`.

<ClientOnly>
  <b-card>
    <div>
      <b-button-toolbar justify aria-label="Toolbar with justify">
        <b-button-group class="mx-1">
          <b-button>New</b-button>
          <b-button>Edit</b-button>
          <b-button>Undo</b-button>
        </b-button-group>
        <b-dropdown class="mx-1" right text="menu">
          <b-dropdown-item>Item 1</b-dropdown-item>
          <b-dropdown-item>Item 2</b-dropdown-item>
          <b-dropdown-item>Item 3</b-dropdown-item>
        </b-dropdown>
        <b-button-group class="mx-1">
          <b-button>Save</b-button>
          <b-button>Cancel</b-button>
        </b-button-group>
      </b-button-toolbar>
    </div>
  </b-card>
</ClientOnly>

```html
<div>
  <b-button-toolbar justify aria-label="Toolbar with justify">
    <b-button-group class="mx-1">
      <b-button>New</b-button>
      <b-button>Edit</b-button>
      <b-button>Undo</b-button>
    </b-button-group>
    <b-dropdown class="mx-1" right text="menu">
      <b-dropdown-item>Item 1</b-dropdown-item>
      <b-dropdown-item>Item 2</b-dropdown-item>
      <b-dropdown-item>Item 3</b-dropdown-item>
    </b-dropdown>
    <b-button-group class="mx-1">
      <b-button>Save</b-button>
      <b-button>Cancel</b-button>
    </b-button-group>
  </b-button-toolbar>
</div>
```

## Component reference

### `<b-button-toolbar>`

#### Properties

| Property    | Type      | Default | Description                                                                                                                    |
| ----------- | --------- | ------- | ------------------------------------------------------------------------------------------------------------------------------ |
| `aria-role` | `String`  | `group` | Sets the ARIA attribute `role` to a specific value                                                                             |
| `justify`   | `Boolean` | `false` | Make the toolbar span the maximum available width, by increasing spacing between the button groups, input groups and dropdowns |

#### Slots

| Name      | Scoped | Description                            |
| --------- | ------ | -------------------------------------- |
| `default` | No     | Content to place in the button toolbar |
