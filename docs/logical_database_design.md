# Logical Database Design

## Strong Entities

### Client
- ClientID
- telephone
- email
- address
- dateJoined

#### Specialization:
- **Individuals**
  - ClientID
  - firstName
  - lastName
  - gender
- **GroupClient**
  - ClientID
  - groupName
  - groupDescription

### Training Session
- TrainingSessionID
- trainingDescription
- maximumCapacity
- duration

### Team
- TeamID
- teamName
- jobDescription
- teamCapacity

### Discount Package
- DiscountPackageID
- packageName
- percentageDiscount
- minimumHires

### License Category
- LicenseCategoryNo
- licenseCategory

### Insurance Type
- InsuranceTypeNo
- insuranceType

### Mode of Payment
- ModeOfPaymentNo
- paymentMode

### Working Availability
- WorkingAvailabilityID
- schedule

## Weak Entities

### Staff
- StaffID
- firstName
- lastName
- dateOfBirth
- gender
- telephone
- email
- address
- startDate
- salary
- TeamID

#### Specialization:
- **Manager**
  - StaffID
  - mgrStartDate
  - monthlyAllowance
  - dayOff
- **TeamLead**
  - StaffID
  - leadStartDate
  - dayOff
  - TeamID

### StaffTrainingSession
- STSessionID
- trainingDate
- startTime
- endTime
- numberOfAttendees
- TrainingSessionID
- Staff1ID
- Staff2ID

### Driver
- DriverID
- firstName
- lastName
- dateOfBirth
- gender
- telephone
- email
- address
- dateJoined
- licenseNumber
- licenseExpDate
- LicenseCategoryNo
- hasVehicle
- vehicleType
- vehicleNumberPlate
- yearsOfExperience
- WorkingAvailabilityID
- STSessionID

### DriverInsuranceType
- DITypeID
- InsuranceExpDate
- insuranceCompany
- InsuranceTypeID
- DriverID

### Hire Contract
- HireContractID
- startDate
- endDate
- signingDate
- termsConditions
- monthlyCost
- hireSpecifications
- driverMonthlyPay
- HirePaymentID
- totalCost
- amountPaid
- paymentDate
- ModeOfPaymentNo
- MonitoringStaffID
- LeasingStaffID
- ClientID
- DriverID

### applies
- HirePaymentID
- DiscountPackageID
- discountAmount

### isEntitledTo
- ClientID
- DiscountPackageID
