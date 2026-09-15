`http_request for adding new booking`

url: localhost:8000/bookings/    

method: post  

body: {  
    "guest_name": "thushara",   
    "room_number": "101",  
    "room_type": "single",  
    "check_in_date": "2026-09-15",  
    "check_out_date": "2026-09-17",  
    "status": "Reserved",  
    "total_amount": 3000.00  
}

`http_request for list all bookings`

url: localhost:8000/bookings/

method: get

`http_request for fetching booking detail`

url: localhost:8000/bookings/5/

method: get

`http_request for update booking`

url: localhost:8000/bookings/5/

method: put

body: {  
    "guest_name": "vishnu",  
    "room_number": "301",  
    "room_type": "deluxe",  
    "check_in_date": "2026-09-20",  
    "check_out_date": "2026-09-23",  
    "status": "Checked-in",  
    "total_amount": 8000.00  
}  

`http_request for delete booking`

url: localhost:8000/bookings/5/

method: delete

## /bookings/

class BookingListCreateView:

    def get(self, request)
    def post(self, request)


## /bookings/{pk}/

class BookingRetrieveUpdateDeleteView:

    def get(self, request, id)
    def put(self, request, id)
    def delete(self, request, id)


## model – Booking

booking_id  
guest_name  
room_number  
room_type  
check_in_date  
check_out_date  
status  
total_amount  
created_at  


# apps

hotel_app