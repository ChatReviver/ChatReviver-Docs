<style>
    /* Shows the pointer when you hover over the @ */
    .tag { cursor: pointer; }
    
    /* Copy to clipboard tooltip container */
    .tag {
      position: relative;
      display: inline-block;
      /*border-bottom: 1px dotted black;*/
    }

    /* Tooltip text */
    .tag .tag_text {
      visibility: hidden;
      background-color: black;
      color: #fff;
      text-align: center;
      padding: 3px 0;
      border-radius: 6px;   /* This rounds the corners for some reason */

      width: 130px;
      bottom: 100%;
      left: 50%;
      margin-left: -65px; /* Use half of the width (130/2 = 65), to center */

      position: absolute;
      z-index: 1;
    }
    
    /* On hover */
    .tag:hover .tag_text {
      visibility: visible;
    }

</style>

# Custom Prefixes
The bot has support for setting your own custom prefixes.

!!! tip
    If you ever forget your custom prefixes, you can always use the default `r?`
    or mention the bot instead of a prefix 
    <a class="tag" onclick="navigator.clipboard.writeText('@ChatReviver#0198 ')">
    `@ChatReviver`<span class="tag_text">Copy to clipboard</span></a> 
    followed by a command.
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