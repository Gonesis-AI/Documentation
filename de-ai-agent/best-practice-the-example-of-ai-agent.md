# Best Practice: The Example of AI Agent

This example shows how to create an AI Agent (a single NFT) based on AI721.

## LLM

Choose any large language model to load trait model. Here we use gpt-4.&#x20;

```
llm = "llm://gpt-4"
```

## Trait Model Guide

The traits and trait model of a single AI agent are **OPTIONAL**, unless you want it to highlight key differentiating features in the standard ERC721 format, or create unique personality for more fun. The trait model can define key personality variables to offer more interesting gameplay options.

A traits example of an AI agent would be like (after converting):

```
{
    "Hair":"Yellow long spiky",
    "Face":"Round blue sunglasses",
    "Clothing": "Shinto robe",
}
```

Then you can write a simple trait model like:

"You have the hair: \{{Hair\}}, and face: \{{Face\}}, wearing \{{Clothing\}}. Please use a style and tone that match these characteristics."

### The Final Prompt

"You have the hair: Yellow long spiky, and face: Round blue sunglasses, wearing Shinto robe. Please use a style and tone that match these characteristics."

## Workflow

Check the [guide](workflow.md) of workflow.

## AI721 Metadata Example

Upload trait model, public memories and workflow to your storage service or IPFS get `{{trait_model_url}}` and `{{public_memories_url}}`. Then combine these fields with ERC721 metadata.&#x20;

Here is an example for Azuki #3582:

<pre><code>{
    // ERC721 metadata fields
<strong>    name: "Azuki #3582",
</strong>    image: "ipfs://QmYDvPAXtiJg7s8JdRBSLWdgSphQdac8j1YuQNNxcGE1hg/3582.png",
    attributes: [
        {
            trait_type: "Hair",
            value: "Yellow long spiky"
        },
        {
            trait_type: "Face",
            value: "Round blue sunglasses"
        },
        {
            trait_type: "Clothing",
            value: "Shinto robe"
        },
    ],
    // AI fields
    llm: "llm://gpt-4",
    trait_model: {{trait_model_url}}
    public_memories: {{public_memories_url}},
    workflow:{{workflow_url}}
}
</code></pre>
