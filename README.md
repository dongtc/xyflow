![readme-header-dark](https://user-images.githubusercontent.com/3797215/156258604-73ab192f-e13c-4caf-aabb-e46f5d6b26af.svg#gh-dark-mode-only)
![readme-header](https://user-images.githubusercontent.com/3797215/156259138-fb9f59f8-52f2-474a-b78c-6570867e4ead.svg#gh-light-mode-only)

<div align="center">

  ![GitHub License MIT](https://img.shields.io/github/license/wbkd/react-flow?color=%23FF0072)
  ![npm downloads](https://img.shields.io/npm/dt/react-flow-renderer?color=%23FF0072&label=downloads)
  ![GitHub Repo stars](https://img.shields.io/github/stars/wbkd/react-flow?color=%23FF0072)
  ![GitHub release (latest by date)](https://img.shields.io/github/v/release/wbkd/react-flow?color=%23FF0072)

### Wire Your Ideas With React Flow!  
A highly customizable React component for building interactive graphs and node-based editors.

[🚀 Getting Started](https://reactflow.dev/docs/getting-started/installation) | [📖 Documentation](https://reactflow.dev/docs/api/react-flow-props) | [📺 Examples](https://reactflow.dev/docs/examples/overview) | [☎️ Discord](https://discord.gg/Bqt6xrs)
  
</div>

----

## Key Features

- **Easy to use:** Seamless zooming and panning, single- and multi selection of graph elements and keyboard shortcuts are supported out of the box
- **Customizable:** Different [node](https://reactflow.dev/docs/api/nodes/node-types) and [edge types](https://reactflow.dev/docs/api/edges/edge-types) and support for custom nodes with multiple handles and custom edges
- **Fast rendering:** Only nodes that have changed are re-rendered and only those in the viewport are displayed
- **Hooks and Utils:** [Hooks](https://reactflow.dev/docs/api/hooks/use-react-flow) for handling nodes, edges and the viewport and graph [helper functions](https://reactflow.dev/docs/api/graph-util-functions)
- **Plugin Components:** [Background](https://reactflow.dev/docs/api/plugin-components/background), [MiniMap](https://reactflow.dev/docs/api/plugin-components/minimap) and [Controls](https://reactflow.dev/docs/api/plugin-components/controls)
- **Reliable**: Written in [Typescript](https://www.typescriptlang.org/) and tested with [cypress](https://www.cypress.io/)

## Installation

The easiest way to install the latest version of React Flow is to install it via npm:

```bash
npm install react-flow-renderer
```

## Usage Example

```jsx
import ReactFlow, { MiniMap, Controls } from 'react-flow-renderer';

function Flow({ nodes, edges, onNodesChange, onEdgesChange, onConnect }) {
  return (
    <ReactFlow
      nodes={nodes}
      edges={edges}
      onNodesChange={onNodesChange}
      onEdgesChange={onEdgesChange}
      onConnect={onConnect}
    >
      <MiniMap />
      <Controls />
    </ReactFlow>
  );
}
```

## Local Development

@todo

## Maintainers

React Flow is developed and maintained by [webkid](https://webkid.io), a data visualization studio from Berlin. If you need help or want to talk to us about a collaboration, feel free to contact us:

* Moritz Klack • [Twitter](https://twitter.com/moklick) • [Github](https://github.com/moklick)
* Christopher Möller • [Twitter](https://twitter.com/chrtze) • [Github](https://github.com/chrtze)

You can also use our [contact form](https://webkid.io/contact/) or join the [React Flow Discord Server](https://discord.gg/Bqt6xrs).

## Community Packages

* [useUndoable](https://github.com/Infinium8/useUndoable) - Hook for undo/redo functionality with an explicit React Flow example
* [react-flow-smart-edge](https://github.com/tisoap/react-flow-smart-edge) - Custom edge that doesn't intersect with nodes
* [Feliz.ReactFlow](https://github.com/tforkmann/Feliz.ReactFlow) - Feliz React Bindings for React Flow

## Credits

React Flow was initially developed for [datablocks](https://datablocks.pro), a graph-based editor for transforming, analyzing and visualizing data in your browser. Under the hood, React Flow depends on these great libraries:

* [d3-zoom](https://github.com/d3/d3-zoom) - used for zoom, pan and drag interactions with the graph canvas
* [react-draggable](https://github.com/react-grid-layout/react-draggable) - used for making the nodes draggable
* [zustand](https://github.com/pmndrs/zustand) - internal state management

## License

React Flow is [MIT licensed](https://github.com/wbkd/react-flow/blob/main/LICENSE).
