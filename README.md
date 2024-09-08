# Build Your Own Copilot with Azure Cosmos DB - Hackathon

Welcome to the Build Your Own Copilot with Azure Cosmos DB hackathon!

## Introduction

This hackathon is designed to help you expand your knowledge about the Generative AI patterns used in the **Build Your Own Copilot with Azure Cosmos DB** solution accelerator. The solution accelerator demonstrates how to design and implement a Generative AI solution that incorporates Azure Cosmos DB with Azure OpenAI Service along with other key Azure services, to build an AI assistant user interface.

The hackathon consists of six challenges as follows:

Challenge number | Challenge code | Description
--- | --- | ---
1 | `[Challenge 1]` | Deploy the solution accelerator to your Azure subscription and explore the solution architecture.
2 | `[Challenge 2]` | Learn about the basics of Semantic Kernel, a Large Language Model (LLM) orchestrator that powers the solution accelerator.
3 | `[Challenge 3]` | Learn about intercepting and using key assets from Semantic Kernel's inner workings - prompt and function calling data.
4 | `[Challenge 4]` | Learn how prompts are used in the solution accelerator and experiment with changes to the prompts.
5 | `[Challenge 5]` | Learn about the inner workings and applications of semantic caching in the solution accelerator.
6 | `[Challenge 6]` | Learn about implementing system commands based on user input in the solution accelerator.

> [!IMPORTANT]
> We recommend that you complete the challenges in the order they are presented. The challenges are designed to build on each other, and completing them in order will help you understand the solution accelerator better.

Except for Challenge 1, each challenge will have a set of coding tasks that you need to complete. This repo provides you with the starter project (under the `code/starter` folder).

> [!NOTE]
> At this point, it is a good moment to clone this repository to your local machine. You can do this by running the following command in your terminal or command prompt:

```cmd
git clone https://github.com/solliancenet/byoc-hackathon <your_folder_name>
```

For each challenge, you can easily find the code snippets that you need to modify or add by searching for the challenge code in the code files. For example, to identify the code snippets for Challenge 2, search for `[Challenge 2]` in the code files. In Visual Studio 2022, you can use the `Edit -> Find and Replace -> Find in Files` menu option of the `Ctrl + Shift + F` keyboard command to search for the challenge code. The result of the search will return multiple locations, each labeled as `// TODO: [Challenge X][Exercise X.E.T]` where `X` is the challenge number, `E` is the exercise number, and `T` is the task number.

> [!IMPORTANT]
> Within each challenge, we also recommend that you complete the exercises in the order they are presented. The exercises are designed to build on each other, and completing them in order will help you understand the solution accelerator better. Make sure you read the hints added as code comments to help you complete the tasks.

Last but not least, for some of the challenges we are also providing some open-ended exercises which do not have a specific solution. These exercises are designed to help you think about the solution accelerator and its components in a more creative way. We encourage you to complete these exercises as well, ideally at the end of the hackathon, after you have successfully completed all the challenges and their exercises.

For each challenge the recommended order of operations is the following:

1. Identify all the exercises for the challenge and read the hints provided in the code comments.
2. Attempt to tackle the exercises in the order they are presented. For each exercise, check the list of suggested readings to help you understand the concepts you need to apply (those lists are provided below for each challenge).
3. Take a note of any open-ended exercises and try to complete them at the end of the hackathon.

## Challenge 1: Deploy the solution accelerator to your Azure subscription and explore the solution architecture

The main repository for the solution accelerator is located here: [Build Your Own Copilot with Azure Cosmos DB](https://github.com/Azure/BuildYourOwnCopilot). Start by completing the following tasks:

- Read the information in the landing page of the solution accelerator repository.
- Read the [Key Concepts](https://github.com/Azure/BuildYourOwnCopilot/blob/main/docs/concepts.md) document to understand the key concepts of the solution accelerator. You wil likely return to this document throughout the hackathon to revisit some of the concepts related to each challenge.
- Deploy the solution accelerator to your Azure subscription by following the instructions in the [Deployment Guide](https://github.com/Azure/BuildYourOwnCopilot/blob/main/docs/deployment.md).

> [!NOTE]
> For the purpose of this hackathon, we recommend that you choose the Azure Container Apps (ACA) option which is the quickest to deploy.

> [!IMPORTANT]
> Before you proceeed, make sure you review the prerequisites list and you deploy them.

- Once the deployment is complete, follow the steps in the [Quickstart section](https://github.com/Azure/BuildYourOwnCopilot/blob/main/docs/quickstart.md) to explore the solution accelerator.

- Set up your environment for running locally and debugging. You can find the instructions in the [Run locally and debug](https://github.com/Azure/BuildYourOwnCopilot/blob/main/docs/runlocal.md) section in the solution acceleartor repository.

> [!NOTE]
> The process of deploying the solution accelerator will involve cloing the solution accelerator repository to your local machine. This is a different repository than the one you are currently in, which is the hackathon repository. You will need to follow the steps for running locally and debugging only for the starter project in this hackathon repository.

- Once you complete the setup for running locally ensure you can run the hackathon starter project using the Azure artifacts deployed by the solution accelerator setup in your Azure subscription.

> [!IMPORTANT]
> As you might have noticed already, the solution accelerator repository is a public repository. Since this hackathon is based on the solution accelerator, the full set of solutions for the challenges and their exercises are easibly accessible in the solution accelerator repository. Copying and pasting them allows one to complete the hackathon in probably less than a half hour. That would completely defeat the purpose of this exercise which is to produce the solutions on your own, by understanding the inner workings of the solution accelerator and the technologies it is built upon. This is why we strongly encourage you to try to solve the challenges on your own first. If you get stuck, you can always refer to the solution accelerator repository for guidance, but that should be your last resort.

## Challenge 2: Learn about the basics of Semantic Kernel

Here are some suggested readings that will help you address the tasks in the challenge:

- [Understanding the kernel](https://learn.microsoft.com/en-us/semantic-kernel/concepts/kernel?pivots=programming-language-csharp)
- [What is a Plugin?](https://learn.microsoft.com/en-us/semantic-kernel/concepts/plugins/?pivots=programming-language-csharp)
- [How to use function calling with Azure OpenAI Service](https://learn.microsoft.com/en-us/azure/ai-services/openai/how-to/function-calling)
- [What is a Planner?](https://learn.microsoft.com/en-us/semantic-kernel/concepts/planning?pivots=programming-language-csharp)
- [Embeddings](https://platform.openai.com/docs/guides/embeddings/use-cases)
- [Build Your Own Copilot with Azure Cosmos DB - Key Concepts](https://github.com/Azure/BuildYourOwnCopilot/blob/main/docs/concepts.md)

This challenge does not have open-ended exercises.

## Challenge 3: Learn about intercepting and using key assets from Semantic Kernel's inner workings

Here are some suggested readings that will help you address the tasks in the challenge:

- [Using Filters in Semantic Kernel](https://devblogs.microsoft.com/semantic-kernel/filters-in-semantic-kernel/)

Open-ended exercises (recommended to be completed at the end of the hackathon):
- Exercise `3.3.1` - implement your own `IFunctionInvocationFilter`.

## Challenge 4: Learn how prompts are used in the solution accelerator

Here are some suggested readings that will help you address the tasks in the challenge:

- [Prompt injection article from the Open Worldwide Application Security Project (OWASP)](https://genai.owasp.org/llmrisk/llm01-prompt-injection/) to understand the core principles of prompt injection vulnerabilities.

Open-ended exercises (recommended to be completed at the end of the hackathon):
- Implement an `ISystemPromptService` class that retrieves the system prompt from a different source (e.g., Azure Cosmos DB, GitHub, etc.) and use it in the solution.

## Challenge 5: Learn about the inner workings and applications of semantic caching

Here are some suggested readings that will help you address the tasks in the challenge:
- [Build Your Own Copilot with Azure Cosmos DB - Key Concepts](https://github.com/Azure/BuildYourOwnCopilot/blob/main/docs/concepts.md)

This challenge does not have open-ended exercises.

## Challenge 6: Learn about implementing system commands based on user input

Here are some suggested readings that will help you address the tasks in the challenge:
- [Build Your Own Copilot with Azure Cosmos DB - Key Concepts](https://github.com/Azure/BuildYourOwnCopilot/blob/main/docs/concepts.md)

Open-ended exercises (recommended to be completed at the end of the hackathon):
- Create a new system command and plug it into the system.

Temporary docker fix:

azd hooks run predeploy
azd provision
Update the images in ACR
azd hooks run postdeploy


Instructions to update the images:

Go to the ca-chatservicew-.. container app in the resource group
Select Application -> Revisions and replicas
Select Create new revision from the top toolbar
Select the container image named main
Set Image source to Docker Hub or other registries
Set Authentication to Public
Set registry login server to `crdszvooit6qzhq.azurecr.io`
Set Image and tag to `buildyourowncopilot/chatapi-byoc-01:azd-deploy-1722937955`


Go to the ca-search-.. container app in the resource group
Select Application -> Revisions and replicas
Select Create new revision from the top toolbar
Select the container image named main
Set Image source to Docker Hub or other registries
Set Authentication to Public
Set registry login server to `crdszvooit6qzhq.azurecr.io`
Set Image and tag to `buildyourowncopilot/userportal-byoc-01:azd-deploy-1722937987`