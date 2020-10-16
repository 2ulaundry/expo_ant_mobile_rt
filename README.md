# POC Expo with ant mobile RN (IOS|Android|Web)

DEMO: [https://dexter-lab-02.web.app/](https://dexter-lab-02.web.app/)

![Demo A](repo_images/demo_a.png "Demo A")

## Steps to review this repo

- [ ] run `. ./scripts/web.server.sh`

## Steps to install in fresh expo project

- [ ] run `. ./scripts/bootstrap_v2.sh`  or `. ./scripts/bootstrap.sh`

- [ ] update the file: `babel.config.js`

```javascript
module.exports = function(api) {
  api.cache(true);
  return {
    presets: ['babel-preset-expo','module:metro-react-native-babel-preset'],
    plugins: [
      ['import', {libraryName: '@ant-design/react-native'}],
    ],
  };
};
```

## References

[2020 React Native usa componentes Ant Design Mobile RN](https://blog.csdn.net/lxyoucan/article/details/108334465)

[autolinking](https://github.com/react-native-community/cli/blob/master/docs/autolinking.md)
