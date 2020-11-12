# Data Grid

### API reference for Material Extensions Data Grid

`import { MtxGridModule } from '@ng-matero/extensions/data-grid';`

## Directives

### MtxGrid

Selector: `mtx-grid`

Exported as: `mtxGrid`

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
        <p><code>columns: MtxGridColumn[]</code>
        </p>
      </td>
      <td style="text-align:left">The grid columns defination.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>data: any[]</code>
        </p>
      </td>
      <td style="text-align:left">The grid data source.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>length: number</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>The length of the total number of data.</p>
        <p>Defaulted to <b>0</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>loading: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether the table loading is ended.</p>
        <p>Defaulted to <b>false</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>trackBy: TrackByFunction&lt;any&gt;</code>
        </p>
      </td>
      <td style="text-align:left">Tracking function that will be used to check the differences in data changes.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>pageOnFront: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether paging the data just on front end.</p>
        <p>Defaulted to <b>true</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>showPaginator: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether show the paginator.</p>
        <p>Defaulted to <b>true</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>pageDisabled: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether the paginator is disabled.</p>
        <p>Defaulted to <b>false</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">@Input()<code>showFirstLastButtons: boolean</code>
      </td>
      <td style="text-align:left">
        <p>Whether to show the first/last buttons UI to the user.</p>
        <p>Defaulted to <b>true</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>pageIndex: number</code>
        </p>
      </td>
      <td style="text-align:left">The zero-based page index of the displayed list of items.
        <br />Defaulted to <b>0</b>.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>pageSize: number</code>
        </p>
      </td>
      <td style="text-align:left">Number of items to display on a page.
        <br />By default set to <b>10</b>.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>pageSizeOptions: number[]</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>The set of provided page size options to display to the user.</p>
        <p>By default set to <b>[10, 50, 100]</b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>hidePageSize: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether hide the pagesize.</p>
        <p>Defaulted to <b>false</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Output()</p>
        <p><code>page: EventEmitter&lt;PageEvent&gt;</code>
        </p>
      </td>
      <td style="text-align:left">Event emitted when the paginator changes the page size or page index.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>sortOnFront: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether sort data just on front end.</p>
        <p>Defaulted to <b>true</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>sortActive: string</code>
        </p>
      </td>
      <td style="text-align:left">The id of the most recently sorted MatSortable.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>sortDirection: SortDirection</code>
        </p>
      </td>
      <td style="text-align:left">The sort direction of the currently active MatSortable.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>sortDisableClear: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether to disable the user from clearing the sort by finishing the sort
          direction cycle. May be overriden by the column&apos;s disable clear definition.</p>
        <p>Defaulted to <b>false</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>sortDisabled: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether the grid sort is disabled.</p>
        <p>Defaulted to <b>false</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>sortStart: &apos;asc&apos; | &apos;desc&apos;</code>
        </p>
      </td>
      <td style="text-align:left">The direction to set when an MatSortable is initially sorted. May be overriden
        by the column&apos;s sort definition. Defaulted to asc.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Output()</p>
        <p><code>sortChange: EventEmitter&lt;sort&gt;</code>
        </p>
      </td>
      <td style="text-align:left">Event emitted when the user changes either the active sort or sort direction.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>expandable: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether the row can be expanded.</p>
        <p>Defaulted to <b>false</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>expansionTemplate: TemplateRef&lt;any&gt;</code>
        </p>
      </td>
      <td style="text-align:left">The template of expandable row.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Output()</p>
        <p><code>expansionChange: EventEmitter&lt;any&gt;</code>
        </p>
      </td>
      <td style="text-align:left">Event emitted when the user toggle the expandable row.</td>
    </tr>
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
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>columnHideable: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether the column can be hiding.</p>
        <p>Defaulted to <b>true</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>columnHidingChecked: &apos;show&apos; | &apos;hide&apos;</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Hide or show when column hiding checkbox be checked.</p>
        <p>Defaulted to <b>&apos;show&apos;</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>columnMovable: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether the column can be moving.</p>
        <p>Defaulted to <b>true</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Output()</p>
        <p><code>columnChange: EventEmitter&lt;string[]&gt;</code>
        </p>
      </td>
      <td style="text-align:left">Event emitted when the column be hided or be resorted.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>showColumnMenuHeader: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether show header of column menu.</p>
        <p>Defaulted to <b>false.</b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>columnMenuHeaderText: string</code>
        </p>
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
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>showColumnMenuFooter: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether show footer of column menu.</p>
        <p>Defaulted to <code>false</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>columnMenuFooterText: string</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>The header text of column menu.</p>
        <p>Defaulted to <code>&apos;Columns Footer&apos;</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>columnMenuFooterTemplate: TemplateRef&lt;any&gt;</code>
        </p>
      </td>
      <td style="text-align:left">The footer template of column menu.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>showColumnMenuButton: boolean</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Whether show column menu button.</p>
        <p>Defaulted to <b>true</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>columnMenuButtonText: string</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>The column menu button text.</p>
        <p>Defaulted to <b>&apos;&apos;</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>columnMenuButtonType: &apos;raised&apos; | &apos;stroked&apos; | &apos;flat&apos; | &apos;icon&apos; | &apos;fab&apos; | &apos;mini-fab&apos; | &apos;&apos;</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>The column menu button type.</p>
        <p>Defaulted to &apos;<b>stroked&apos;</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>columnMenuButtonColor: string</code>
        </p>
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
      <td style="text-align:left">
        <p>@Input()</p>
        <p><code>columnMenuButtonIcon: string</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>The column menu button icon.</p>
        <p>Defaulted to <b>&apos;&apos;</b>.</p>
      </td>
    </tr>
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

