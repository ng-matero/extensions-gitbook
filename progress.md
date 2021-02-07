# Progress

### API reference for Material Extensions Progress

`import { MtxProgressModule } from '@ng-matero/extensions/progress';`

## Directives

### MtxProgress

Selector: `mtx-progress`

Exported as: `mtxProgress`

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
        <p>The progress types.</p>
        <p>Defaulted to <b>info</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>value: number</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>The progress value.</p>
        <p>Defaulted to <b>0</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>height: number</code>
        </p>
      </td>
      <td style="text-align:left">The progress height.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>color: string</code>
        </p>
      </td>
      <td style="text-align:left">The progress text color.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>foreground:string</code>
        </p>
      </td>
      <td style="text-align:left">The progress bar color.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>background:string</code>
        </p>
      </td>
      <td style="text-align:left">The progress track color.</td>
    </tr>
    <tr>
      <td style="text-align:left">@Input()
        <br /><code>striped: boolean</code>
      </td>
      <td style="text-align:left">Whether applies striped class.</td>
    </tr>
    <tr>
      <td style="text-align:left">@Input()
        <br /><code>animate: boolean</code>
      </td>
      <td style="text-align:left">Whether applies animated class.</td>
    </tr>
  </tbody>
</table>



