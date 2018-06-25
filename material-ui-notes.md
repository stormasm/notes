This concept is shown in the material-ui AppFrame.

```
export default compose(
  withStyles(styles, {
    name: 'AppFrame',
  }),
  connect(state => ({
    uiTheme: state.theme,
  })),
)(AppFrame);
```

This concept is shown in florida-mui-menu AppChapter.

```
const part = compose(
    withStyles(styles, {
      name: 'MenuAppBar',
    }),
    connect(mapStateToProps))(MenuAppBar);

export default withRoot(part);
```

and other ways to do it...
```
export default connect(mapStateToProps)(MenuAppBar);
export default withRoot(withStyles(styles)(MenuAppBar));
```
