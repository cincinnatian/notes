notes
=====

notes
def to_roman
	roman =""
	thousands = num/1000
	hundreds = num/100
	tens = num/10
	roman= roman + (num/1000)*"M"
	num = num%1000
	if num/100 == 9 
		roman = roman + "CM"
	else if num/100 == 4
		roman = roman + "CD"
	else if num/100 == 5
		roman = roman + "D"
	else if num/100 > 5
		roman = roman + "D" + ((num/100)-5)*"C")
	else if num/100 < 5
		roman = roman + (num/100)*"C")
	end
	num = num%100
	if num/10 == 9 
		roman = roman + "XC"
	else if num/10 == 4
		roman = roman + "XL"
	else if num/10 == 5
		roman = roman + "L"
	else if num/10 > 5
		roman = roman + "L" + ((num/10)-5)*"X")
	else if num/10 < 5
		roman = roman + ((num/10))*"X")
	end
	num = num%10
	if  == 9 
		roman = roman + "IX"
	else if num/10 == 4
		roman = roman + "IV"
	else if num/10 == 5
		roman = roman + "V"
	else if num/10 > 5
		roman = roman + "V" + ((num-5)*"I")
	else if num/10 < 5
		roman = roman + (num*"I")
	end
end

		
