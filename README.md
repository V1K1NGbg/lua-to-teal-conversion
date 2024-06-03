# lua-to-teal-conversion

Test the migration of luarocks from lua to teal

## Operation steps

### Set up

luarocks install cyan

cyan init

### Build

cyan build

### Configure path

export LUA_PATH=./build/?.lua

### Run

lua build/luatoteal/a.lua

OR

tl run src/luatoteal/a.tl

### Upload

luarocks pack luatoteal-1.0-1.rockspec

luarocks upload luatoteal-1.0-1.rockspec --api-key=<key>

https://luarocks.org/modules/v1k1ngbg/luatoteal