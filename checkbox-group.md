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
        <br /><code>change: EventEmitter&lt;{<br />model: MtxCheckboxGroupOption[];<br />index: number; }&gt;()</code>
      </td>
      <td style="text-align:left">Event emitted when the selection changed.</td>
    </tr>
  </tbody>
</table>

## Interfaces

### Checkbox Group Option

```typescript
export interface MtxCheckboxGroupOption {
  label: string;
  value: string;
  checked?: boolean;
  disabled?: boolean;
}
```

