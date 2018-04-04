In visual studio

1. Create Service Fabric Application
2. Select dotnet core stateless service
3. Empty Web template

What are the needed steps to make this project packable for both Unix and Windows clusters?

I know that i found some quickstart repository with an example. But hey, that was a bunch of sh, cmd files and what not. Its not the experience I am looking for. I dont want to develop on linux.

I just want a nice visual studio experience where I can press F5 to test on my windows dev box and when done commit the code and have VSTS build both a linux and windows package.


Here is what I tried.

Updating web1.csproj to use two RuntimeIdentifiers for Unix and windows. This broke the visual studio build/f5 experience.

I could get vsts to build this semi buy adding msbuild arguments to select the right runtime. 

I am up for trying more things, but would be super cool to have some advices on best path/most promishing path that will lead to success.


# If you know how
Feel free to make a pull request to this with an updated solution  and updating readme with build steps to make it work.