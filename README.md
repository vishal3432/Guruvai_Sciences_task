# Guruvai_Sciences_task
In this repository, I am going to complete the task which is being assigned by the Guruvai Sciences .
LRU Cache & Event Scheduler
This repository contains implementations of two classic backend system design problems:
LRU Cache – Efficient caching mechanism with constant time operations.
Event Scheduler – Utilities for detecting event conflicts and calculating the minimum number of meeting rooms required.
These problems demonstrate knowledge of data structures, algorithm optimization, and backend system design patterns.

# Problem 1: LRU Cache
## Description
The Least Recently Used (LRU) Cache stores key-value pairs with a fixed capacity. When the cache reaches its limit, it automatically removes the least recently used item before inserting a new one.

Supported Operations
1.get(key)
Returns the value associated with the key.
Returns -1 if the key does not exist.
Marks the key as recently used.

2.put(key, value)
Inserts or updates a key-value pair.
If the cache exceeds capacity, the least recently used item is gone.

### Approach
The implementation combines two data structures:

## 1.Hash Map
Provides fast lookup of keys in O(1) time.

## 2.Doubly Linked List
Maintains the order of recently used items.
The most recently used item is placed at the front.
The least recently used item is removed from the tail when capacity is exceeded.

## This combination allows both operations to run in constant time.
# Problem 2: Event Scheduler

The scheduler processes a list of events represented as:
(start_time, end_time)
Adjacent events where the end time equals the next start time do not overlap.

# 1. can_attend_all(events)
## Purpose
Determines whether a person can attend all events without schedule conflicts.
Time Complexity -	O(n log n)
Space Complexity - O(1)
# 2. min_rooms_required(events)
## Purpose
Determines the minimum number of meeting rooms required so that all events can occur without conflict.
Time Complexity - O(n log n)
Space Complexity -	O(n)


