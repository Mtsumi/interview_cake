# HiCal Meeting Scheduler

A Python solution to the [HiCal Meeting Scheduler problem](https://www.interviewcake.com/question/python3/meeting-merger) from Interview Cake.

## Problem Description

Given a list of meeting times represented as tuples of integers `(start_time, end_time)`, where each integer represents the number of 30-minute blocks past 9:00am, write a function `merge_ranges` that returns a condensed list of meeting times. If two meetings overlap or are adjacent, they should be merged into one block of time. The function should be able to handle large numbers representing time ranges, such as Unix timestamps.

For example, given the list `[(0, 1), (3, 5), (4, 8), (10, 12), (9, 10)]`, the function should return `[(0, 1), (3, 8), (9, 12)]`.

## Solution

The solution involves sorting the list of meetings by start time, then iterating through the sorted list and merging any meetings that overlap or are adjacent. The resulting list of merged meetings is returned.

See the `hical.py` file for the Python implementation of the solution.

## Usage

1. Clone this repository to your local machine using `git clone https://github.com/Mtsumi/interview_cake.git`.
2. Navigate to the project directory in your terminal.
3. Run `python3 hical_scheduler.py` or `./hical_scheduler.py`to execute the program and see the results of the provided test cases.
4. To use the program with your own list of meetings, modify the `meetings` list within the `merge_ranges()` function with your own meeting times in the format `(start_time, end_time)`.
5. Run the program using `python3 hical_scheduler.py` to see the merged meetings.

## Tests

This program includes a suite of tests to ensure proper functionality. To run the test suite, simply execute `python3 hical.py`. Each test case will output either `ok` if the test passes, or an error message if the test fails.

## Contributing

Contributions are always welcome! If you find any bugs or would like to suggest additional features, please create an issue or submit a pull request.
