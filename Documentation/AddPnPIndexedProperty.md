# Add-PnPIndexedProperty

## SYNOPSIS
Marks the value of the propertybag key specified to be indexed by search.

## SYNTAX 

```powershell
Add-PnPIndexedProperty -Key <String>
                       [-Web <WebPipeBind>]
```

## PARAMETERS

### -Key
Key of the property bag value to be indexed

```yaml
Type: String
Parameter Sets: (All)

Required: True
Position: 0
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