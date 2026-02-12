Runoff Voting System
Overview

This program implements a runoff (instant-runoff) election system, where voters rank candidates in order of preference. If no candidate receives a majority of the votes, the candidate(s) with the fewest votes are eliminated, and votes are redistributed according to voter preferences. This process continues until a winner is found or a tie occurs.

How It Works

Candidate names are provided as command-line arguments.

The program asks for the number of voters.

Each voter ranks all candidates from highest to lowest preference.

Votes are initially counted for each voter’s first choice.

If no candidate has more than 50% of the votes:

The candidate(s) with the lowest vote count are eliminated.

Votes are reassigned to the next preferred non-eliminated candidate.

The process repeats until:

A candidate wins with a majority, or

All remaining candidates are tied.

Program Features

Supports up to 100 voters

Supports up to 9 candidates

Handles ties correctly

Follows the official CS50 Runoff problem specification

Files

runoff.c — Contains the full implementation of the runoff voting algorithm.

Compilation

Compile the program using:

make runoff

Usage

Run the program by passing candidate names as arguments:

./runoff candidate1 candidate2 candidate3

Example
./runoff Alice Bob Charlie

Example Interaction
Number of voters: 3
Rank 1: Alice
Rank 2: Bob
Rank 3: Charlie

Alice

Notes

Votes are counted only for non-eliminated candidates.

The program continues running rounds until a clear winner or a tie is determined.

Input validation ensures only valid candidate names are accepted.

Author

This program was written as part of CS50 – Introduction to Computer Science.
