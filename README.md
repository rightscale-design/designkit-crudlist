# designkit-crudlist
1.0.0

A Sass module for * used in RightScale apps.

## Install
```
npm i --save designkit-crudlist
```

## CSS

```css
.crud-list-wrap {
  position: relative;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
}

.crud-list-view {
  width: 32%;
  padding-right: 30px;
}

.crud-list-view .list-scroll {
  z-index: 1;
  max-height: 70vh;
  padding: 0;
  margin: 0;
  overflow: auto;
  background-color: #fff;
  border: 1px solid #d1d6dc;
  border-bottom: 1px solid #c8ced5;
  border-radius: 3px;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.05);
}

.crud-list-view .list-item {
  position: relative;
  overflow: hidden;
  list-style: none;
  border-bottom: 1px solid #e2e5e9;
}

.crud-list-view .list-item:first-of-type.selected:after {
  border-radius: 2px 0 0 0;
}

.crud-list-view .list-item:last-of-type {
  border-bottom: none;
}

.crud-list-view .list-item.selected {
  background-color: #fff;
}

.crud-list-view .list-item.selected:after {
  position: absolute;
  top: -1px;
  bottom: -1px;
  left: 0;
  width: 2px;
  content: "";
  background: #0a83f6;
}

.crud-list-view .list-item:not(.selected) .ani-list {
  transition: height .4s ease-in-out;
}

.crud-list-view .item-anchor {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  padding: 1.4rem 2rem;
  -ms-flex-wrap: nowrap;
      flex-wrap: nowrap;
}

.crud-list-view .item-anchor:before {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  z-index: 1;
  width: 60px;
  content: "";
  background-image: linear-gradient(90deg, rgba(255, 255, 255, 0), white 30%);
  opacity: 0;
  transition: all 0.3s cubic-bezier(0.3, 0, 0, 1.3);
  -webkit-transform: translateX(100%) scale(0.7);
          transform: translateX(100%) scale(0.7);
}

.crud-list-view .item-anchor:after {
  position: absolute;
  top: 0;
  right: 1.5rem;
  bottom: 0;
  z-index: 2;
  width: 13px;
  content: "";
  opacity: 0;
  transition: all 0.3s cubic-bezier(0.3, 0, 0, 1.3);
  -webkit-transform: translateX(100%) scale(0.7);
          transform: translateX(100%) scale(0.7);
}

.crud-list-view .list-item:not(.selected) .item-anchor:hover:before,
.crud-list-view .list-item:not(.selected) .item-anchor:hover:after {
  opacity: 1;
  -webkit-transform: translateX(0%) scale(1);
          transform: translateX(0%) scale(1);
}

.crud-list-view .list-body {
  -webkit-box-flex: 1;
      -ms-flex: 1 50%;
          flex: 1 50%;
}

.crud-list-view .list-body .list-title {
  display: block;
  font-weight: bold;
  text-overflow: ellipsis;
}

.crud-list-view .list-body .list-subtitle {
  display: block;
  font-size: 1.2rem;
  color: #76899a;
  -webkit-box-flex: 1;
      -ms-flex: 1 50%;
          flex: 1 50%;
}

.crud-detail-view {
  width: 68%;
  height: 100%;
  background-color: #fff;
  border: 1px solid #d1d6dc;
  border-bottom: 1px solid #c8ced5;
  border-radius: 3px;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.05);
  transition: all 0.3s cubic-bezier(0.3, 0, 0, 1.3);
}

.crud-detail-view .detail-padding {
  padding: 2rem;
}

```

## Author

Jason Melgoza

## License

MIT
