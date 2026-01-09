# Week 6 – Unit Testing and Test Doubles 

## Overview
This repository contains the Week 6 lab work for the 2CWK70 Software Testing and Quality Assurance module.
The focus of this week is the implementation of automated unit tests using test doubles.

## System Under Test (SUT)
The System Under Test is the `PostManager` class, which is responsible for:
- Scheduling posts for future publication
- Publishing posts immediately
- Cancelling scheduled posts
- Logging system events

The class depends on external components:
- DateTimeProvider
- PlatformService
- Logger

These dependencies are replaced with test doubles to enable isolated and deterministic testing.

## Test Doubles Used
- **Dummy**: `DummyLogger` – satisfies the dependency without behaviour
- **Stub**: `StubDateTimeProvider` – returns a fixed date/time
- **Spy**: `SpyLogger` – captures log messages
- **Spy**: `SpyPlatformService` – records platform interactions

## Testing Framework
- JUnit 5
- Tests follow the Arrange–Act–Assert (AAA) pattern

## How to Run Tests
1. Open the project in IntelliJ IDEA
2. Navigate to `PostManagerTest.java`
3. Right-click and select **Run 'PostManagerTest'**
4. All tests should pass successfully

## Evidence
Screenshots showing successful test execution are included in the final assignment report.

