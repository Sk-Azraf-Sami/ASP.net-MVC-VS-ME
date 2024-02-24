# ASP.net-MVC VS Me

step 1: $`dotnet new mvc`<br>
step 2: $`dotnet add package Microsoft.EntityFrameworkCore.SqlServer` <br>
step 3: $`dotnet add package Microsoft.EntityFrameworkCore.Tools --version 2.1.1` <br>
step 4: $`dotnet restore`<br>
step 5: $`dotnet run` <br>
```cs
<ItemGroup>
      <DotNetCliToolReference
          Include="Microsoft.EntityFrameworkCore.Tools.DotNet"
          Version="2.1.1"/>
  </ItemGroup>

```
``

Source: [YouTube](https://youtu.be/yH0-LGKvVpc)

<b>install some packages:</b>

![img1](https://user-images.githubusercontent.com/106574604/231245634-05c5232b-49b4-4c90-b76f-80b1cec4f089.png)
![img2](https://user-images.githubusercontent.com/106574604/231246126-8f4c374d-3939-406f-9253-2c4d8904879c.png)

<b>install</b> package `"Microsoft.AspNetCore.Mvc.Razor.RuntimeCompilation->Version=6.0.16"` by `"nuget package install gui".` <br><br>
<b>You</b> will be notice a change in `"[project_name].cproj"` like this " `<PackageReference Include="Microsoft.AspNetCore.Mvc.Razor.RuntimeCompilation" Version="6.0.16" />"` <br> <br>
<b>You</b> will also add this line `builder.Services.AddRazorPages().AddRazorRuntimeCompilation();` in `Program.cs` file after this line `builder.Services.AddControllersWithViews();`<br>


