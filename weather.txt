print("Hello and welcome to the Hello weather system there will be reccomendations and other things regarding todays weather")
get_input = lambda prompt: input(prompt)
convert_to_float = lambda value: float(value) if value.replace(".", "", 1).isdigit() else None

user_input = input("Please enter the current temperature in degrees Farenheit: ")
temperature = float(user_input)
if temperature > 50:
    print("HOT")
    print("it's hot out")
    print("Wear light close to reduce the chance of sweating")
    print("and be cautious of mosquitos and bee stings.")
else:
    print("COLD")
    print("it is cold out wear a jacket.")
    print("wear heavy close to reduce the chance of a cold")
    print("remember to not stay out for so long")
wind_speed = convert_to_float(get_input("if you entered and got the answer cold or warm how is the mph for wind:"))
wind = float(wind_speed)
if wind > 15:
    print("it is quite windy out if it is cold weather then this is considered bad")
    print("be alert of the cold breeze as it can give you a fever.")
    print("Another thing would be alert for tornado sightings.")
else:
    print("that is not bad this could be actually safe for you")
    print("be sure to still wear the appropriate clothing as some things may change as the time goes by.")

humidity_data = convert_to_float(get_input("How is the humidity in your area in %:"))
humidity = float(humidity_data)
if humidity > 50:
    print("The humidity in your area is quite high stay hydrated.")
elif humidity < 30:
    print("The humidity is quite low be alert of your outdoor activities.")
else:
    print("your humidity levels are great!")
air_quality = convert_to_float(get_input("How is the air quality:"))
airquality = float(air_quality)
if airquality > 100:
    print("the air quality in your area is quite high and may affect sensitive groups.")
elif airquality < 100:
    print("the airquality in your area is alright and ok for all groups.")
if airquality < 50:
    print("the airquality is safe.")
UV_index = convert_to_float(get_input("in your area how is the UV-index:"))
UVindex = float(UV_index)
if UVindex > 8:
    print("The UV-index in your area is quite high wear sunscreen")
else:
    print("The UV-index in your area is ok and you should not get any sort of skin problems." )
pressure_data = convert_to_float(get_input("How is the pressure in your area:"))
pressure = float(pressure_data)
if pressure > 30:
    print("The pressure in your area is high be aware of headaches and take acetaminophen if your headache gets worse.")
else:
    print("The pressure in your area is ok and you have a low chance of getting a headache but still be aware.")
print("Thanks for giving me the input on your weather depending on how much info I provided please let me know how I did with this rating")
rating_stars = convert_to_float(get_input("From a rating 1 to 5 how would you like to rate your experiance:"))
rating = float(rating_stars)
if rating < 2:
    print(" thank you for your rating is there anything we can do to make the experiance better if so here is my contact hk0735@wayne.edu.")
else:
    print ("Thank you for the positive rating! If there is any reccomendations please reach out to my email hk0735@wayne.edu.")