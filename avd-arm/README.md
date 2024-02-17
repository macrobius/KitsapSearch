New-AzResourceGroup  -Name "storage-resource-group" -Location "westus"

New-AzResourceGroupDeployment -name "storage-account-deployment" -ResourceGroupName "storage-resource-group" -TemplateFile ".\azuredeploy.json" -TemplateParameterFile .\azuredeploy.parameters.json