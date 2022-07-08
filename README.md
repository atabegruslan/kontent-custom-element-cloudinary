# Cloudinary for Kentico Kontent 

## Have a Cloudinary account

![cloudinary_account](https://user-images.githubusercontent.com/20809372/177953019-2f2e5576-d6b6-4bca-b056-b703369e38a3.png)

## Good-for-imitation tutorial

This tutorial is about Markdown editor, not Cloudinary uploader. But the steps are analogous.

https://kontent.ai/learn/tutorials/develop-apps/integrate/content-editing-extensions/

## Examples of Custom Element

- https://kontent.ai/integrations/
- https://kentico.github.io/kontent-custom-element-samples/gallery/

![digital_asset_management](https://user-images.githubusercontent.com/20809372/177953362-2221670a-0185-4f9f-afed-186c15a4d0ae.PNG)

The example for Cloudinary uploader : https://github.com/Kentico/kontent-custom-elementcloudinary

A similar example for Bynder: https://github.com/Kentico/kontent-custom-element-bynder
Which results as: https://assets-us-01.kc-usercontent.com/4ec262a7-3d6c-008c-aa10-1e6ffc6c2e14/58d37abd-dd00-4dbf-85ba-4ebdf281bede/bynder.gif

But now, we are going to add a Cloudinary Custom Element uploader, so fork https://github.com/Kentico/kontent-custom-element-cloudinary , then host it on Github as follows:

![github_host](https://user-images.githubusercontent.com/20809372/177953801-b12c745f-e3ef-47b6-9ad9-a56387db1340.PNG)

**Note** You can't just pull this repository to localhost and run it there, because you have to embed it into Kontent; It won't work as a standalone app.

![not_standalone](https://user-images.githubusercontent.com/20809372/177953890-08082e16-1fab-4adf-a1cb-c12ca4fc9de7.PNG)

## Make the Cloudinary Custom Element uploader

![setup1](https://user-images.githubusercontent.com/20809372/177953963-6308895b-33d9-43f9-956f-1adc2d8c2580.png)

Above is what https://kontent.ai/learn/tutorials/develop-apps/integrate/content-editingextensions/#
a-displaying-your-custom-editor-in-kontent is essentially trying to say.

## Create some contents and test the Cloudinary Custom Element uploader

![setup2](https://user-images.githubusercontent.com/20809372/177954102-c9082f5c-f665-4159-a607-e34c3edf42ea.png)

![setup3](https://user-images.githubusercontent.com/20809372/177954178-79f61c80-4e58-474d-8785-05ae2a86903b.png)

Note that the Cloudinary URL reference is still used. https://github.com/Kentico/kontentcustom-element-cloudinary#what-is-saved  
It is also evident when you get this content via Kontent's Delivery API  

- https://kontent.ai/learn/tutorials/develop-apps/integrate/integrations-overview/
  - https://kontent.ai/learn/reference/kontent-apis-overview/
  - https://kontent.ai/learn/tutorials/develop-apps/get-started/postman-collection/

![](https://user-images.githubusercontent.com/20809372/177956683-3dabc2af-00b0-4a03-b8c2-1361cae44d20.png)

**Note** you may have noticed that you didn't do the things in this step https://kontent.ai/learn/tutorials/develop-apps/integrate/content-editing-extensions/#aensuring- secure-hosting (ie: You didn't explicitly made any iFrames). That's because: The custom element is just a simple web application. Once you add a custom element in Kontent, setup the URL and the settings, Kontent then adds it into the app through iframe.

## Make ANY custom element

- https://www.youtube.com/watch?v=6nFsX22CZXM
- Deeper tech notes: https://kontent.ai/learn/reference/custom-elements-js-api/
- Examples to imitate: https://github.com/Kentico/kontent-custom-element-samples
- Further help and contact: https://kontent.ai/discord
