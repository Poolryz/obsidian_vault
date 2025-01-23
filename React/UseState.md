```dataview 
TABLE without id
file.outlinks AS "OUTGOING",
file.inlinks AS "BACKLINKS"
WHERE file.name = this.file.name
```
#reference/info
# Links
[[02. React Hooks]]






# Description

useState - это хук React, который позволяет следить и изменять состояние некоторого значения. Значение может быть и объектом.

Вызывается он вначале функционального компонента или в кастомном хуке.

Принимает начальное значение и имеет под капотом функцию, которая изменяет значение.

Пример:
```jsx
import {useState} from 'react'

export default function myComponent(){
const [value, setValue]
}
```