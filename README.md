PnP Powershell Documentation: https://pnp.github.io/powershell/cmdlets/Add-PnPAlert.html

"Save Site as Template" Tutorial https://spgeeks.devoworx.com/missing-save-site-as-template-sharepoint-online/#whats-the-save-site-as-template-in-sharepoint

Change PnP Management Shell Permissions at https://myapps.microsoft.com


<h1>CMDLETS</h1>

- Login to Sharepoint: Connect-PnPOnline -Url "sharepoint site url" -Interactive

- Check current context: Get-PnPConnection

- Get Site Template: Get-PnPSiteTemplate -Out "file path"  
e.g. Get-PnPSiteTemplate -Out "C:\Users\artc\Desktop\template.pnp"

- Create new (classic) site: New-PnPTenantSite  
e.g. New-PnPTenantSite -Title arthurclient_SG -Url "https://xxx.sharepoint.com/sites/arthurclient_SG" -Owner arthur.chionh@xxx.com -TimeZone 21 -Template STS#3

  - Get timezone IDs: Get-PnPTimeZoneId  
  e.g. 21 = Singapore UTC +8

  - Get available classic web templates: Get-PnPWebTemplates
  e.g. STS#3 = Team Site (no Microsoft 365 group)
