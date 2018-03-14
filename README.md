# postcss-flex-short

PostCSS plugin for write short flex parameters

## Install

```
npm install postcss-flex-short --save
```

## Example

### Input

```css
div { 
  flex-container: width-1200px direction-row align-center justify-stretch; 
} 

p { 
  flex-column: width-400px flex-1 align-flex-start; 
}
```

### Output

```css
div { 
  display: flex; 
  width: 100%; 
  max-width: 1200px; 
  flex-direction: row; 
  align-items: center; 
  justify-content: stretch; 
} 

p { 
  width: 100%; 
  max-width: 400px; 
  align-self: flex-start; 
}
```