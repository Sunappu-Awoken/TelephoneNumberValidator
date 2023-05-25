# TelephoneNumberValidator

The telephoneCheck function uses a regular expression pattern to match valid US phone numbers. The pattern (1\s?)? at the beginning allows for an optional country code of 1 followed by an optional whitespace character. The pattern (\(\d{3}\)|\d{3}) matches either three digits enclosed in parentheses or three digits without parentheses, representing the area code. The pattern [\s-]? allows for an optional whitespace character or hyphen. The pattern \d{3} matches three digits for the next part of the phone number, and [\s-]? allows for another optional whitespace character or hyphen. Finally, \d{4} matches the last four digits of the phone number.

The test method of the regular expression is used to check if the str matches the pattern. If it does, the function returns true; otherwise, it returns false.

You can test the function with the provided examples to see if they are identified as valid or invalid US phone numbers.
