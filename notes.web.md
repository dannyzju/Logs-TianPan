### References

- [jawbone](https://jawbone.com/up)
- twitter
- weibo
- facebook
- renren
- evernote
- [windows build conference](http://www.buildwindows.com/)
  - div class = overlay
  - id = bg
- [squarespace](http://www.squarespace.com/?channel=display&subchannel=daringfireball&campaign=610)



------------------------------------------------------------------------------
## Ideas

- 做logo： j像一个跳起的小人
- masterpie.ce 师傅带徒弟
- Learning Tips
  - 学习的过程是螺旋向上的，不要妄想通过第一遍或者两三遍就能学得清晰透彻。当学习新知识的时候，先迅速过完第一遍，不求细节，只求轮廓，从第二遍更加仔细地看，如此反复，加之不断训练，以学习知识提升技能。


------------------------------------------------------------------------------
## short-cuts
ctrl + .  : 快速打开匹配选项卡
ctrl + shift + b  : build
F12/gd : go to definition

------------------------------------------------------------------------------
## definitions

routing engine: map url to controller

Controllers: define the response to the url call

        public ActionResult Search(string name)
        {
            var message = Server.HtmlEncode(name); // prevent malicious attack
            return Content(message);

        }

ActionResult 有很多类型可以返回

Action Selectors
[HttpPost] [HttpGet]

Action Filters
[Authorize]


*Exception*: throw new Exception("Something terrible happened");

  - Exception info will be displayed at runtime on the same machine
  - which is configured in Web.config
  - customErrors: on/off 是否显示 view/shared/error.cshtml

Razor Views

  - Template + data = generated output
  - razor 对embeded scripts 是有预防的: @Html.DisplayFor()，但是对Html.Raw(stringA) 可能会导致严重的后果


在cshtml 里面可以用@后面接C#代码，在C#代码里面可以@:加html代码

    @{
         @:htmlcode
    }

_layout


HTML Helpers(@Html.methods())

- Html is a property of the ViewPage base class
     - create inputs
     - create links
     - create forms


view
partial view


`@"blah blah"` 这里的@相当于System.String()

- [bool property without Required attribute is required](http://stackoverflow.com/questions/14992010/bool-property-without-required-attribute-is-required)
  - Reference Type and Value Type
    - A data type is a value type if it holds the data within its own memory allocation. A reference type contains a pointer to another memory location that holds the data.

## datetime vs datetimeoffset

http://stackoverflow.com/questions/4331189/datetime-vs-datetimeoffset

------------------------------------------------------------------------------
## Data

entity framework

DbContext

Dispose method 

ctrl + k, ctrl + c:  comment out

*Database Migration*

AutomaticMigrationsEnabled = true; // automatically update the database schema

package manager console: powershell

    PM> enable-migrations -ContextTypeName SportsContext-20130519135514
    PM> Update-Database

LINQ like SQL but `select` locates at the last

101 LINQ Samples

alt+Down : open drop down control

------------------------------------------------------------------------------
## Frontend: [Bootstrap Framework](http://twitter.github.io/bootstrap/)

[Chinese Reference](http://www.bootcss.com/)

Color Candidates

- navbar
  - black
  - white

·#ed1556  to dark `#cc0033·
·#0e7ac4·

    ::selection {
      background: #ed1556;
      color: white;
      text-shadow: none;
    }


------------------------------------------------------------------------------
## Square Brackets

Square brackets are also used to specify Attributes (C# and Visual Basic):

    using System.Diagnostics; 
    
    [Conditional("DEBUG")] 
    void TraceMethod() {}

------------------------------------------------------------------------------
## Lambda Expression






