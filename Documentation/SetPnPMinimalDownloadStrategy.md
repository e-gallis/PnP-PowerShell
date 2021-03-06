# Set-PnPMinimalDownloadStrategy

## SYNOPSIS
Activates or deactivates the minimal downloading strategy.

## SYNTAX 

### On
```powershell
Set-PnPMinimalDownloadStrategy -On [<SwitchParameter>]
                               [-Force [<SwitchParameter>]]
                               [-Web <WebPipeBind>]
```

### Off
```powershell
Set-PnPMinimalDownloadStrategy -Off [<SwitchParameter>]
                               [-Force [<SwitchParameter>]]
                               [-Web <WebPipeBind>]
```

## DESCRIPTION
Activates or deactivates the minimal download strategy feature of a site

## EXAMPLES

### ------------------EXAMPLE 1------------------
```powershell
PS:> Set-PnPMinimalDownloadStrategy -Off
```

Will deactivate minimal download strategy (MDS) for the current web.

### ------------------EXAMPLE 2------------------
```powershell
PS:> Set-PnPMinimalDownloadStrategy -On
```

Will activate minimal download strategy (MDS) for the current web.

## PARAMETERS

### -Force
Specifying the Force parameter will skip the confirmation question.

```yaml
Type: SwitchParameter
Parameter Sets: (All)

Required: False
Position: Named
Accept pipeline input: False
```

### -Off
Turn minimal download strategy off

```yaml
Type: SwitchParameter
Parameter Sets: Off

Required: True
Position: Named
Accept pipeline input: False
```

### -On
Turn minimal download strategy on

```yaml
Type: SwitchParameter
Parameter Sets: On

Required: True
Position: Named
Accept pipeline input: False
```

### -Web
The GUID, server relative url (i.e. /sites/team1) or web instance of the web to apply the command to. Omit this parameter to use the current web.

```yaml
Type: WebPipeBind
Parameter Sets: (All)

Required: False
Position: Named
Accept pipeline input: False
```

# RELATED LINKS

[SharePoint Developer Patterns and Practices](http://aka.ms/sppnp)