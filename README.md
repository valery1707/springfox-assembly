SpringFox dependency prepared for use in JDK 9+.

Similar to [andreasfrosig](/andreasfrosig)'s solution in [springfox/springfox#2064](https://github.com/springfox/springfox/issues/2064#issuecomment-416462729).

Builded library hosted on [JitPack](https://jitpack.io/).

For use `springfox` as module in JKD 9+ project with modules you need only this steps:
1. Add the JitPack repository to your build file as described in [JitPack](https://jitpack.io/) documentation
2. Add dependency on [`com.github.valery1707:springfox-assembly`](https://jitpack.io/#valery1707/springfox-assembly) with required version
3. Remove direct dependency on `io.springfox:springfox-core`, `io.springfox:springfox-spi` or `io.springfox:springfox-schema`
4. Remove transient dependency on `io.springfox:springfox-core`, `io.springfox:springfox-spi` or `io.springfox:springfox-schema` from libraries such as `io.springfox:springfox-swagger2`, `io.springfox:springfox-swagger-ui` and etc.
5. Replace modules `springfox.core` and `springfox.spi` with `springfox.assembly`

If version is need for you does not exists already - you can request it by creating an Issue.
