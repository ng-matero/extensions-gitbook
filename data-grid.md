# Data Grid

### API reference for Material Extensions Data Grid

`import { MtxGridModule } from '@ng-matero/extensions/data-grid';`

## Directives

### MtxGrid

Selector: `mtx-grid`

Exported as: `mtxGrid`

#### **Properties**

Basic

| **Name** | Description |
| :--- | :--- |
| @Input\(\)`columns: MtxGridColumn[]` | The grid columns defination. |
| @Input\(\) `data: any[]` | The grid data source. |
| @Input\(\) `length: number` | The length of the total number of data. Defaulted to **0**. |
| @Input\(\) `loading: boolean` | Whether the table loading is ended. Defaulted to **false**. |
| @Input\(\)`trackBy: TrackByFunction<any>` | Tracking function that will be used to check the differences in data changes. |

Page

| **Name** | Description |
| :--- | :--- |
| @Input\(\)`pageOnFront: boolean` | Whether paging the data just on front end. Defaulted to **true**. |
| @Input\(\)`showPaginator: boolean` | Whether show the paginator. Defaulted to **true**. |
| @Input\(\)`pageDisabled: boolean` | Whether the paginator is disabled. Defaulted to **false**. |
| @Input\(\)`showFirstLastButtons: boolean` | Whether to show the first/last buttons UI to the user. Defaulted to **true**. |
| @Input\(\)`pageIndex: number` | The zero-based page index of the displayed list of items. Defaulted to **0**. |
| @Input\(\) `pageSize: number` | Number of items to display on a page. By default set to **10**. |
| @Input\(\)`pageSizeOptions: number[]` | The set of provided page size options to display to the user. By default set to **\[10, 50, 100\]** |
| @Input\(\)`hidePageSize: boolean` | Whether hide the pagesize. Defaulted to **false**. |
| @Output\(\)`page: EventEmitter<PageEvent>` | Event emitted when the paginator changes the page size or page index. |

Sort

| **Name** | Description |
| :--- | :--- |
| @Input\(\) `sortOnFront: boolean` | Whether sort data just on front end. Defaulted to **true**. |
| @Input\(\)`sortActive: string` | The id of the most recently sorted MatSortable. |
| @Input\(\)`sortDirection: SortDirection` | The sort direction of the currently active MatSortable. |
| @Input\(\)`sortDisableClear: boolean` | Whether to disable the user from clearing the sort by finishing the sort direction cycle. May be overriden by the column's disable clear definition. Defaulted to **false**. |
| @Input\(\)`sortDisabled: boolean` | Whether the grid sort is disabled. Defaulted to **false**. |
| @Input\(\)`sortStart: 'asc' | 'desc'` | The direction to set when an MatSortable is initially sorted. May be overriden by the column's sort definition. Defaulted to asc. |
| @Output\(\)`sortChange: EventEmitter<sort>` | Event emitted when the user changes either the active sort or sort direction. |

Expansion

| **Name** | Description |
| :--- | :--- |
| @Input\(\) `expandable: boolean` | Whether the row can be expanded. Defaulted to **false**. |
| @Input\(\) `expansionTemplate: TemplateRef<any>` | The template of expandable row. |
| @Output\(\) `expansionChange: EventEmitter<any>` | Event emitted when the user toggle the expandable row. |

Selection

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
        <p><code>multiSelectable: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether the user can selecte multiple row or cell.</p>
        <p>Defaulted to <b>true</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>rowSelectable: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether the row can be selectable.</p>
        <p>Defaulted to <b>false</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>rowSelected: any[]</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>The row selected items default.</p>
        <p>Defaulted to <code>[]</code>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>hideRowSelectionCheckbox: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether hide the row selection checkbox.</p>
        <p>Defaulted to <b>false</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>rowSelectionFormatter: MtxGridRowSelectionFormatter</code>
        </p>
      </td>
      <td style="text-align:left">The row selection formatter to set disabled and checkbox hiding.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Output()</p>
        <p><code>rowSelectionChange: EventEmitter&lt;any&gt;</code>
        </p>
      </td>
      <td style="text-align:left">Event emitted when the row be selected.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>cellSelectable: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether the cell can be selectable.</p>
        <p>Defaulted to <b>true</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Output()</p>
        <p><code>cellSelectionChange: EventEmitter&lt;any&gt;</code>
        </p>
      </td>
      <td style="text-align:left">Event emitted when the cell be selected.</td>
    </tr>
  </tbody>
</table>

Toolbar

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
        <p><code>showToolbar: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether show the grid toolbar.</p>
        <p>Defaulted to <b>false</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>toolbarTitle: string</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>The toolbar title.</p>
        <p>Defaulted to <b>&apos;&apos;</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>toolbarTemplate:</code>  <code>TemplateRef&lt;any&gt;</code>
        </p>
      </td>
      <td style="text-align:left">The toolbar template.</td>
    </tr>
  </tbody>
</table>

Column menu

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
      <td style="text-align:left">@Input() <code>columnHideable: boolean</code>
      </td>
      <td style="text-align:left">
        <p>Whether the column can be hiding.</p>
        <p>Defaulted to <b>true</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">@Input() <code>columnHideableChecked: &apos;show&apos; | &apos;hide&apos;</code>
      </td>
      <td style="text-align:left">
        <p>Hide or show when column hiding checkbox be checked.</p>
        <p>Defaulted to <b>&apos;show&apos;</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">@Input() <code>columnMovable: boolean</code>
      </td>
      <td style="text-align:left">
        <p>Whether the column can be moving.</p>
        <p>Defaulted to <b>true</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">@Output() <code>columnChange: EventEmitter&lt;string[]&gt;</code>
      </td>
      <td style="text-align:left">Event emitted when the column be hided or be resorted.</td>
    </tr>
    <tr>
      <td style="text-align:left">@Input() <code>showColumnMenuHeader: boolean</code>
      </td>
      <td style="text-align:left">
        <p>Whether show header of column menu.</p>
        <p>Defaulted to <b>false.</b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">@Input()<code>columnMenuHeaderText: string</code>
      </td>
      <td style="text-align:left">
        <p>The header text of column menu.</p>
        <p>Defaulted to <code>&apos;Columns Header&apos;</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>columnMenuHeaderTemplate: TemplateRef&lt;any&gt;</code>
        </p>
      </td>
      <td style="text-align:left">The header template of column menu.</td>
    </tr>
    <tr>
      <td style="text-align:left">@Input() <code>showColumnMenuFooter: boolean</code>
      </td>
      <td style="text-align:left">
        <p>Whether show footer of column menu.</p>
        <p>Defaulted to <code>false</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">@Input() <code>columnMenuFooterText: string</code>
      </td>
      <td style="text-align:left">
        <p>The header text of column menu.</p>
        <p>Defaulted to <code>&apos;Columns Footer&apos;</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">@Input()<code>columnMenuFooterTemplate: TemplateRef&lt;any&gt;</code>
      </td>
      <td style="text-align:left">The footer template of column menu.</td>
    </tr>
    <tr>
      <td style="text-align:left">@Input() <code>showColumnMenuButton: boolean</code>
      </td>
      <td style="text-align:left">
        <p>Whether show column menu button.</p>
        <p>Defaulted to <b>true</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">@Input() <code>columnMenuButtonText: string</code>
      </td>
      <td style="text-align:left">
        <p>The column menu button text.</p>
        <p>Defaulted to <b>&apos;&apos;</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">@Input() <code>columnMenuButtonType: &apos;raised&apos; | &apos;stroked&apos; | &apos;flat&apos; | &apos;icon&apos; | &apos;fab&apos; | &apos;mini-fab&apos; | &apos;&apos;</code>
      </td>
      <td style="text-align:left">
        <p>The column menu button type.</p>
        <p>Defaulted to &apos;<b>stroked&apos;</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">@Input() <code>columnMenuButtonColor: string</code>
      </td>
      <td style="text-align:left">
        <p>The column menu button color.</p>
        <p>Defaulted to <b>&apos;&apos;</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">@Input() <code>columnMenuButtonClass: string</code>
      </td>
      <td style="text-align:left">
        <p>The column menu button class.</p>
        <p>Defaulted to <b>&apos;&apos;</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">@Input() <code>columnMenuButtonIcon: string</code>
      </td>
      <td style="text-align:left">
        <p>The column menu button icon.</p>
        <p>Defaulted to <b>&apos;&apos;</b>.</p>
      </td>
    </tr>
  </tbody>
</table>

Template

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
        <p><code>noResultText: string</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>The no result text.</p>
        <p>Defaulted to <b>&apos;No records found&apos;</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>noResultTemplate: TemplateRef&lt;any&gt;</code>
        </p>
      </td>
      <td style="text-align:left">The no result template.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>headerTemplate: TemplateRef&lt;any&gt; | MtxGridCellTemplate</code>
        </p>
      </td>
      <td style="text-align:left">The grid header cell template.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>cellTemplate: TemplateRef&lt;any&gt; | MtxGridCellTemplate</code>
        </p>
      </td>
      <td style="text-align:left">The grid body cell template.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>showSummary: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether show summary.</p>
        <p>Defaulted to <b>false</b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>summaryTemplate: TemplateRef&lt;any&gt; | MtxGridCellTemplate</code>
        </p>
      </td>
      <td style="text-align:left">The summary template.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Output()</p>
        <p><code>rowClick: EventEmitter&lt;any&gt;;</code>
        </p>
      </td>
      <td style="text-align:left">Row click event.</td>
    </tr>
  </tbody>
</table>

## Interfaces

### Column

```typescript
export interface MtxGridColumn {
  field: string;
  header?: string;
  hide?: boolean;
  disabled?: boolean;
  pinned?: 'left' | 'right';
  left?: string;
  right?: string;
  width?: string;
  resizable?: boolean;
  sortable?: boolean | string;
  sortProp?: MtxGridColumnSortProp;
  type?: MtxGridColumnType;
  typeParameter?: MtxGridColumnTypeParameter;
  tag?: MtxGridColumnTag;
  buttons?: MtxGridColumnButton[];
  formatter?: (rowData: any, colDef?: any) => void;
  cellTemplate?: TemplateRef<any> | null;
  showExpand?: boolean;
  description?: string;
  i18n?: string;
  summary?: ((colData: any, colDef?: any) => void) | string;
}
```

### Column Type

```typescript
export declare type MtxGridColumnType =
  | 'tag'
  | 'button'
  | 'link'
  | 'image'
  | 'boolean'
  | 'number'
  | 'currency'
  | 'percent'
  | 'date';
```

### Column Type Parameter

```typescript
export interface MtxGridColumnTypeParameter {
  currencyCode?: string;
  display?: string | boolean;
  digitsInfo?: string;
  format?: string;
  locale?: string;
  timezone?: string;
}
```

### Column Sort Properties

```typescript
export interface MtxGridColumnSortProp {
  arrowPosition?: 'before' | 'after';
  disableClear?: boolean;
  id?: string;
  start?: 'asc' | 'desc';
}
```

### Column Button

```typescript
export interface MtxGridColumnButton {
  type?: 'basic' | 'icon';
  text?: string;
  icon?: string;
  color?: 'primary' | 'accent' | 'warn';
  click?: (record: any) => void;
  pop?: boolean;
  popTitle?: string;
  children?: MtxGridColumnButton[];
  iif?: (record: any) => boolean;
  tooltip?: string;
}
```

### Column Tag

```typescript
export interface MtxGridColumnTag {
  [key: number]: MtxGridColumnTagValue;
  [key: string]: MtxGridColumnTagValue;
}
export interface MtxGridColumnTagValue {
  text?: string;
  color?: string;
}
```

### Row Selection Formatter

```typescript
export interface MtxGridRowSelectionFormatter {
  disabled?: (rowData: any) => boolean;
  hideCheckbox?: (rowData: any) => boolean;
}
```

