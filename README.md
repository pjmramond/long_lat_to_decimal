# long_lat_to_decimal
Convert Latitude and Longitude written in degree-min-sec to decimal

This is a modified version of the function developped by A. Marcia Barbosa (https://modtools.wordpress.com/) and PaulMelloy.
The original version can be found here: https://github.com/AMBarbosa/unpackaged/blob/master/dms2dec

In this version, Commas "," were added as a seprator.

All credits goes to the original authors.

Use as follow:

```
# import function
source("https://raw.githubusercontent.com/pjmramond/long_lat_to_decimal/main/dms2dec2")

# generate example data
data<-data.frame(Latitude = c("9°2,419S","9°2,419S" ,"9°29,929S" ,"9°29,929S", "9°43,552S", "9°43,552S", "10°1,492S"),
Longitude = c("139°39,846W", "139°39,846W", "138°57,937W", "138°57,937W", "139°10,824W", "139°10,824W", "139°24,097w"))

dms2dec(data$Latitude)
dms2dec(data$Longitude)
```

