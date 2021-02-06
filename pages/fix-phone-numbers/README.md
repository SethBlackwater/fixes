## Fix Phone Numbers (EDITING, NOT FINISHED)
```
def fixPhoneNumber(number)
  number = number.to_i.delete("^0-9")
  if number.digits.count == 11 && number.digits[0] == 1
    newNumber = number.sub(/(\d{1})(\d{3})(\d{3})(\d{4})/, "+\\1 (\\2)-\\3-\\4")
  elsif number.digits.count == 12
    newNumber = number.sub(/(\d{3})(\d{2})(\d{3})(\d{2})(\d{2})/, "+\\1 \\2 \\3-\\4-\\5")
  elsif 
end
```
