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

UseContext - хук React который помогает переносить данные сразу в нужный компонент не прокидывая props через все дерево.

Создать useContext можно следующим образом.
1. Создаем отдельный файл в jsx.
2. Импортируем туда react и createContext.
3. Создаем контекст 
   ```jsx
   export const valueContext = createContext()
   ```
4. Пишем логику в отдельном компоненте и возвращаем из него обертку с Provider и в качестве атрибута передаем туда информацию.
   ```jsx
   export default function Context(props){
   //Логика
   const value
		return(
		<CarContext.Provider value={value}>
		{props.children}
		</CarContext.Provider>
		)
   }
   ```
5. А после используем эту обертку для передачи информации в нужный компонент, оборачивая его.