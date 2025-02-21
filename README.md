# Ruby Instance Variable Immutability Through Accessor Method

This example demonstrates an uncommon error in Ruby where attempting to modify an instance variable through its accessor method doesn't change its value. This is because the accessor method only provides read access unless explicitly defined as a writer.

## Bug Report

The `bug.rb` file shows that assigning a new value to the `value` instance variable through the accessor (`my_object.value = 20`) doesn't update the internal state of the object. The output remains 10.

## Solution

The `bugSolution.rb` file provides a corrected version. It introduces a `value=` method to allow for modifying the instance variable.

## Setup

No special setup is required. Simply run the ruby files.