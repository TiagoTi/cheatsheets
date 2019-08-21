---
title: Pitaco Front
category: React
layout: 2017/sheet
ads: true
tags: [Featured]
updated: 2019-07-30
weight: -10
keywords:
  - React.Component
  - render()
  - componentDidMount()
  - props/state
  - dangerouslySetInnerHTML
intro: |
  [React](https://reactjs.org/) is a JavaScript library for building user interfaces. This guide targets React v15 to v16.
---

{%raw%}

## React

### Tabela Sever Side Data

{: .-prime}

```jsx
<ReactTable
  ...
  data={this.state.data} // should default to []
  pages={this.state.pages} // should default to -1 (which means we don't know how many pages we have)
  loading={this.state.loading}
  manual // informs React Table that you'll be handling sorting and pagination server-side
  onFetchData={(state, instance) => {
    // show the loading overlay
    this.setState({loading: true})
    // fetch your data
    Axios.post('mysite.com/data', {
      page: state.page,
      pageSize: state.pageSize,
      sorted: state.sorted,
      filtered: state.filtered
    })
      .then((res) => {
        // Update react-table
        this.setState({
          data: res.data.rows,
          pages: res.data.pages,
          loading: false
        })
      })
  }}
/>
```

React Table
-----------
* [React Table With Server Data](https://www.npmjs.com/package/react-table#server-side-data)

Also see
--------

* [React website](https://reactjs.org) _(reactjs.org)_
* [React cheatsheet](https://reactcheatsheet.com/) _(reactcheatsheet.com)_
* [Awesome React](https://github.com/enaqx/awesome-react) _(github.com)_
* [React v0.14 cheatsheet](react@0.14) _Legacy version_

{%endraw%}