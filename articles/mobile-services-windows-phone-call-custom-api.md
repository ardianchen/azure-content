<properties urlDisplayName="Call a custom API from the client" pageTitle="Call a custom API from a Windows Phone client - Mobile Services" metaKeywords="" description="Learn how to define a custom API and then call it from a Windows Phone app that use Azure Mobile Services." metaCanonical="" services="mobile-services" documentationCenter="windows" title="" authors="ggailey777" solutions="" manager="dwrede" editor=""/>

<tags ms.service="mobile-services" ms.workload="mobile" ms.tgt_pltfrm="mobile-windows-phone" ms.devlang="dotnet" ms.topic="article" ms.date="10/06/2014" ms.author="glenga" />

# Call a custom API from the client

[WACOM.INCLUDE [mobile-services-selector-call-custom-api](../includes/mobile-services-selector-call-custom-api.md)]

This topic shows you how to call a custom API from a Windows Phone app. A custom API enables you to define custom endpoints that expose server functionality that does not map to an insert, update, delete, or read operation. By using a custom API, you can have more control over messaging, including reading and setting HTTP message headers and defining a message body format other than JSON.

The custom API created in this topic gives you the ability to send a single POST request that sets the completed flag to `true` for all the todo items in the table. Without this custom API, the client would have to send individual requests to update the flag for each todo item in the table.

You will add this functionality to the app that you created when you completed the [Add Mobile Services to an existing app](/en-us/documentation/articles/mobile-services-windows-phone-get-started-data/) tutorial. To do this, you will complete the following steps:

1. [Define the custom API]
2. [Update the app to call the custom API]
3. [Test the app] 

This tutorial is based on the GetStartedWithData sample, a simple TodoList app. Before you start this tutorial, you must first complete [Add Mobile Services to an existing app](/en-us/documentation/articles/mobile-services-windows-phone-get-started-data/).

## <a name="define-custom-api"></a>Define the custom API

[WACOM.INCLUDE [mobile-services-create-custom-api](../includes/mobile-services-create-custom-api.md)]

[WACOM.INCLUDE [mobile-services-windows-phone-call-custom-api](../includes/mobile-services-windows-phone-call-custom-api.md)]

## Next steps

Now that you have created a custom API and called it from your Windows Phone app, consider finding out more about the following Mobile Services topics:

* [Mobile Services server script reference]
  <br/>Learn more about creating custom APIs.

* [Store server scripts in source control]
  <br/> Learn how to use the source control feature to more easily and securely develop and publish custom API script code.

<!-- Anchors. -->
[Define the custom API]: #define-custom-api
[Update the app to call the custom API]: #update-app
[Test the app]: #test-app
[Next Steps]: #next-steps

<!-- Images. -->


<!-- URLs. -->
[Mobile Services server script reference]: http://go.microsoft.com/fwlink/?LinkId=262293
[Get started with Mobile Services]: /en-us/documentation/articles/mobile-services-windows-phone-get-started/
[Get started with data]: /en-us/documentation/articles/mobile-services-windows-phone-get-started-data/
[Get started with authentication]: /en-us/documentation/articles/mobile-services-windows-phone-get-started-users/
[Get started with push notifications]: /en-us/documentation/articles/mobile-services-windows-phone-get-started-push/

[Store server scripts in source control]: /en-us/documentation/articles/mobile-services-store-scripts-source-control
