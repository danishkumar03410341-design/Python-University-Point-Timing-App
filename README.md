schedule = {
    "City Gate": {
        "Morning": "7:30 AM",
        "Return": "2:30 PM"
    },
    "Naseem Nagar": {
        "Morning": "7:00 AM",
        "Return": "3:00 PM"
    },
    "Ali Plus": {
        "Morning": "8:00 AM",
        "Return": "4:00 PM"
    } 
}

print("------ University Point Timing App ------")

area_input = input("Enter your area: ").strip().title()  
# strip() extra spaces remove karta hai
# title() first letter capital kar deta hai taake dictionary key match ho

if area_input in schedule:
    print("Morning Time:", schedule[area_input]["Morning"])
    print("Return Time:", schedule[area_input]["Return"])
else:
    print("Sorry, area not found.")
