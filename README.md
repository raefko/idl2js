# *WIP* idl2js

### Examples

`idl`
```
[Exposed=(Window,Worker)]
interface Blob {
  [Throws]
  constructor(optional sequence<BlobPart> blobParts,
              optional BlobPropertyBag options = {});

  [GetterThrows]
  readonly attribute unsigned long long size;

  readonly attribute DOMString type;

  [Throws]
  Blob slice(optional [Clamp] long long start,
             optional [Clamp] long long end,
             optional DOMString contentType);

  [NewObject, Throws] ReadableStream stream();
  [NewObject] Promise<USVString> text();
  [NewObject] Promise<ArrayBuffer> arrayBuffer();
};
```
`js`
```
let v_cb16fe6dbaf1498f99875a42200b4516 = new Blob()
let v_5f826e18849a4e569445dbd281b4a353 = v_cb16fe6dbaf1498f99875a42200b4516.size
let v_92e1d27127ff461eb333111cba8911ab = v_cb16fe6dbaf1498f99875a42200b4516.type
let v_a657497572654ca983cb044065628cde = v_cb16fe6dbaf1498f99875a42200b4516.slice()
let v_2711e5fdc3574e02bb24278b86db8bcf = v_cb16fe6dbaf1498f99875a42200b4516.stream()
let v_c5e916aed01b4b109a0a0bcb78de0de7 = v_cb16fe6dbaf1498f99875a42200b4516.text()
let v_23894af618ed479d89fa3b765ef3cfda = v_cb16fe6dbaf1498f99875a42200b4516.arrayBuffer()

```


### Links

* [searchfox - webidl](https://searchfox.org/mozilla-central/source/dom/webidl)
