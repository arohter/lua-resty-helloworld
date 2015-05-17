## lua-resty-helloworld

```
server {
  listen 80;
  #lua_code_cache off;

  location /helloworld {
    default_type text/html;
    content_by_lua_file "<%= @lua_path %>/lua-resty-helloworld/lib/resty/helloworld.lua";
  }

}
```
