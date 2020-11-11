# Checkbox Group

### API reference for Material Extensions CheckboxGroup

`import { MtxCheckboxGroupModule } from '@ng-matero/extensions/checkbox-group';`

## Directives

### MtxCheckboxGroup

Selector: `mtx-checkbox-group`

Exported as: `mtxCheckboxGroup`

#### **Properties**

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>Name</b>
      </th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>items: any[]</code>
        </p>
      </td>
      <td style="text-align:left">Items array</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>bindLabel: string</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Object property to use for label.</p>
        <p>Defaulted to <b>&apos;label&apos;</b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>bindValue: string</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Object property to use for selected model. By default binds to whole object.</p>
        <p>Defaulted to <b>&apos;value&apos;</b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>compareWith: (a: any, b: any) =&gt; boolean</code>
        </p>
      </td>
      <td style="text-align:left">A function to compare the option values with the selected values. The
        first argument is a value from an option. The second is a value from the
        selection(model). A boolean should be returned.</td>
    </tr>
    <tr>
      <td style="text-align:left">@Input()
        <br /><code>showSelectAll: boolean</code>
      </td>
      <td style="text-align:left">
        <p>Whether show select all.</p>
        <p>Defaulted to <b>true</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">@Input()
        <br /><code>selectAllLabel: string</code>
      </td>
      <td style="text-align:left">
        <p>The lable of select all.</p>
        <p>Defaulted to <b>Select All</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">@Output()
        <br /><code>change: EventEmitter&lt;{ <br />model: MtxCheckboxGroupOption[]; <br />index: number; }&gt;()</code>
      </td>
      <td style="text-align:left">Event emitted when the selection changed.</td>
    </tr>
  </tbody>
</table>

## Interfaces

### Checkbox Group Option

```typescript
export interface MtxCheckboxGroupOption {
  ariaDescribedby?: string;
  ariaLabel?: string;
  ariaLabelledby?: string;
  label?: any;
  value?: any;
  color?: string;
  checked?: boolean;
  disabled?: boolean;
  disableRipple?: boolean;
  indeterminate?: boolean;
  labelPosition?: 'before' | 'after';
  id?: string;
  name?: string | null;
  required?: boolean;
  [k: string]: any;
}
```

