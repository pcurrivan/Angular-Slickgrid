# Angular-Slickgrid
One of the best javascript datagrid [SlickGrid](https://github.com/mleibman/SlickGrid) which was originally developed by @mleibman is now available to Angular. I have used a few datagrids and slickgrid beats most of them in terms of functionalities and performance (it can easily deal with even a million row).

### SlickGrid Source
We will be using [6pac SlickGrid fork](https://github.com/6pac/SlickGrid/) (the most active fork since the original @mleibman fork was closed some time ago by his author personal reasons).

### Goal
The goal is of course to be able to run SlickGrid within Angular 4+ but also to incorporate as much as possible the entire list of functionalities (and more) that SlickGrid offers (you can see a vast list of samples on the [6pac SlickGrid examples](https://github.com/6pac/SlickGrid/wiki/Examples) website).

### Demo page
[https://ghiscoding.github.io/Angular-Slickgrid](https://ghiscoding.github.io/Angular-Slickgrid)

### NPM Package
[Angular-Slickgrid on NPM](https://www.npmjs.com/package/angular-slickgrid)

<a name="wiki"></a>

## Wiki / Documentation
The Wiki is where all the documentation and instructions will go, so please consult the [Angular-Validation - Wiki](https://github.com/ghiscoding/angular-slickgrid/wiki) before opening any issues. The [Wiki - HOWTO](https://github.com/ghiscoding/angular-slickgrid/wiki/HOWTO---Step-by-Step) is a great place to start with.


<a name="main-features"></a>

## Main features
You can see some screenshots below and the instructions down below.

This is a work in progress, but so far here are some of the features that `angular-slickgrid` brings (on top of Slickgrid itself):
- Easier use of SlickGrid within `Angular` as it is just a component (simply pass a column definitions and a dataset and you're good to go)
- Bootstrap Theme with SASS variables for extra customization (if you create a theme, then please make a PR)
- Auto-resize (boolean flag), will resize the datagrid viewport with available space even on browser resize (basically takes available space of it's container)
- Integrated Plugins.
    - Column Picker (show/hide any column by doing `right+click` in the header, click [here to see print screen](/screenshots/columnPicker.png)).
    - ... more to come
- Server side (backend) Services (filtering, sorting, pagination)
    - [GraphQL](https://github.com/ghiscoding/Angular-Slikgrid/wiki/GraphQL)
    - [OData](https://github.com/ghiscoding/Angular-Slickgrid/wiki/OData)
- Some Features of SlickGrid itself which are working out of the gate
  - Sort/Multi-Sort (client/server side)
  - Header Row with Filters (currently support `Input` and `Select` dropdown, multi-select is planned)
  - Formatters (a few default ones were added, and you can easily create custom ones too)
  - Optimized DataView which brings a lot of functionalities (sort, grouping, and more)
    - even server side data is saved into the SlickGrid DataView
- ... more to come

<a name="missing-features"></a>

## Missing features (planned items, not necessarily in order of execution)
The following are SlickGrid features which are not yet included in this library but will be in the eventual future.
- Inline Editors
- Filters to support multi-select dropdown and eventually custom filters
- Plugins (Header Menu, Grid Menu, Column Header Buttons)
- Row selection, will probably provide a `onRowsChanged()` in the `gridOptions` object
- Cell click, will probably provide a `onCellClicked()` in the `gridOptions` object

### License
[MIT License](https://github.com/ghiscoding/Angular-Slickgrid/blob/master/LICENSE)

## Use it, like it?
You like and use this great library `Angular-Slickgrid`? You can always upvote :star: and/or contribute :)

## Screenshots

Screenshots from the demo app with the `Bootstrap` theme (that is the only available theme, but there is a lot of SASS variables to make it look like Material, or other theme if you wish to. If you create a new theme, please submit a PR).

### Slickgrid example with Formatters (last column shown is a custom Formatter)

![Default Slickgrid Example](/screenshots/formatters.png)

### Filter and Sort (clientside with DataView)

![Slickgrid Server Side](/screenshots/filter_and_sort.png)

### Slickgrid Example with Server Side (Filter/Sort/Pagination)

![Slickgrid Server Side](/screenshots/pagination.png)