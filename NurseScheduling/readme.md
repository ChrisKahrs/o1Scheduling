# Nurse Scheduling Problem

The nurse scheduling problem involves assigning shifts to nurses in a way that meets various constraints and requirements. Here is a classical formulation of the problem below.  Notice in the output the model cannot satisfy one of the constraints but it does a good job of balancing the workload among the nurses as evenly as possible and lets you know what it is not able to meet.  Humans can then reprompt or adjust the constraints to get a better solution.

## Problem Description

You are tasked with creating a schedule for a set of nurses over a given period (e.g., one week). The schedule must satisfy the following constraints:

### Constraints

1. **Shift Coverage**: Each shift must be covered by a minimum number of nurses.
2. **Maximum Shifts**: Each nurse can work a maximum number of shifts per week.
3. **Minimum Rest**: Each nurse must have a minimum number of hours of rest between consecutive shifts.
4. **Shift Preferences**: Nurses may have preferences for certain shifts, which should be taken into account if possible.
5. **Weekend Shifts**: Each nurse should work a limited number of weekend shifts.
6. **Consecutive Shifts**: Nurses should not work more than a specified number of consecutive shifts.

### Example Data

- **Nurses**: {Nurse1, Nurse2, Nurse3, Nurse4, Nurse5}
- **Shifts**: {Morning, Afternoon, Night}
- **Days**: {Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday}

### Objective

The objective is to create a schedule that satisfies all the constraints while balancing the workload among the nurses as evenly as possible.

## Input Format

- List of nurses
- List of shifts
- List of days
- Minimum number of nurses required per shift
- Maximum number of shifts per nurse per week
- Minimum rest hours between shifts
- Nurse shift preferences
- Maximum number of weekend shifts per nurse
- Maximum number of consecutive shifts per nurse

## Output Format

A schedule indicating which nurse is assigned to which shift on each day.

## Example

| Day       | Morning Shift | Afternoon Shift | Night Shift |
|-----------|---------------|-----------------|-------------|
| Monday    | Nurse1        | Nurse2          | Nurse3      |
| Tuesday   | Nurse4        | Nurse5          | Nurse1      |
| Wednesday | Nurse2        | Nurse3          | Nurse4      |
| Thursday  | Nurse5        | Nurse1          | Nurse2      |
| Friday    | Nurse3        | Nurse4          | Nurse5      |
| Saturday  | Nurse1        | Nurse2          | Nurse3      |
| Sunday    | Nurse4        | Nurse5          | Nurse1      |

Use this prompt to run the o1 model and generate a nurse schedule that meets the specified constraints.

## Runs
create a table of runs here
| Input File          | Output File          | Token Count | Run Time  | Run Date    | Description |
|---------------------|----------------------|-------------|-----------|-------------|-------------|
|prompt20241107_1.md  |output20241107_1.md   |  460        |  1.2s     | 2024-11-07  |             |


