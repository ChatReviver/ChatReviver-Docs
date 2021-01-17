<style>
.container { cursor: pointer; }

.full { display: none; }
.container:hover .short { display: none; }
.container:hover .full { display: inline; }
</style>

# Custom Prefixes
The bot has support for setting your own custom prefixes.

!!! tip
    If you ever forget your custom prefixes, you can always use the default `r?`
    or a mention instead of a prefix
    <span class="container">
       <code><a class="short">@ChatReviver</a>
       <a class="full" onclick="navigator.clipboard.writeText(this.textContent)">@ChatReviver#0198</a>
    </span></code>followed by your command.
---

## Creating a custom prefix
To create a custom prefix, invoke the command `r?prefix add` followed by the custom prefix you want to add.

!!! example
    `r?prefix add !`  
    Prefixes can contain letters, numbers, spaces, symbols, etc. but make sure yours is easily typable on all platforms.  

!!! warning
    Custom prefixes must be 16 characters or shorter and cannot contain backticks **`` ` ``**
    or any other characters disallowed by Discord.  
    The bot will strip any characters automatically to meet these requirements.

## Viewing prefixes
Invoke the command `r?prefixes` to see all default and custom prefixes on your server.

!!! example "Example output"
    ![](/images/logo.png)
    
## Deleting custom prefixes
The bot has an interactive menu to delete custom prefixes.  
Invoke the command `r?prefixes remove` to access this.

!!! info
    The default prefixes cannot be removed