---
title: Visual Studio IntelliCode
titleSuffix: ""
ms.date: 05/21/2019
ms.prod: visual-studio-family
ms.technology: intellicode
ms.topic: conceptual
author: gewarren
ms.author: gewarren
manager: jillfra
---
# Overview of IntelliCode

Visual Studio IntelliCode enhances software development using artificial intelligence. IntelliCode delivers [context-aware code completions](#context-aware-code-completions) and guides developers to adhere to the [patterns and styles of their team](code-style-inference.md). IntelliCode is available in [Visual Studio](intellicode-visual-studio.md) and as an extension for [Visual Studio Code](intellicode-visual-studio-code.md).

For more information and to sign up for news and updates, see [Visual Studio IntelliCode](https://visualstudio.microsoft.com/services/intellicode/).

## Install IntelliCode

Before you begin, ensure you have a version of Visual Studio or Visual Studio Code that supports IntelliCode. The minimum requirements are:

- Visual Studio Code October 2018 Release 1.29 or later
- Visual Studio 2019 (any version and edition)
- Visual Studio 2017 version 15.8 and later (any edition)

The following table contains details about how to obtain IntelliCode for your development environment:

|Development environment|Installation instructions|
|-|-|
|![Visual Studio Code logo](https://docs.microsoft.com/visualstudio/intellicode/media/vs-code-logo.svg)|1. Install [Visual Studio Code](https://code.visualstudio.com/) for Windows, MacOS, or Linux.<br />2. [Download the Visual Studio IntelliCode extension](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode) from the marketplace, or install it directly from the **Extensions** view in Visual Studio Code.<br />3. Reload and wait for dependencies to download and install (see status bar).|
|![Visual Studio 2019 logo](https://docs.microsoft.com/visualstudio/intellicode/media/vs-ide-2019.svg)|1. [Download Visual Studio 2019](https://visualstudio.microsoft.com/downloads/?utm_medium=microsoft&utm_source=docs.microsoft.com&utm_campaign=inline+link&utm_content=download+vs2019) version 16.1 or later.<br />2. Install a [supported workload](intellicode-visual-studio.md#supported-workloads), such as .NET desktop development.<br />3. Visual Studio IntelliCode is installed by default.<br /><br />Or:<br /><br />1. Download a version of Visual Studio 2019 prior to version 16.1.<br />2. [Download the Visual Studio IntelliCode extension](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.VSIntelliCode) from Visual Studio Marketplace.|
|![Visual Studio 2017 logo](https://docs.microsoft.com/visualstudio/intellicode/media/vs-ide-2017.svg)|1. [Download Visual Studio 2017](https://visualstudio.microsoft.com/vs/older-downloads/?utm_medium=microsoft&utm_source=docs.microsoft.com&utm_campaign=vs+2017+download) version 15.8 or later.<br />2. [Download the Visual Studio IntelliCode extension](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.VSIntelliCode) from Visual Studio Marketplace.|

## Context-aware code completions

IntelliCode provides AI-assisted IntelliSense in both Visual Studio and Visual Studio Code. IntelliCode suggestions appear at the top of the completion list with a star icon next to them:

![Starred IntelliSense suggestions using IntelliCode in Visual Studio](media/starred-intellisense-suggestions.png)

The completion list suggests the most likely correct API for a developer to use rather than presenting a simple alphabetical list of members. To provide this dynamic list, IntelliCode uses the developer's current code context as well as patterns based on thousands of highly rated, open-source projects on GitHub. The results form a model that predicts the most likely and most relevant API calls.

### Supported languages

The supported languages for AI-assisted IntelliSense completions are:

- C#, C++, XAML, JavaScript, and TypeScript for Visual Studio.

- Java, JavaScript, TypeScript, and Python for Visual Studio Code.

## Telemetry

We capture some anonymized usage and error-reporting data to help improve IntelliCode. No user-defined code is sent to Microsoft, but we collect information about your use of the IntelliCode results.

For base model suggestions, which are open source or .NET types and members, we capture whether you selected an IntelliCode suggestion and log the name of the suggestion. Microsoft uses the data to monitor the quality of the base model. For custom models, we capture whether you selected an IntelliCode suggestion but *do not* log the names of your user-defined types or methods.

In Visual Studio, you can opt out of the [Visual Studio Experience Improvement Program](/visualstudio/ide/visual-studio-experience-improvement-program), which turns off data collection for IntelliCode too. From the menu bar, select **Help** > **Send Feedback** > **Settings**. In the **Visual Studio Experience Improvement Program** dialog, select **No, I would not like to participate** and then select **OK**.

In Visual Studio Code, you can disable telemetry reporting by following [these instructions](https://code.visualstudio.com/docs/supporting/faq#_how-to-disable-telemetry-reporting).

IntelliCode may periodically ask you to complete an anonymous survey. You can also sign up for news and updates but are not required to do so.

## See also

- [Visual Studio IntelliCode FAQ](faq.md)
