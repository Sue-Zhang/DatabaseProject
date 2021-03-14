# Database
1. Background

The local state government wishes to develop a database to record the details of
"on-the-spot" traffic offences incurred by drivers. When a driver commits an offence they
are stopped and booked "on the spot" by a police officer and provided with an offence
notice. Offences cause drivers to incur demerit points which accumulate against the
drivers' licence.

The system records the details of all registered vehicles driven in the local government
area. A vehicle is identified by a Vehicle Identification Number (VIN). Background reading
on a VIN is available from several sites such as AutoCheck. Other attributes recorded for a
vehicle are the vehicle's year of manufacture, main colour, model name, manufacturer
name and vehicle type.

Drivers are identified by their licence number. Other attributes recorded for a driver are the
driver's mobile number, first name, last name, residential address, date of birth and expiry
date for the licence. It is assumed for this task that each driver has a mobile number and
that number will be unique.

Each demerit (potential driving offence) is identified by a demerit code. A description of the
demerit and the number of points incurred for that demerit are also recorded. For example,
the demerit with code 108, has a description of "Failing to give way, or stop, or remain
stopped" and results in 3 demerit points being incurred by the driver.
Each traffic offence by a driver is identified by an offence number. The location of the
offence and the date and time at which the offence occurred is also stored. In some
circumstances when a driver is stopped by a police officer, for example, a speeding
offence, the police officer may also identify other offences such as "Driving contrary to a
major defect notice". Each offence recorded has a unique offence number and is for only
one particular demerit. The police officer who issued the offence is also recorded.

Once a driver has accumulated 12 demerit points over a period of three years the driver’s
licence is suspended for a period of 6 months. When an offence committed by a driver is
added to the system by the police officer, the system at that time will determine
automatically if the licence should be suspended or not. When this occurs the driver’s
licence is suspended from the date recorded for the offence which caused the points to
equal or exceed the permitted maximum points. The date at which the suspension began
and the date at which it ends are to be stored in the system. The driver, if suspended, is
not allowed to drive and driving while suspended will lead to a criminal charge and may
cause the driver to be jailed.
After a driver’s suspension ends, their total demerit points are reset to zero and they begin
accumulating points again. For any previously suspended driver, to determine the new
suspension date, the system will calculate the accumulated demerit points from the date
their last suspension ended.

Police officers are identified by an officer id. The system only records the officer's first
name and last name.

2. A data model has been created for Traffic Demerit System and is shown below:

![image](https://user-images.githubusercontent.com/79569693/109511620-2f4f8100-7ade-11eb-817a-60a37bc97e8d.png)
