# Start

## How to deploy the Solution in Azure

For more information visit this URL: https://learn.microsoft.com/en-us/training/modules/deploy-dotnet-aspire-app-azure/4-exercise-deploy-azure

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

We verify the deployment process 




