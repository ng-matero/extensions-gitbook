# popover

### API reference for Material Extensions Popover

`import { MtxPopoverModule } from '@ng-matero/extensions/popover';`

## Directives

### MtxPopover

Selector: `[mtx-popover]`

Exported as: `mtxPopover`

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
        <p><code>xPosition: &apos;after&apos; | &apos;before&apos; | &apos;center&apos;</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Position of the popover in the X axis.</p>
        <p>Defaults to <code>&apos;after&apos;</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>yPosition: &apos;top&apos; | &apos;below&apos;</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Position of the popover in the Y axis.</p>
        <p>Defaults to <code>&apos;below&apos;</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>enterDelay: number</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Popover enter delay. Only support hover event.</p>
        <p>Defaults to <code>100</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>leaveDelay: number</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Popover enter delay. Only support hover event.</p>
        <p>Defaults to <code>100</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>xOffset: number</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Popover target offset X.</p>
        <p>Defaults to <code>0</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>yOffset: number</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Popover target offset Y.</p>
        <p>Defaults to <code>0</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>overlapTrigger: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether overlap trigger.</p>
        <p>Defaults to <code>false</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>closeOnPanelClick: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether close popover when click the panel.</p>
        <p>Defaults to <code>false</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>closeOnBackdropClick: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether close popover when click the backdrop.</p>
        <p>Defaults to <code>true</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>focusTrapEnabled: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether the popover should focus trap.</p>
        <p>Defaults to <code>true</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>focusTrapAutoCaptureEnabled: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether the popover should focus trap auto capture focus.</p>
        <p>Defaults to <code>true</code>
        </p>
      </td>
    </tr>
  </tbody>
</table>

### MtxPopoverTrigger

Selector: `[mtxPopoverTriggerFor]`

Exported as: `mtxPopoverTrigger`

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
        <p><code>mtxPopoverTriggerFor: MtxPopoverPanel</code>
        </p>
      </td>
      <td style="text-align:left">References the popover instance that the trigger is associated with.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>mtxPopoverTriggerOn: MtxPopoverTriggerEvent</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Event for triggering popover click, hover and none.</p>
        <p>Defaults to <code>&apos;hover&apos;</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>mtxPopoverTargetAt: MtxTarget</code>
        </p>
      </td>
      <td style="text-align:left">References the popover target instance that the popover positioning is
        associated with.</td>
    </tr>
  </tbody>
</table>

