# Set-PnPTaxonomyFieldValue

## SYNOPSIS
Sets a taxonomy term value in a listitem field

## SYNTAX 

### ITEMS
```powershell
Set-PnPTaxonomyFieldValue -ListItem <ListItem>
                          -InternalFieldName <String>
                          [-Terms <Hashtable>]
```

### ITEM
```powershell
Set-PnPTaxonomyFieldValue -TermId <GuidPipeBind>
                          -ListItem <ListItem>
                          -InternalFieldName <String>
                          [-Label <String>]
```

### PATH
```powershell
Set-PnPTaxonomyFieldValue -TermPath <String>
                          -ListItem <ListItem>
                          -InternalFieldName <String>
```

## EXAMPLES

### ------------------EXAMPLE 1------------------
```powershell
PS:> Set-PnPTaxonomyFieldValue -ListItem $item -InternalFieldName 'Department' -TermId 863b832b-6818-4e6a-966d-2d3ee057931c
```

Sets the field called 'Department' to the value of the term with the ID specified

### ------------------EXAMPLE 2------------------
```powershell
PS:> Set-PnPTaxonomyFieldValue -ListItem $item -InternalFieldName 'Department' -TermPath 'CORPORATE|DEPARTMENTS|HR'
```

Sets the field called 'Department' to the term called HR which is located in the DEPARTMENTS termset, which in turn is located in the CORPORATE termgroup.

### ------------------EXAMPLE 3------------------
```powershell
PS:> Set-PnPTaxonomyFieldValue -ListItem $item -InternalFieldName 'Department' -Terms @{"TermId1"="Label1";"TermId2"="Label2"}
```

Sets the field called 'Department' with multiple terms by ID and label. You can refer to those terms with the {ID:label} token.

## PARAMETERS

### -InternalFieldName
The internal name of the field

```yaml
Type: String
Parameter Sets: (All)

Required: True
Position: Named
Accept pipeline input: False
```

### -Label
The Label value of the term

```yaml
Type: String
Parameter Sets: ITEM

Required: False
Position: Named
Accept pipeline input: False
```

### -ListItem
The list item to set the field value to

```yaml
Type: ListItem
Parameter Sets: (All)

Required: True
Position: Named
Accept pipeline input: False
```

### -TermId
The Id of the Term

```yaml
Type: GuidPipeBind
Parameter Sets: ITEM

Required: True
Position: Named
Accept pipeline input: False
```

### -TermPath
A path in the form of GROUPLABEL|TERMSETLABEL|TERMLABEL

```yaml
Type: String
Parameter Sets: PATH

Required: True
Position: Named
Accept pipeline input: False
```

### -Terms
Allows you to specify terms with key value pairs that can be referred to in the template by means of the {id:label} token. See examples on how to use this parameter.

```yaml
Type: Hashtable
Parameter Sets: ITEMS

Required: False
Position: Named
Accept pipeline input: False
```

# RELATED LINKS

[SharePoint Developer Patterns and Practices](http://aka.ms/sppnp)