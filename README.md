# road-between-elements
Create path road between react elements


## How to use

```jsx
import { RoadGenerator, RoadCheckpoint } from "road-between-elements";

const MyComponent = () => {
  const [path, setPath] = useState(undefined);

  useEffect(() => {
    window.addEventListener('scroll', handleScroll);
  }, [])

  return <RoadGenerator onPathChange={path => path(path)}>
    <h1>Hello</h2>
    <RoadCheckpoint position="leftTop">
      <p>How are you</p>
    </RoadCheckpoint>
    <RoadCheckpoint position="rightBottom">
      <p>Test</p>
    </RoadCheckpoint>
  </RoadGenerator>
}
```
