# Hexo-Wordcount-Bengali

## Installation

```bash
yarn add hexo-wordcount-bengali
# or
npm install --save hexo-wordcount-bengali
```

## Usage

### WordCount


```js
wordcount(post.content)
```

### Min2Read

```js
min2read(post.content)
```

Set Reading Speed:

```js
min2read(post.content, {cn: 300, en: 160})
```

### TotalCount

```js
totalcount(site, '0,0.0a')
```

## Demo

### Swig

Post Count:

```swig
   <span class="post-count">{{ wordcount(post.content) }}</span>
```

Post Minutes to Read:

```swig
   <span class="post-count">{{ min2read(post.content) }}</span>
```

Total Count:

```swig
   <span class="post-count">{{ totalcount(site, '0,0.0a') }}</span>
```

Second param `format` optional.

### Ejs

Post Count:

```ejs
   <span class="post-count"><%= wordcount(post.content) %></span>
```

Post Minutes to Read:

```ejs
   <span class="post-count"><%= min2read(post.content) %></span>
```

Total Count:

```ejs
   <span class="post-count"><%= totalcount(site) %></span>
```

### Jade

Post Count:

```jade
   span.post-count= wordcount(post.content)
```

Post Minutes to Read:

```jade
    span.post-count= min2read(post.content)
```


Total Count:

```swig
   span.post-count= totalcount(site)
```

## LICENSE

MIT
