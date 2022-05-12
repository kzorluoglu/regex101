### Demo Dataset
| Phone Numbers |
| --- |
1234567890
123-456-7890
123 456 7890
(123) 456 7890
+49 123 456 7890
+49 123-456-7890

#### Get the Phone Number
`/\d+`

#### Create Groups based 3,3,4 Characters
`(\d{3})(\d{3})(\d{4})`

#### Get the number, which is also empty and minus between Charactes exists
`(\d{3})[ -]?(\d{3})[ -]?(\d{4})`

#### Get the number, which started with `(` `)` beging of number
`\(?(\d{3})\)?[ -]?(\d{3})[ -]?(\d{3})`

#### Get the number, which started with `country Code +`
`(\+\d{2})?[ ]?\(?(\d{3})\)?[ -]?(\d{3})[ -]?(\d{3})`

#### Give a name of every selected groups
`(?<countryCode>\+\d{2})?[ ]?\(?(?<areaCode>\d{3})\)?[ -]?(?<mainNumber>\d{3})[ -]?(?<mainNumber2>\d{3})`
