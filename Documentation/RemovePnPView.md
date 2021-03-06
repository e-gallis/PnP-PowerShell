# Remove-PnPView

## SYNOPSIS
Deletes a view from a list

## SYNTAX 

```powershell
Remove-PnPView -Identity <ViewPipeBind>
               -List <ListPipeBind>
               [-Force [<SwitchParameter>]]
               [-Web <WebPipeBind>]
```

## EXAMPLES

### ------------------EXAMPLE 1------------------
```powershell
PS:> Remove-PnPView -List "Demo List" -Identity "All Items"
```

Removes the view with title "All Items" from the "Demo List" list.

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

### -Identity
The ID or Title of the view.

```yaml
Type: ViewPipeBind
Parameter Sets: (All)

Required: True
Position: 0
Accept pipeline input: True
```

### -List
The ID or Url of the list.

```yaml
Type: ListPipeBind
Parameter Sets: (All)

Required: True
Position: 1
Accept pipeline input: True
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