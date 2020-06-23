# treeForIcon
tree树控件修改图标css

## 不要加scoped
// 旋转
.el-tree-node__expand-icon.expanded {
  -webkit-transform: rotate(0deg) !important;
  transform: rotate(0deg) !important;
}
.el-icon-caret-right:before {
  // 加号图片
  content: "\e723" !important;
  font-size: 16px;
}
.expanded:before {
  // 减号图片
  content: "\e722" !important;
  font-size: 16px;
}
// 叶子类目不要图标
.is-leaf.el-tree-node__expand-icon.el-icon-caret-right:before {
  content:"" !important;
  font-size: 16px;
}