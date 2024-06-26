<br/>

<div align="center">
   <a href="https://www.npmjs.com/package/@candlefinance%2Fcache">
  <img alt="npm downloads" src="https://img.shields.io/npm/dw/@candlefinance/cache?logo=npm&label=NPM%20downloads&cacheSeconds=3600"/>
   </a>
  <a alt="discord users online" href="https://discord.gg/qnAgjxhg6n" 
  target="_blank"
  rel="noopener noreferrer">
    <img alt="discord users online" src="https://img.shields.io/discord/986610142768406548?label=Discord&logo=discord&logoColor=white&cacheSeconds=3600"/>
    </a>
</div>
<br/>

<h1 align="center">
   Cache store for React Native 
</h1>


<div align="center">
<img width="690" alt="Screenshot 2024-05-01 at 12 27 12 AM" src="https://github.com/candlefinance/cache/assets/12258850/4632a696-3b0c-44f9-98f5-d2393137de9f">
</div>
<br/>

Using DiskCache for Android and non-deadlocking parallel [PINCache](https://github.com/pinterest/PINCache) for iOS, this library provides a simple interface to store data in a key-value format for offline mode.

## Installation

- Requires `iOS 12+` for iOS

1. 
```sh
yarn add @candlefinance/cache
```

```sh
npm i @candlefinance/cache
```

2. Add to your target in your Podfile if you get an error
```ruby
pod 'PINCache', :modular_headers => true
```

## Usage

Currently max size on iOS is 50MB and 200MB on Android. 

```js
await write('key', 'value');

const result = await read('key'); // can be undefined if key doesn't exist

await remove('key');

await clear();
```

## Contributing

Join our [Discord](https://discord.gg/qnAgjxhg6n) and ask questions in the **#oss** channel.

## License

MIT
