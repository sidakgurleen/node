# Node.js 21 ChangeLog

<!--lint disable maximum-line-length no-literal-urls prohibited-strings-->

<table>
<tr>
<th>Current</th>
</tr>
<tr>
<td>
<a href="#21.0.0">21.0.0</a><br/>
</td>
</tr>
</table>

* Other Versions
  * [19.x](CHANGELOG_V19.md)
  * [18.x](CHANGELOG_V18.md)
  * [17.x](CHANGELOG_V17.md)
  * [16.x](CHANGELOG_V16.md)
  * [15.x](CHANGELOG_V15.md)
  * [14.x](CHANGELOG_V14.md)
  * [13.x](CHANGELOG_V13.md)
  * [12.x](CHANGELOG_V12.md)
  * [11.x](CHANGELOG_V11.md)
  * [10.x](CHANGELOG_V10.md)
  * [9.x](CHANGELOG_V9.md)
  * [8.x](CHANGELOG_V8.md)
  * [7.x](CHANGELOG_V7.md)
  * [6.x](CHANGELOG_V6.md)
  * [5.x](CHANGELOG_V5.md)
  * [4.x](CHANGELOG_V4.md)
  * [0.12.x](CHANGELOG_V012.md)
  * [0.10.x](CHANGELOG_V010.md)
  * [io.js](CHANGELOG_IOJS.md)
  * [Archive](CHANGELOG_ARCHIVE.md)

<a id="21.0.0"></a>

## 2023-10-17, Version 21.0.0 (Current), @RafaelGSS and @targos

// Intro

Node.js 21 will replace Node.js 20 as our ‘Current’ release line when Node.js 20 enters long-term support (LTS) later this month.
As per the release schedule, Node.js 21 will be ‘Current' release for the next 6 months, until April 2024.

### Notable Changes

//

### Semver-Major Commits

* \[[`4e3983031a`](https://github.com/nodejs/node/commit/4e3983031a)] - **(SEMVER-MAJOR)** **build**: bump supported macOS and Xcode versions (Michaël Zasso) [#49164](https://github.com/nodejs/node/pull/49164)
* \[[`5a0777776d`](https://github.com/nodejs/node/commit/5a0777776d)] - **(SEMVER-MAJOR)** **crypto**: do not overwrite \_writableState.defaultEncoding (Tobias Nießen) [#49140](https://github.com/nodejs/node/pull/49140)
* \[[`e9ff81016d`](https://github.com/nodejs/node/commit/e9ff81016d)] - **(SEMVER-MAJOR)** **deps**: update llhttp to 9.1.2 (Paolo Insogna) [#48981](https://github.com/nodejs/node/pull/48981)
* \[[`1948dce707`](https://github.com/nodejs/node/commit/1948dce707)] - **(SEMVER-MAJOR)** **fs**: add globSync implementation (Moshe Atlow) [#47653](https://github.com/nodejs/node/pull/47653)
* \[[`c5b0b894ed`](https://github.com/nodejs/node/commit/c5b0b894ed)] - **(SEMVER-MAJOR)** **lib**: mark URL/URLSearchParams as uncloneable and untransferable (Chengzhong Wu) [#47497](https://github.com/nodejs/node/pull/47497)
* \[[`3205b1936a`](https://github.com/nodejs/node/commit/3205b1936a)] - **(SEMVER-MAJOR)** **lib**: remove aix directory case for package reader (Yagiz Nizipli) [#48605](https://github.com/nodejs/node/pull/48605)
* \[[`b40f0c3074`](https://github.com/nodejs/node/commit/b40f0c3074)] - **(SEMVER-MAJOR)** **lib**: add `navigator.hardwareConcurrency` (Yagiz Nizipli) [#47769](https://github.com/nodejs/node/pull/47769)
* \[[`4b08c4c047`](https://github.com/nodejs/node/commit/4b08c4c047)] - **(SEMVER-MAJOR)** **lib**: runtime deprecate punycode (Yagiz Nizipli) [#47202](https://github.com/nodejs/node/pull/47202)
* \[[`3ce51ae9c0`](https://github.com/nodejs/node/commit/3ce51ae9c0)] - **(SEMVER-MAJOR)** **module**: harmonize error code between ESM and CJS (Antoine du Hamel) [#48606](https://github.com/nodejs/node/pull/48606)
* \[[`7202859402`](https://github.com/nodejs/node/commit/7202859402)] - **(SEMVER-MAJOR)** **net**: do not treat `server.maxConnections=0` as `Infinity` (ignoramous) [#48276](https://github.com/nodejs/node/pull/48276)
* \[[`c15bafdaf4`](https://github.com/nodejs/node/commit/c15bafdaf4)] - **(SEMVER-MAJOR)** **net**: only defer \_final call when connecting (Jason Zhang) [#47385](https://github.com/nodejs/node/pull/47385)
* \[[`6ffacbf0f9`](https://github.com/nodejs/node/commit/6ffacbf0f9)] - **(SEMVER-MAJOR)** **node-api**: rename internal NAPI\_VERSION definition (Chengzhong Wu) [#48501](https://github.com/nodejs/node/pull/48501)
* \[[`64549731b6`](https://github.com/nodejs/node/commit/64549731b6)] - **(SEMVER-MAJOR)** **src**: throw DataCloneError on transfering untransferable objects (Chengzhong Wu) [#47604](https://github.com/nodejs/node/pull/47604)
* \[[`dac8de689b`](https://github.com/nodejs/node/commit/dac8de689b)] - **(SEMVER-MAJOR)** **stream**: use private properties for strategies (Yagiz Nizipli) [#47218](https://github.com/nodejs/node/pull/47218)
* \[[`1fa084ecdf`](https://github.com/nodejs/node/commit/1fa084ecdf)] - **(SEMVER-MAJOR)** **stream**: use private properties for encoding (Yagiz Nizipli) [#47218](https://github.com/nodejs/node/pull/47218)
* \[[`4e93247079`](https://github.com/nodejs/node/commit/4e93247079)] - **(SEMVER-MAJOR)** **stream**: use private properties for compression (Yagiz Nizipli) [#47218](https://github.com/nodejs/node/pull/47218)
* \[[`7cd4e70948`](https://github.com/nodejs/node/commit/7cd4e70948)] - **(SEMVER-MAJOR)** **test\_runner**: support passing globs (Moshe Atlow) [#47653](https://github.com/nodejs/node/pull/47653)
* \[[`ccca547e28`](https://github.com/nodejs/node/commit/ccca547e28)] - **(SEMVER-MAJOR)** **util**: runtime deprecate `promisify`-ing a function returning a `Promise` (Antoine du Hamel) [#49609](https://github.com/nodejs/node/pull/49609)

### Semver-Minor Commits

//

### Semver-Patch Commits

//
