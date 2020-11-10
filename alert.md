# Alert

### API reference for Material Extensions Alert

`import { MtxAlertModule } from '@ng-matero/extensions/alert';`

## Directives

### MtxAlert

Selector: `mtx-alert`

Exported as: `mtxAlert`

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
        <p><code>type: &apos;default&apos; | &apos;info&apos; | &apos;success&apos; | &apos;warning&apos; | &apos;danger&apos;</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>The alert types.</p>
        <p>Defaulted to <b>default</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>isOpen: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether alert visible.</p>
        <p>Defaulted to <b>true</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>dismissible: boolean</code>
        </p>
      </td>
      <td style="text-align:left">Whether displays an inline <code>close</code> button.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>color: string</code>
        </p>
      </td>
      <td style="text-align:left">The alert text color.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>elevation</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>The material elevation for alert.</p>
        <p>Defaulted to <b>0</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Output()</p>
        <p><code>closed: EventEmitter&lt;MtxAlertComponent&gt;</code>
        </p>
      </td>
      <td style="text-align:left">This event fires when alert closed.</td>
    </tr>
  </tbody>
</table>

\*\*\*\*

