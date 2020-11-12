# Color Picker

### API reference for Material Extensions ColorPicker

`import { MtxColorPickerModule } from '@ng-matero/extensions/color-picker';`

## Directives

### MtxColorPicker

Selector: `[mtx-color-picker]`

Exported as: `mtxColorPicker`

#### Properties

The color picker component is just like a `matInput`

<table>
  <thead>
    <tr>
      <th style="text-align:left">Name</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>value: string</code>
        </p>
      </td>
      <td style="text-align:left">Value of the color picker control.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>placeholder: string</code>
        </p>
      </td>
      <td style="text-align:left">Placeholder of the color picker control.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>disabled: boolean</code>
        </p>
      </td>
      <td style="text-align:left">Whether disabled the color picker control.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Output()</p>
        <p><code>colorChange: EventEmitter&lt;{ color: Color; $event: MouseEvent }&gt;</code>
        </p>
      </td>
      <td style="text-align:left">Event emitted when the color changed.</td>
    </tr>
  </tbody>
</table>

