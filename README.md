# react-data-grid

> The core of react-data-grid


## Install

Add the dependency declaration (`{..."react-data-grid": "git://github.com/cstjohn-bhg/react-data-grid-css-fix.git#no-style-testing"...}`) to your project's package.json pointing to the github URL and `npm install`.  The default CSS for the package has been provided at `./css/react-data-grid.css` to be exported and potentially modified for your consuming application.
```

## Usage

```sh
import ReactDataGrid from 'react-data-grid';

const columns = [{ key: 'id', name: 'ID' }, { key: 'title', name: 'Title' }];
const rows = [{ id: 1, title: 'Title 1' }, ...];
const rowGetter = rowNumber => rows[rowNumber];

const Grid = () => {
  return <ReactDataGrid
    columns={columns}
    rowGetter={rowGetter}
    rowsCount={rows.length}
    minHeight={500} />);
}
```

## Exports
Asside from the grid this package exports:

name                   | source                                  |
-----------------------|-----------------------------------------|
RowComparer            | [RowComparer](./src/RowComparer.js)     |
RowsContainer          | [RowsContainer](./src/RowsContainer.js) |
Row                    | [Row](./src/Row.js)                     |
Cell                   | [Cell](./src/Cell.js)                   |
HeaderCell             | [HeaderCell](./src/HeaderCell.js)       |
editors                | [Editors](./src/editors)                |
utils                  | [utils](./src/utils)                    |
shapes                 | [shapes](./src/PropTypeShapes)          |
_constants             | [_constants](./src/AppConstants.js)     |
_helpers               | [_helpers](./src/helpers)               |
