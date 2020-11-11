# loader

### API reference for Material Extensions Loader

`import { MtxLoaderModule } from '@ng-matero/extensions/loader';`

## Directives

#### **Properties**

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
        <p><code>type: &apos;spinner&apos; | &apos;progressbar&apos;</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>The loader type.</p>
        <p>Defaulted to <b>&apos;spinner&apos;</b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>loading: boolean</code>
        </p>
      </td>
      <td style="text-align:left">The loading status.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>color: ThemePalette</code>
        </p>
      </td>
      <td style="text-align:left">Theme color palette for the component.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>mode&#xFF1A;ProgressSpinnerMode | ProgressBarMode</code>
        </p>
      </td>
      <td style="text-align:left">Mode of the progress circle.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>value: number</code>
        </p>
      </td>
      <td style="text-align:left">Value of the progress circle or progress bar.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>strokeWidth: number</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Stroke width of the progress spinner.</p>
        <p>Defaulted to <b>4</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>diameter: number</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>The diameter of the progress spinner (will set width and height of svg).</p>
        <p>Defaulted to <b>48.</b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>bufferValue: number</code>
        </p>
      </td>
      <td style="text-align:left">Buffer value of the progress bar. Defaulted to <b>0</b>.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>hasBackdrop: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether show loader backdrop.</p>
        <p>Defaulted to <b>true.</b>
        </p>
      </td>
    </tr>
  </tbody>
</table>



