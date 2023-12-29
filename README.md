<B> If you have any issues following these steps, create an issue under the Issues tab on this repository. </b>
# Godot installation
At BluePlay, we make games in Godot (pronounced Go-dot, contrary to popular belief) using the .NET platform, a platform of programming languages made by Microsoft.
When you first join BluePlay, follow these steps.
- Get godot from [here](https://godotengine.org/download/windows/)


Make sure you get the .NET version.


![.NET version](READMEmedia/godot_dotnet.png)
- Extract the files, then move to the next step.
# .NET installation
.NET SDK version 6.X is needed to develop Godot games. 
- Install from https://dotnet.microsoft.com/en-us/download/dotnet/6.0

Make sure to download the .NET 6 SDK.


![.NET 6 SDK](READMEmedia/dotnet_6.png)


- If you use Visual Studio, download 6.0 either from the Visual Studio version of the .NET SDK from [here](https://dotnet.microsoft.com/en-us/download/visual-studio-sdks)

![Visual Studio 2022 .NET 6 SDK](READMEmedia/dotnet_6_vs.png)

 or through Visual Studio Installer > Visual Studio 2022 > Modify > Individual Components.

![.NET 6 Visual Studio component](READMEmedia/dotnet_6_vs_component.png)


# Visual Studio Installation (Optional, but highly recommended)
- We recommend using Visual Studio while developing with .NET, as Visual Studio was specially designed for .NET and C++ and contains many useful features to speed up development such as IntelliSense and GitHub code snippet finder. Download Visual Studio 2022 from [here](https://visualstudio.microsoft.com/).
![Visual Studio 2022 Community](READMEmedia/vs_community.png)
- You can find instructions to use it with Godot [here](https://docs.godotengine.org/en/stable/contributing/development/configuring_an_ide/visual_studio.html). (Note that Visual Studio does _not_ require a solution file, you can select "Open Folder" or "Open .csproj" and it will generate a solution file)
- Visual Studio's other features like hot reload will also aid you on developing things other than games,  such as .NET MAUI cross-platform applications. If you use Visual Studio for other things, we recommend using .NET 8, but Godot games will use .NET 6. 
# .NET community
- Now that you've installed the .NET SDK, you're a part of the .NET community! We welcome you to start exploring .NET for yourself.
- npxl32 has previous experience as a .NET developer, so ask them for help if you need it.
- .NET is a platform of programming languages and libraries created by Microsoft. The platform most prominently includes the langauges C# (C-Sharp), F# (F-Sharp), and VB.
- The .NET platform lets you create cross-platform apps for Desktop, Mobile, and Apple TV, single-page application websites, normal websites, machine learning applications, IoT apps, Games through [a lot of game engines](https://dotnet.microsoft.com/en-us/apps/games/engines), and Cloud Applications!
- C# is the most used .NET language, and is very similar in terms of syntax to other programming languages. C++, Java, and JavaScript developers will feel right at home developing in C#!
- These languages all compile to a single language called "IL" (Intermediate Language). This is also sometimes called MSIL (Microsoft Intermediate Language). The IL code is then executed through the .NET runtime, which works on all major operating systems. The .NET runtime can either be packaged with your app or installed separately by your users.
- There are multiple implementations of .NET that have been made. First there was the .NET framework released in 2002. The .NET framework was Windows-only and was composed of VB and C#. Then came Mono, which aimed to create a cross-platform implementation of the .NET framework. Mono worked on Windows, Mac, and Linux, and still exists today as a shadow of its former self. Next came Xamarin which was a company that supported Mono, and created Xamarin.Android (formerly Mono for Android) and Xamarin.iOS (formerly MonoTouch.) After that, there was .NET Core which was an official cross-platform implementation of the .NET framework by Microsoft. Around this time, they also bought Xamarin. Xamarin.Forms is what followed, which was a cross-platform app creation framework that would let you build for Windows, Linux, Android, and even Samsung Tizen and Apple tvOS. Afterwards, Microsoft created .NET MAUI, the evolution of Xamarin.Forms, which adds MacOS and iOS support via MacCatalyst.
- NuGet is .NET's package manager, which is where you can find libraries to use in your .NET code.
# Code editing
## Forking and cloning
On the repository you would like to contribute to, follow these steps.
- If this is your first time, click "fork", and fork the repository. 
- Edit the code as described below.
- Go back to the original repository, click on "Pull Requests", and open a new pull request.

## Editing the code and Git
- At BluePlay, if you can't tell yet, we use a version control system called Git.
- On Git, forking a repository is when you create your own duplicate to make your own changes.
- On Git, a commit is a change to the files.
- On Git, a pull request is when you request your code from your fork to be merged with the original repository.
- At BluePlay, we recommend you use GitHub Desktop or Git CLI (not to be confused with GitHub CLI) to edit your code with bigger commits. The difference is that GitHub Desktop is GitHub only, while Git CLI works with any Git service (like GitHub, GitLab, and Bitbucket), you can use whichever tools you want with the Git CLI, and that you'll have to know how to use a command line to use Git CLI.
- To edit the code: follow these steps:

1. Go into your fork of the repository on GitHub.
2. If this is a small commit, like a change to a README, you can use the pencil button on the GitHub view of your repository. 
3. If this is a game, and you haven't cloned it yet, click the green code button.
![GitHub Code Button](READMEmedia/github_code_button.png)
4. Clone it using GitHub Desktop or Git CLI with the URL it gives you. Git CLI example: 
![Git CLI example](READMEmedia/git_cli_clone.png)
5. If you are on Git CLI, it will now have created a directory with the cloned repository in it. If you are on Windows, we recommend opening the directory via the command line to get used to the CLI. Windows example here:
![Cloned repository in Windows Explorer](READMEmedia/explorer_cloned_repository.png)

Once it is done, you can now edit the code and push the changes to the repository using Git!
Now that you've cloned the repository, open it in Godot:
1. Open Godot, (found in your extracted folder, make sure not to open the "console" version.)<br />
![GUI version](READMEmedia/godot_noconsole.png)
2. Click Import
![import button](READMEmedia/godot_import.png)
3. Select the folder containing the repository you cloned. (Of course, normally you would select a godot game instead of a README)
![Opening the folder in Godot](READMEmedia/godot_opening_repository_img.png)

Once you import the folder into godot, hit CTRL+S.
- Once you are done editing the game, use GitHub Desktop or the Git CLI to push your changes to your fork. Here is a tutorial for Git CLI:
1. Change to the directory that the repository is in with the "CD" command. (The equivalent of double-clicking a folder in explorer)
2. Add all files to the commit with "git add --all".
3. Actually do the commit with "git commit -m [commit message here]".
4. Push the commit with "git push". (This step will make the commits appear on GitHub)
![Git Add Commit Push](READMEmedia/git_add_commit_push.png)
5. BONUS: if you make a change on GitHub, it will not let you push until you update the cloned repository. Type "git pull" to do this.
6. BONUS BONUS: if you need to make an empty commit, type "git commit -m [commit message here] --allow-empty" instead of "git commit -m [commit message here]".
- Back on GitHub, open a pull request.