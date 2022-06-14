# 01 - .NET Basics

## 1. Project / Solution

### 1.1 Structure
Every C# Program is using Microsoft .NET<br>
There are two *main* Editions, .NET Framework and .NET Core<br>
.NET Framework is mostly used for Windows-only Development, as Programs
compiled with .NET Framework as Target only work with Windows. <br>
.NET Core is more *universal* and is useable on Windows, MacOS and Linux-based Operating Systems.

### 1.2 Creating a .NET Project
In Loco Software, we only use .NET Core - and therefor i will only cover .NET Core in this Lecture. <br>
.NET Core Projects can be created multible ways, using a IDE like Visual Studio or JetBrains Raider,<br>
and the .NET Console Utility (also called *.NET CLI*)
#### 1.2.1 Creating using Visual Studio
1. Open Visual Studio (>2017)
2. Create a new Project or open a existing Solution and add a new Project by right-Clicking on the Solution -> Add
3. Under *Project Templates*, select the Type of Application you want:
    - *Console App* for Console Based Applications
    - *Class Library* for Shared Libraries (DLL)
    - *ASP .NET Core Web App* for Web Applications (Client, Server, API)
4. Now a Solution including a Project was created for you to use. 

#### 1.2.2 Creating using the .NET CLI
1. Open a Command Prompt (Windows Terminal, MacOS Terminal/iTerm2, Linux Terminal)
2. For help, enter `dotnet new`
    ```
    ❯ dotnet new
    Mit dem Befehl "dotnet new" wird ein NET-Projekt basierend auf einer Vorlage erstellt.

    Allgemeine Vorlagen:
    Vorlagenname          Kurzname      Sprache     Tags
    --------------------  ------------  ----------  -------------------
    ASP.NET Core Web App  webapp,razor  [C#]        Web/MVC/Razor Pages
    Blazor Server App     blazorserver  [C#]        Web/Blazor
    Klassenbibliothek     classlib      [C#],F#,VB  Common/Library
    Konsolen-App          console       [C#],F#,VB  Common/Console
    Windows Forms App     winforms      [C#],VB     Common/WinForms
    WPF-Anwendung         wpf           [C#],VB     Common/WPF

    Beispiel:
    dotnet new console

    Vorlagenoptionen anzeigen mit:
    dotnet new console -h
    Alle installierte Vorlagen anzeigen mit:
    dotnet new --list
    Auf NuGet.org verfügbare Vorlagen anzeigen mit:
    dotnet new web --search
    ```
3. You have here a similar selection as like in Visual Studio or similar IDEs, just created using the CLI
4. For general .NET CLI Help enter `dotnet --help`
5. **Note: If you create a Project using the CLI, no Solution will be created only the .csproj itself!**

### 1.3 Demo Projects
- There a multiple Demo Projects (Console Applications) in sub-folders so you can see how it will look like

## 1.4 File Structure
When creating a .NET Project, there are some boilerplate Files created:
| File / Folder | Description                  |
|---------------|------------------------------|
| bin           | build binaries               |
| obj           | build objects                |
| program.cs    | main entrypoint into project |
| *.csproj      | C# Project File              |
| *.sln         | Visual Studio Solution       |