# Complicated proto are

```

syntax = "proto3";

// Define an enum representing the type of phone numbers:

enum PhoneType {
  MOBILE = 0;
  HOME = 1;
  WORK = 2;
}

// Define a message type representing a phone number:

message PhoneNumber {
  string number = 1;
  PhoneType type = 2;
}

// Define a message type representing an address:

message Address {
  string street = 1;
  string city = 2;
  string state = 3;
  string zip = 4;
}

// Define a message type representing a person:

message Person {
  string name = 1;
  int32 age = 2;
  repeated PhoneNumber phone_numbers = 3;
  Address address = 4;
}

```
