# Calliope Mermaid Diagram Plugin

This plugin is for [Calliope](https://calliope.site) and is designed to provide functionality for mermaid diagrams inside of pages and posts.

### Installation

The plugin can be installed from NPM via:

        npm install calliope-mermaid

### Usage

Inside of your `_calliope/app/config/plugins/index.jsx` file, add the following:

```javascript
    // Import the module at the top
    import MermaidDiagram from "calliope-mermaid";
    // and then further down inside of the switch statement add the following
    // ...
    case "mermaid":
      console.log(MermaidDiagram);
      let { diagram } = props.attributes;
      if (diagram) {
        return <MermaidDiagram diagram={diagram} />;
      } else {
        return <></>;
      }
    // ...
```