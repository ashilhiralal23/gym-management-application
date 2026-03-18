# gym-management-application
Integrated project showcasing a gym management application with  process design/system documentation.Between user and system

START
  ↓
Start Registration Process
  ↓
Enter User Information
  ↓
[Decision] Is the information valid?
  ├── No → Display Error Message / Re-enter Information
  └── Yes → Create New Profile
                ↓
         Send Account Registration Confirmation
                ↓
         Select Package Type
                ↓
         Make Payment for Package
                ↓
       [Decision] Was payment successful?
          ├── No → Display Payment Failed Message / Retry Payment
          └── Yes → Send Payment Approval Message
                        ↓
              [Decision] Would the user like to book a class?
                ├── Yes → Select Class Type
                │          ↓
                │   Make Payment for Class
                │          ↓
                │   [Decision] Was class payment successful?
                │       ├── No → Display Payment Failed Message / Retry Payment
                │       └── Yes → Send Class Booking Confirmation
                │                     ↓
                │              Receive Confirmation
                │
                └── No
                        ↓
              [Decision] Would the user like to buy supplements?
                ├── Yes → Select Desired Products
                │          ↓
                │   Make Payment for Products
                │          ↓
                │   [Decision] Was product payment successful?
                │       ├── No → Display Payment Failed Message / Retry Payment
                │       └── Yes → Send Purchase Confirmation
                │                     ↓
                │              Receive Confirmation
                │
                └── No
                        ↓
                       END
