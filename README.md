# 居中

## 1.table实现水平垂直居中

```
.dt {
    display: table;
    width: 400px;
    height: 400px;
    border: 1px #000 solid;
}

.dtc {
    display: table-cell;
    vertical-align: middle;
}

.box {
    width: 100px;
    height: 100px;
    background-color: red;
    margin: 0 auto;
}
```

## 2.absolute实现水平垂直居中

```
.container {
    position: relative;

    width: 400px;
    height: 400px;

    border: 1px #000 solid;
}

.box {
    position: absolute;
    /*top: calc(50% - 50px);
    left: calc(50% - 50px);*/
    top: 50%;
    left: 50%;

    width: 100px;
    height: 100px;
    margin-top: -50px;
    margin-left: -50px;

    background-color: red;
}
```

## 3.margin实现水平垂直居中

```
.container {
    position: relative;

    width: 400px;
    height: 400px;

    border: 1px #000 solid;
}

.box {
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;

    width: 100px;
    height: 100px;
    margin: auto; /*需要用绝对定位撑开*/

    background-color: red;
}
```

## 4.translate实现水平垂直居中

```
.container {
    position: relative;

    width: 400px;
    height: 400px;

    border: 1px #000 solid;
}

.box {
    position: absolute;
    top: 50%;
    left: 50%;

    width: 100px;
    height: 100px;

    background-color: red;

    transform: translate(-50%, -50%);
}
```

## 5.flex实现水平垂直居中

```
.container {
    display: flex;
    align-items: center;
    justify-content: center;

    width: 400px;
    height: 400px;

    border: 1px #000 solid;
}

.box {
    width: 100px;
    height: 100px;

    background-color: red;
}
```