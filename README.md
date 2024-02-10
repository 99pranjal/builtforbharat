# builtforbharat
The provided code is a C++ program that demonstrates a simple implementation of a merchant service. The program allows merchants to register their serviceable pincodes and checks if a given pincode is serviceable by a specific merchant.

**Merchant Class**
The Merchant class represents a merchant and contains a set of serviceable pincodes. The class has two constructors: a default constructor and a constructor that takes a vector of pincodes as input. The constructor with the vector of pincodes initializes the serviceablePincodes set by inserting the pincodes from the vector.

The isServiceable function checks if a given pincode is present in the serviceablePincodes set. It returns true if the pincode is serviceable by the merchant, and false otherwise.

**MerchantService Class*
The MerchantService class manages a collection of merchants using an unordered map. Each merchant is associated with a unique merchant ID. The addMerchant function allows merchants to be added to the merchants map by providing their merchant ID and a vector of serviceable pincodes.

The isPincodeServiceable function checks if a given pincode is serviceable by a specific merchant. It first searches for the merchant in the merchants map using the provided merchant ID. If the merchant is found, it calls the isServiceable function of the corresponding Merchant object to check if the pincode is serviceable. If the merchant is not found, it returns false.

**Main Function**
The main function demonstrates the usage of the MerchantService class. It creates an instance of MerchantService and adds two merchants with their respective serviceable pincodes. Then, it tests the isPincodeServiceable function by checking if a specific pincode is serviceable by a specific merchant. The result is printed to the console.

In the provided code, the pincode 1002 is checked for serviceability by merchant 1. If the pincode is serviceable, the program outputs "Pincode 1002 is serviceable by Merchant 1". Otherwise, it outputs "Pincode 1002 is not serviceable by Merchant 1".
