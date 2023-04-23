# TailwindCSS

```
https://tailwindcss.com/docs/installation
```

## Background

```
class:
    bg-<colorName>-<colorIntensity>

//ex
<div class="bg-green-100">
    ...
</div>
```

## Typegraphy

### Color

```
class:
    text-<colorName>-<colorIntensity>

//ex
<div class="text-red-600">Hello World</div>
```
### Size

```
class:
    text-<type>

//ex
<div class="text-lg">Hello World</div>
<div class="text-white text-xl">Hello World</div>
```

### Style

```
font-italic
uppercase
lowercase
capitalize

//ex
<div class="text-white text-xl uppercase">Hello World</div>
```

### Weight
```
class :
    font-<typt>
    or
    forn-weight: <100 - 900>
//ex
<div class="text-white text-4xl font-weight:900">Hello World</div>
```

### Alignment

```
text-center
text-right
text-left

//ex
<div class="text-white text-4xl font-weight:900 text-right">Hello World</div>
```

### Opacity

```
class :
    text-opacity-<value 0 - 100>

//ex 
<div class="text-white text-4xl font-weight:900 text-right text-opacity-50">Hello World</div>
```

## Width, Height

```
w
h

//ex
<div class="bg-red-500 text-white w-40 h-40">1</div>
```

## Marging, Padding

```
One Direction
    m{t|r|b|l}-{size}

Horizon
    mx-{size}
    (x = left, righ)

Vertical
    my-{size}
    (y = top, bottom)

m-{size}
```

```
One Direction
    p{t|r|b|l}-{size}

Horizon
    px-{size}
    (x = left, righ)

Vertical
    py-{size}
    (y = top, bottom)

p-{size}
```

```
//ex
<div class="bg-blue-500 m-10 p-10">
    <div class="bg-red-500">Content</div>
</div>
```

## Border

```
//Border size
class :
    border-size
    border-{t|r|b|l}-size

//Border Color
class :
    border-<colorName>-<colorIntensity>

//ex
<button class="bg-green-500 text-white m-10 p-5 border border-red-500">Click</button>
<button class="bg-green-500 text-white m-10 p-5 border-red-500 border-t-8">Click</button>

---

//Border Radius
rounded, rounded-sm, rounded-lg, rounded-full, rounded-t-md,  etc

//ex
<button class="bg-green-500 text-white m-10 p-5 rounded">Click</button>
<button class="bg-green-500 text-white m-10 p-5 rounded-lg">Click</button>
<button class="bg-green-500 text-white m-10 p-5 rounded-full">Click</button>
<button class="bg-green-500 text-white m-10 p-5 rounded-r-lg">Click</button>


//Border Style
border-none, -solid, -dashed, -dotted, -double

//ex
<button class="bg-green-500 text-white m-10 p-5 border-8 border-red-500 border-dashed">Click</button>
```

## Box Shadow
```
//ex
<button class="bg-white m-10 p-5 shadow-2xl">Click</button>
<button class="bg-white m-10 p-5 shadow-inner">Click</button>
```

## Pseudo Selector
```
focus : bg-green-200
hover : bg-blue-200
```

```
<input type="text" placeholder="Enter some text" class="bg-gray-200 focus:bg-green-200" />
<button class="bg-yellow-500 hover:bg-red-500 hover:text-white">Save</button>
```

## Container, Breakpoint

```
class : 
    container
```

```
<div class="container bg-red-500 mx-auto">
    <h1 class="text-4xl sm:text-yellow-500 md:text-white">Heading</h1>
</div>
```

## Flexbox

### Flex Direction

```
row
row-reverse
column
column-reverse
```

```
<div class="bg-yellow-500 w-auto flex">
    <div class="w-10 h-10 bg-red-500">Box1</div>
    <div class="w-10 h-10 bg-red-500">Box2</div>
    <div class="w-10 h-10 bg-red-500">Box3</div>
</div>
<div class="bg-yellow-500 w-auto flex-column">
    <div class="w-10 h-10 bg-red-500">Box1</div>
    <div class="w-10 h-10 bg-red-500">Box2</div>
    <div class="w-10 h-10 bg-red-500">Box3</div>
</div>
```

### Wrap FlexItem

```
nowrap
wrap
wrap-reverse
```

```
<div class="bg-yellow-500 w-auto flex flex-wrap">
    <div class="w-80 h-10 bg-red-500">Box1</div>
    <div class="w-80 h-10 bg-red-500">Box2</div>
    <div class="w-80 h-10 bg-red-500">Box3</div>
</div>
```

### Grow, Shrink

```
flex-1
shrink
grow
```

```
<div class="bg-yellow-500 w-auto flex flex-wrap">
    <div class="w-80 h-10 bg-red-500">Box1</div>
    <div class="w-80 h-10 bg-blue-500 flex-grow">Box2</div>
    <div class="w-80 h-10 bg-green-500">Box3</div>
</div>
```

## Grid Layout

```
Row
Column
```

```
<div class="bg-yellow-500 w-auto grid grid-cols-3 grid-rows-3 gap-4">
    <div class="h-10 bg-red-500">Box1</div>
    <div class="h-10 bg-red-500">Box2</div>
    <div class="h-10 bg-red-500">Box3</div>
    <div class="h-10 bg-red-500">Box4</div>
    <div class="h-10 bg-red-500">Box5</div>
    <div class="h-10 bg-red-500">Box6</div>
    <div class="h-10 bg-red-500">Box7</div>
    <div class="h-10 bg-red-500">Box8</div>
    <div class="h-10 bg-red-500">Box9</div>
</div>
```

### Gap

```
gap-size
gra-x-size
gra-y-size
```

```
<div class="bg-yellow-500 w-auto grid grid-cols-3 grid-rows-3 gap-x-4 gap-y-8">
    <div class="h-10 bg-red-500">Box1</div>
    <div class="h-10 bg-red-500">Box2</div>
    <div class="h-10 bg-red-500">Box3</div>
    <div class="h-10 bg-red-500">Box4</div>
    <div class="h-10 bg-red-500">Box5</div>
    <div class="h-10 bg-red-500">Box6</div>
    <div class="h-10 bg-red-500">Box7</div>
    <div class="h-10 bg-red-500">Box8</div>
    <div class="h-10 bg-red-500">Box9</div>
</div>
```

## Justify-Items

```
start
center
end
stretch
```

```
<div class="bg-yellow-500 w-auto grid justify-items-center">
    <div class="h-10 bg-red-500">Box1</div>
    <div class="h-10 bg-red-500">Box2</div>
    <div class="h-10 bg-red-500">Box3</div>
</div>
```

### Justify-self

```
start
center
end
```

```
<div class="bg-yellow-500 w-auto grid">
    <div class="h-10 bg-red-500 justify-self-start">Box1</div>
    <div class="h-10 bg-red-500 justify-self-center">Box2</div>
    <div class="h-10 bg-red-500 justify-self-end">Box3</div>
</div>
```

## Layer, Apply

```
@tailwind base;         : Manage element
@tailwind components;   : Manage class
@tailwind utilities;    : Customize clase
```

### base

input.css
```
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base{
    a{
        @apply text-red-500
    }
}
```

index.html
```
<a href="#">Menu1</a>
<a href="#">Menu2</a>
<a href="#">Menu3</a>
```

### components

input.css
```
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer components{
    .menu-button{
        @apply text-white bg-red-500 p-3
    }
}
```

index.html
```
<a href="#" class="menu-button">Menu1</a>
<a href="#" class="menu-button">Menu2</a>
<a href="#" class="menu-button">Menu3</a>
```

### utilities

input.css
```
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer utilities{
    .text-red-500{
        color: blue;
        font-size: 1.5rem;
        font-weight: 500;
    }
}
```

index.html
```
<h1 class="text-red-500">Hello World</h1>
```

---