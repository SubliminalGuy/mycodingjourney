#### What is the purpose of the **useMemo** hook in React?

The **useMemo** hook is used to memoize the result of a computationally expensive operation in a functional component. It helps optimize performance by caching the result of the operation and returning the cached result on subsequent renders if the dependencies have not changed.

#### Example:

``` js
import { useMemo } from 'react';

function TodoList({ todos, tab, theme }) {  
	const visibleTodos = useMemo(() => filterTodos(todos, tab), [todos, tab]);  
	// ...
}
```


#### Links:
[useMemo React Docs](https://react.dev/reference/react/useMemo)