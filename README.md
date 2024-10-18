# How to create eShop application step by step

## 1. Prerequisites

Visual Studio 2022 Community Edition

.NET 9

.NET Aspire worload

Docker Desktop



## 2. Create a Blazor Web App 

## 3. Create a .NET Web API


## 4. Consuming API from the Blazor Web App

## 5. Adding Aspire Host project

## 6. Adding the Aspire ServiceDefault project

## 7. Adding the Orchestration Support in the projects

## 8. Adding the Migration Manager project (Catalog.Data.Manager.csproj)




## 9. How to deploy the Solution in Azure

For more information visit this URL: 

https://learn.microsoft.com/en-us/training/modules/deploy-dotnet-aspire-app-azure/4-exercise-deploy-azure

Navigate to the Host project and open in a command prompt and run the command **azd init**

```
C:\14. Blazor LCE Youtube channel\mslearn-aspire-starter\Start\eShop.AppHost>azd init
```

Follow the steps highlighted in red. Select the **resource group name** where to deploy in Azure 

![image](https://github.com/user-attachments/assets/e8c07efc-6f20-4cb1-b125-17f68640f4c4)

We verify the following files **azure.yaml** and **next-steps** and folder **.azure**

![image](https://github.com/user-attachments/assets/8c9a92e4-b382-4849-843b-86a044ea5b1c)

After run the command **azd up**

```
C:\14. Blazor LCE Youtube channel\mslearn-aspire-starter\Start\eShop.AppHost>azd up
```

or 

```
azd provision
```

and 

```
azd deploy
```

After running **azd up**, we verify the deployment process. We have to select the **Azure Subscription** and the deployment **Region**

![image](https://github.com/user-attachments/assets/450f3e97-b134-4e76-b421-cdb4ea3c1602)

When the deployment is finished we can navigate to the **Dashboard** web page

![image](https://github.com/user-attachments/assets/915d243e-4ab9-4075-a133-c42e7df56037)

We can restart the **catalog-db-mgr** if appears an issue pressing the three dots **...** and then in the **Restart catalog-db-mgr**

![image](https://github.com/user-attachments/assets/baa21026-4279-4a93-851d-bf26df3fcb6c)

Now we navigate inside the deployment resource group **rg-eshop_deployment**

![image](https://github.com/user-attachments/assets/b06c3b6a-dc4a-4136-adcf-404e82497465)

![image](https://github.com/user-attachments/assets/eb1015c5-3d77-4776-92aa-54a161b123e5)

![image](https://github.com/user-attachments/assets/743d674f-1e73-43f6-9ad8-b8a86bda1c18)

We have to grant permission to the **weapp** for accepting the ingress traffic

![image](https://github.com/user-attachments/assets/61fefff2-7cc6-4e36-906f-f398f324bec2)

We select **Settings** and **Ingress** and select the option **Accept Traffic from Anywhere** and press the **Save** button

![image](https://github.com/user-attachments/assets/b60f05a8-7412-4937-b20d-d02e69af77c6)

![image](https://github.com/user-attachments/assets/1a549256-d98c-4ad3-9181-dec18f767d02)

We finally verify the web applicattion is running properly

![image](https://github.com/user-attachments/assets/541def2a-34e8-414c-8f66-cfc81e21c07e)

![image](https://github.com/user-attachments/assets/64bb1e64-a840-4138-aa71-8cbc1e6a12c5)




