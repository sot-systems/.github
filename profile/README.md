
# Table of Contents

1.  [SOT Systems](#org7b7df22)
2.  [Principles](#org544e17b)
    1.  [Dynamic](#orgeeee4a0)
    2.  [Incremental](#org59fd54d)
    3.  [Simple](#org47a3a9f)
    4.  [Orthogonal](#org3539a1b)
    5.  [Moldable](#org41504d4)
3.  [Synergies](#org7fac3a0)
    1.  [Dynamic and Incremental](#orgbaf905c)
    2.  [Simple and Orthogonal](#org1b7d2cc)
    3.  [Incremental and Moldable](#org3b668db)



<a id="org7b7df22"></a>

# SOT Systems

SOT Systems, named after [Ship of Theseus](https://en.wikipedia.org/wiki/Ship_of_Theseus), is a collection
of software systems that follow following core principles:


<a id="org544e17b"></a>

# Principles


<a id="orgeeee4a0"></a>

## Dynamic

Most characterstics of a software system end up being changed over time.

Some examples:

1.  Changing Data models and flows in the system, which might require
    backfills.
2.  New components, followed by an adoption phase.
3.  Component rewrites, followed by migration phase.
4.  Deployment topology
5.  Tech stack to different degrees
6.  Performance and uptime requirements
7.  Compliance requirements

Accomodating these changes is Priority #1.


<a id="org59fd54d"></a>

## Incremental

Many systems don't have upfront knowledge of requirements or
don't have the resource to design for all requirements.

Incremental integration, Incremental costs for additional capatilities
and being cheaply able to rollback the system without accumulating
cruft is Priority #2.


<a id="org47a3a9f"></a>

## Simple

Making our system simple to use correctly is Priority #3.

This would mean adopting various ideas for reducing complexity
and incorrect usage:

1.  Declarative v/s imperative.
2.  Linting/static checkers.
3.  Avoid surprises at runtime.
4.  Ideas in literature like: Our of the tar pit, A philosophy of
    software design.
5.  Restrictive wrappers.


<a id="org3539a1b"></a>

## Orthogonal

Typically, some characterstics of a software system are more
intricately linked than they need to be. Some of those chactersitics
are:

1.  Scaling/Performance
2.  Deployment topology
3.  Persistence
4.  Implementation
5.  Observability
6.  Reliability
7.  Security
8.  Interface

Making these characterics as orthogonal as possible is Priority #4.


<a id="org41504d4"></a>

## Moldable

Typically, software systems require plumbing before they can be integrated
into an existinting system.

Sometimes, use case evolves so much that new capabilities must
be added to external software system.

Accomodating these plumbings and extensions is priority #5.


<a id="org7fac3a0"></a>

# Synergies


<a id="orgbaf905c"></a>

## Dynamic and Incremental

By prioritizing both the ability to accommodate changes and the
incremental integration of new capabilities, SOT Systems can evolve
smoothly over time without incurring significant costs or accumulating
technical debt.


<a id="org1b7d2cc"></a>

## Simple and Orthogonal

Striving for simplicity and orthogonality in system characteristics
leads to a more maintainable and understandable codebase, reducing the
likelihood of errors and making it easier for developers to work with
the system.


<a id="org3b668db"></a>

## Incremental and Moldable

The combination of incremental development and the ability to mold the
system to fit existing infrastructure and evolving use cases allows
SOT Systems to be easily integrated and adapted to changing
requirements.

