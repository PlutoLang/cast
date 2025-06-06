# Pluto Cast

The original is always the best. Pluto Cast is that concept applied to runtime environments.

## Usage

First create a script to act as the cast target, for example:

```lua
function my_env_func()
    print("Hello from my_env_func")
end

require"cast".here("test")
```

Run the cast target script. Now, you can cast to it, leveraging the same environment as the target:

```lua
require"cast".to("test")

my_env_func() --> Hello from my_env_func
```
