# Remove-PnPIndexedProperty

## SYNOPSIS
Removes a key from propertybag to be indexed by search. The key and it's value remain in the propertybag, however it will not be indexed anymore.

## SYNTAX 

```powershell
Remove-PnPIndexedProperty -Key <String>
                          [-Web <WebPipeBind>]
```

## PARAMETERS

### -Key
Key of the property bag value to be removed from indexing

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