---
title: 'Tutorial: Azure Active Directory integration with SumTotalCentral | Microsoft Docs'
description: Learn how to configure single sign-on between Azure Active Directory and SumTotalCentral.
services: active-directory
documentationCenter: na
author: jeevansd
manager: femila
ms.reviewer: joflore

ms.assetid: 93ad629a-f516-4cac-bfe2-a77257e3a797
ms.service: active-directory
ms.component: saas-app-tutorial
ms.workload: identity
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: article
ms.date: 12/12/2017
ms.author: jeedes

---
# Tutorial: Azure Active Directory integration with SumTotalCentral

In this tutorial, you learn how to integrate SumTotalCentral with Azure Active Directory (Azure AD).

Integrating SumTotalCentral with Azure AD provides you with the following benefits:

- You can control in Azure AD who has access to SumTotalCentral.
- You can enable your users to automatically get signed-on to SumTotalCentral (Single Sign-On) with their Azure AD accounts.
- You can manage your accounts in one central location - the Azure portal.

If you want to know more details about SaaS app integration with Azure AD, see [what is application access and single sign-on with Azure Active Directory](../manage-apps/what-is-single-sign-on.md).

## Prerequisites

To configure Azure AD integration with SumTotalCentral, you need the following items:

- An Azure AD subscription
- A SumTotalCentral single sign-on enabled subscription

> [!NOTE]
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

## Scenario description
In this tutorial, you test Azure AD single sign-on in a test environment. 
The scenario outlined in this tutorial consists of two main building blocks:

1. Adding SumTotalCentral from the gallery
2. Configuring and testing Azure AD single sign-on

## Adding SumTotalCentral from the gallery
To configure the integration of SumTotalCentral into Azure AD, you need to add SumTotalCentral from the gallery to your list of managed SaaS apps.

**To add SumTotalCentral from the gallery, perform the following steps:**

1. In the **[Azure portal](https://portal.azure.com)**, on the left navigation panel, click **Azure Active Directory** icon. 

	![The Azure Active Directory button][1]

2. Navigate to **Enterprise applications**. Then go to **All applications**.

	![The Enterprise applications blade][2]
	
3. To add new application, click **New application** button on the top of dialog.

	![The New application button][3]

4. In the search box, type **SumTotalCentral**, select **SumTotalCentral** from result panel then click **Add** button to add the application.

	![SumTotalCentral in the results list](./media/sumtotalcentral-tutorial/tutorial_sumtotalcentral_addfromgallery.png)

## Configure and test Azure AD single sign-on

In this section, you configure and test Azure AD single sign-on with SumTotalCentral based on a test user called "Britta Simon".

For single sign-on to work, Azure AD needs to know what the counterpart user in SumTotalCentral is to a user in Azure AD. In other words, a link relationship between an Azure AD user and the related user in SumTotalCentral needs to be established.

In SumTotalCentral, assign the value of the **user name** in Azure AD as the value of the **Username** to establish the link relationship.

To configure and test Azure AD single sign-on with SumTotalCentral, you need to complete the following building blocks:

1. **[Configure Azure AD Single Sign-On](#configure-azure-ad-single-sign-on)** - to enable your users to use this feature.
2. **[Create an Azure AD test user](#create-an-azure-ad-test-user)** - to test Azure AD single sign-on with Britta Simon.
3. **[Create a SumTotalCentral test user](#create-a-sumtotalcentral-test-user)** - to have a counterpart of Britta Simon in SumTotalCentral that is linked to the Azure AD representation of user.
4. **[Assign the Azure AD test user](#assign-the-azure-ad-test-user)** - to enable Britta Simon to use Azure AD single sign-on.
5. **[Test single sign-on](#test-single-sign-on)** - to verify whether the configuration works.

### Configure Azure AD single sign-on

In this section, you enable Azure AD single sign-on in the Azure portal and configure single sign-on in your SumTotalCentral application.

**To configure Azure AD single sign-on with SumTotalCentral, perform the following steps:**

1. In the Azure portal, on the **SumTotalCentral** application integration page, click **Single sign-on**.

	![Configure single sign-on link][4]

2. On the **Single sign-on** dialog, select **Mode** as	**SAML-based Sign-on** to enable single sign-on.
 
	![Single sign-on dialog box](./media/sumtotalcentral-tutorial/tutorial_sumtotalcentral_samlbase.png)

3. On the **SumTotalCentral Domain and URLs** section, perform the following steps:

	![SumTotalCentral Domain and URLs single sign-on information](./media/sumtotalcentral-tutorial/tutorial_sumtotalcentral_url.png)

    a. In the **Sign-on URL** textbox, type a URL using the following pattern: `https://<subdomain>.sumtotalsystems.com/sites/default`

	b. In the **Identifier** textbox, type a value: `SumTotalFederationGateway`

	> [!NOTE] 
	> The Sign-on URL value is not real. Update the value with the actual Sign-On URL. Contact [SumTotalCentral Client support team](http://www.sumtotalsystems.com/support/) to get the value. 
 
4. On the **SAML Signing Certificate** section, click **Metadata XML** and then save the metadata file on your computer.

	![The Certificate download link](./media/sumtotalcentral-tutorial/tutorial_sumtotalcentral_certificate.png) 

5. Click **Save** button.

	![Configure Single Sign-On Save button](./media/sumtotalcentral-tutorial/tutorial_general_400.png)

6. To configure single sign-on on **SumTotalCentral** side, you need to send the downloaded **Metadata XML** to [SumTotalCentral support team](http://www.sumtotalsystems.com/support/). They set this setting to have the SAML SSO connection set properly on both sides.

> [!TIP]
> You can now read a concise version of these instructions inside the [Azure portal](https://portal.azure.com), while you are setting up the app!  After adding this app from the **Active Directory > Enterprise Applications** section, simply click the **Single Sign-On** tab and access the embedded documentation through the **Configuration** section at the bottom. You can read more about the embedded documentation feature here: [Azure AD embedded documentation]( https://go.microsoft.com/fwlink/?linkid=845985)
> 

### Create an Azure AD test user

The objective of this section is to create a test user in the Azure portal called Britta Simon.

   ![Create an Azure AD test user][100]

**To create a test user in Azure AD, perform the following steps:**

1. In the Azure portal, in the left pane, click the **Azure Active Directory** button.

    ![The Azure Active Directory button](./media/sumtotalcentral-tutorial/create_aaduser_01.png)

2. To display the list of users, go to **Users and groups**, and then click **All users**.

    ![The "Users and groups" and "All users" links](./media/sumtotalcentral-tutorial/create_aaduser_02.png)

3. To open the **User** dialog box, click **Add** at the top of the **All Users** dialog box.

    ![The Add button](./media/sumtotalcentral-tutorial/create_aaduser_03.png)

4. In the **User** dialog box, perform the following steps:

    ![The User dialog box](./media/sumtotalcentral-tutorial/create_aaduser_04.png)

    a. In the **Name** box, type **BrittaSimon**.

    b. In the **User name** box, type the email address of user Britta Simon.

    c. Select the **Show Password** check box, and then write down the value that's displayed in the **Password** box.

    d. Click **Create**.
 
### Create a SumTotalCentral test user

In this section, you create a user called Britta Simon in SumTotalCentral. Work with [SumTotalCentral support team](http://www.sumtotalsystems.com/support/) to add the users in the SumTotalCentral platform. Users must be created and activated before you use single sign-on.  

### Assign the Azure AD test user

In this section, you enable Britta Simon to use Azure single sign-on by granting access to SumTotalCentral.

![Assign the user role][200] 

**To assign Britta Simon to SumTotalCentral, perform the following steps:**

1. In the Azure portal, open the applications view, and then navigate to the directory view and go to **Enterprise applications** then click **All applications**.

	![Assign User][201] 

2. In the applications list, select **SumTotalCentral**.

	![The SumTotalCentral link in the Applications list](./media/sumtotalcentral-tutorial/tutorial_sumtotalcentral_app.png)  

3. In the menu on the left, click **Users and groups**.

	![The "Users and groups" link][202]

4. Click **Add** button. Then select **Users and groups** on **Add Assignment** dialog.

	![The Add Assignment pane][203]

5. On **Users and groups** dialog, select **Britta Simon** in the Users list.

6. Click **Select** button on **Users and groups** dialog.

7. Click **Assign** button on **Add Assignment** dialog.
	
### Test single sign-on

In this section, you test your Azure AD single sign-on configuration using the Access Panel.

When you click the SumTotalCentral tile in the Access Panel, you should get automatically signed-on to your SumTotalCentral application.
For more information about the Access Panel, see [Introduction to the Access Panel](../user-help/active-directory-saas-access-panel-introduction.md). 

## Additional resources

* [List of Tutorials on How to Integrate SaaS Apps with Azure Active Directory](tutorial-list.md)
* [What is application access and single sign-on with Azure Active Directory?](../manage-apps/what-is-single-sign-on.md)



<!--Image references-->

[1]: ./media/sumtotalcentral-tutorial/tutorial_general_01.png
[2]: ./media/sumtotalcentral-tutorial/tutorial_general_02.png
[3]: ./media/sumtotalcentral-tutorial/tutorial_general_03.png
[4]: ./media/sumtotalcentral-tutorial/tutorial_general_04.png

[100]: ./media/sumtotalcentral-tutorial/tutorial_general_100.png

[200]: ./media/sumtotalcentral-tutorial/tutorial_general_200.png
[201]: ./media/sumtotalcentral-tutorial/tutorial_general_201.png
[202]: ./media/sumtotalcentral-tutorial/tutorial_general_202.png
[203]: ./media/sumtotalcentral-tutorial/tutorial_general_203.png

