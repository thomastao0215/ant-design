---
order: 1
title:
  zh-CN: 带搜索框
  en-US: Select with search field
---

## zh-CN

展开后可对选项进行搜索。

## en-US

Search the options while expanded.

````jsx
import { Select } from 'antd';
const Option = Select.Option;

function handleChange(value) {
  console.log(`selected ${value}`);
}

ReactDOM.render(
  <Select
    showSearch
    style={{ width: 200 }}
    placeholder="Select a person"
    optionFilterProp="children"
    onChange={handleChange}
  >
    <Option value="jack">Jack</Option>
    <Option value="lucy">Lucy</Option>
    <Option value="tom">Tom</Option>
  </Select>
, mountNode);
````
