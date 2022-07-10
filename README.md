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

The example for Cloudinary uploader : https://github.com/Kentico/kontent-custom-element-cloudinary

A similar example for Bynder: https://github.com/Kentico/kontent-custom-element-bynder
Which results as: https://assets-us-01.kc-usercontent.com/4ec262a7-3d6c-008c-aa10-1e6ffc6c2e14/58d37abd-dd00-4dbf-85ba-4ebdf281bede/bynder.gif

But now, we are going to add a Cloudinary Custom Element uploader, so fork https://github.com/Kentico/kontent-custom-element-cloudinary , then host it on Github as follows:

![github_host](https://user-images.githubusercontent.com/20809372/177953801-b12c745f-e3ef-47b6-9ad9-a56387db1340.PNG)

**Note** You can't just pull this repository to localhost and run it there, because you have to embed it into Kontent; It won't work as a standalone app.

![not_standalone](https://user-images.githubusercontent.com/20809372/177953890-08082e16-1fab-4adf-a1cb-c12ca4fc9de7.PNG)

## Make the Cloudinary Custom Element uploader

![setup1](https://user-images.githubusercontent.com/20809372/177953963-6308895b-33d9-43f9-956f-1adc2d8c2580.png)

Above is what https://kontent.ai/learn/tutorials/develop-apps/integrate/content-editingextensions/#a-displaying-your-custom-editor-in-kontent is essentially trying to say.

https://github.com/atabegruslan/kontent-custom-element-cloudinary/blob/main/README_orig.md#configuring-the-custom-element

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

## Preview

Tutorial: https://kontent.ai/learn/tutorials/develop-apps/build-strong-foundation/set-up-preview/

Go to **Settings** > **API Keys**. For this, you will definitely need your **Project ID**. You may also need your **API Key** (depends on what you want to do, but for simple things **Project ID** is enough).

![preview0](https://user-images.githubusercontent.com/20809372/177968219-7ec2ad34-2067-480f-bdae-03f73dbd7156.png)

Now you need to **write a client app** that utilizes the **Delivery API**.

Recall, Kontent have 3 set of APIs that you can interact with:

![apis](https://user-images.githubusercontent.com/20809372/177968951-5f67296e-11c9-4433-995e-41ed97fa8004.png)

The plain Delivery APIs in its pure HTTPS form can be downloaded and imported into POSTMAN from here: https://kontent.ai/learn/tutorials/develop-apps/get-started/postman-collection/

For the 3 content items that comes out of the box, Kontent already have an **example client app**, which we can imitate.

![default](https://user-images.githubusercontent.com/20809372/177969906-8dc8d38f-30e3-454f-a998-460e889febb0.png)

This example app was made by using https://github.com/Kentico/kontent-sample-app-react , which is hosted on Github Pages here `https://kentico.github.io/kontent-sample-app-preview-react/{rest of the URL}` . 

After coding up your client app: https://github.com/atabegruslan/kontent-cloudinary-demo-client

Host it

![preview1](https://user-images.githubusercontent.com/20809372/177971955-0add2227-eb23-4c4a-8a85-dd3c76458578.png)

Define your Preview URL formats

![preview2](https://user-images.githubusercontent.com/20809372/177972087-c9b6fc5c-3f1b-4ffb-9109-c2a0c6cc46f0.png)

Click Preview

![preview3](https://user-images.githubusercontent.com/20809372/177972184-c0b69c42-1ccc-48f1-aa53-136e2a450617.png)

Results

![preview4](https://user-images.githubusercontent.com/20809372/177972262-db4b40bb-61cc-4efc-a234-ece150a269c6.png)

![preview5](https://user-images.githubusercontent.com/20809372/177972312-975431f2-a36b-45dc-9117-78bc6445e61c.png)

---

## Make ANY custom element

- https://www.youtube.com/watch?v=6nFsX22CZXM
- Deeper tech notes: https://kontent.ai/learn/reference/custom-elements-js-api/
- Examples to imitate: https://github.com/Kentico/kontent-custom-element-samples

## Support

- https://kontent.ai/community/
- https://kontent.ai/discord
- Chat bubble at the bottom-right of https://kontent.ai/

## Other Resources

- Install locally: https://www.youtube.com/watch?v=PmoXboT8FHw
  - https://xperience.io/get-started/trial
- Develop: https://www.youtube.com/watch?v=dpkQz5vNPDQ
- Install hosted: https://xperience.io/get-started/hosted-trial
- https://github.com/Kentico/custom-element-devkit
- https://kontent.ai/learn/reference/delivery-api/
- https://kontent.ai/developers/?itm_medium=home-hero&itm_campaign=developers
- https://github.com/Kentico/kontent-delivery-sdk-js
- https://kontent.ai/learn/tutorials/develop-apps/overview/?tech=javascript
- https://kontent.ai/learn/tutorials/write-and-collaborate/create-content/compose-content-in-rich-text/#a-adding-components
