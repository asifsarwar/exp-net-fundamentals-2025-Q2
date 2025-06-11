## Downloaded Azure Resource Template

After deploying my Microsoft Windows Server 2025 to Azure VM.
I downloaded the Resource Templates to be able to easily deploy again.

## Converting Resource Template to Azure Bicep

I launched the Windows Server that has UI.
I want to reuse my resource template files, but they are too hard to 
work with directly. So I am going to convert them to Azure Bicep.

```sh
cd ip-address-management/templates/vm
az bicep decompile --file template.json
```