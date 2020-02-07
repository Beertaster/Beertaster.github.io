---
layout: post
title:      "A review of Class methods and Instance Methods."
date:       2020-02-06 03:14:27 -0500
permalink:  a_review_of_class_methods_and_instance_methods
---

Draft 1

Methods are an organized form of functionality, able to be called and reused as needed. What separates Class and instance methods is whether it provides functionality to an induvidual instance of an object, or functionality to the class itself.

Class methods in ruby are denoted with a 'self.'. A class method should be used when the code being written does not apply to a single instance of an object. The class method below is used to clear a class variable named all. Because @@all is shared between instances of the class, it affects them all. 

def self.reset_all

      @@all.clear
			
end

As instance method only pertain to a single instance of an object, it allows for an induvidual customization of functionality. The instance method below will return the size of an array. For each instance of the (hypothetical) object the (hypothetical) array can be different sizes and contain different variables. If we want to know detailed information of the any specific array then an instance method should be used.

def list

    return "#{@array1.size} total"
		
end
		
The deciding factor in what type of method should be used is scope of functionality.
