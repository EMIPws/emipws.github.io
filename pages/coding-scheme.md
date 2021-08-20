---
layout: single
permalink: /coding-scheme/
header:
title: "Coding Scheme"
sidebar:
  nav: "main"
---

[Coding Scheme](#coding-scheme)

[Source code used for the scheme](#source-code-used-for-the-scheme)

# Coding Scheme

Revised after the workshop (version of February 15th, 2014)

| Category | Codes | Description | Classification |
|---|---|---|---|
| Line | Line1, Line 2 … | Line on which fixation occurs | Observable |
| Block | Attributes, Area, Constructor, Height, Main, Width | General area in which fixation occurs, e.g. a main-method, the height-method etc. | Observable |
| SubBlock | Body, Return, Signature | Specific region of the general area in which fixation occurs, the signature, the line containing the return statement or the body | Observable |
| Signature | FormalParameter- List, Name, Type, Visibility | Precise code section | Observable |
| FormalPara-meterList | x1, x2, y1, y2 | Precise code section | Observable |
| MethodCall | ActualParameterList, Name, PrintLine | Precise code section | Observable |
| Pattern | Flicking, JumpControl, JustPassingThrough, LinearHorizontal, LinearVertical, RetraceDeclaration, RetraceReference, Scan, Signatures, Thrashing, Word(Pattern)- Matching | Flicking: The gaze moves back and forth between two related items, such as the formal and actual parameter lists of a method call. JumpControl: Subject jumps to the next line according to execution order. JustPassingThrough: Fixations are on a blank spot and clearly just stops on the way to some place else. LinearHorizontal: Subject reads a whole line either from from left to right or right to left, all elements in rather equally distributed time. LinearVertical: Subject follows text line by line, for at least three lines, no matter of program flow, no distinction between signature and body. RetraceDeclaration: Often-recurring jumps between places where variable is used and where it had been declared (Uwano et al. 2006). Form of Flicking. RetraceReference: Often-recurring jumps between places where variable is used and where it had been recently referred to (Uwano et al. 2006). Form of Flicking. Scan: Subject first reads all lines of the code from top to the bottom briefly. (Uwano et al. 2006 found that in the first 30 % of the review time a preliminary reading of the whole program occurs.) Signatures: Subject looks at all signatures first, before looking into method/ constructor body.Thrashing: The gaze moves rapidly and wildly in a sequence that appears to make no particular sense. Word(Pattern)Matching: Simple visual pattern matching. | Observable |
| Strategy | AttentionToDetail, DataFlow, Debugging, Deductive, DesignAtOnce, FlowCycle, Inductive, Interprocedural- ControlFlow, Intraprocedural- ControlFlow, StrayGlance, TestHypothesis, Touchstone, Trial&Error, Wandering | AttentionToDetail: Similar to Debugging, however with a different intention. Readers are trying to comprehend a piece of code that is not believed to contain bugs. In most cases, there is a slowness to AttentionToDetail, but the subject could also be verifying a global property, such as that argument/ parameter types agree or that the semi-colons are present in the right places. DataFlow: Following a single object in memory as its value changes through the program. Can also occur backwards through control flow in service of debugging and/or program execution comprehension. Debugging: Similar to DesignAtOnce, but more equally distributed fixation durations, and more equally distributed time of fixation for all text elements. Based on pattern  LinearHorizontal and LinearVertical. The subject’s intention is to find syntactical or semantic errors. Very small jumps, where the subject is presumably validating the syntax. (Note: Maybe debugging is more a goal, than a strategy. See AttentionToDetail.) Deductive: From general to special, from definition to use, typically includes LinearHorizontal. DesignAtOnce: LinearHorizontal or Scan, hardly any jumps back. The subject’s intention is to understand the general or the algorithmic idea, without having the need to go into details. Aiming at understanding by linear reading of the complete (needed) code. Can easily be confused with excessive demand/trial and error, might also include TestHypothesis on local levels. Captures high-level algorithmic thinking, thus, features rather large steps as the gaze sweeps over the text typically associated with Linear and Scan patterns. Suggests reading through part or all of the code in a linear manner, intending to acquire an overall understanding of it. FlowCycle: The same program flow sequence might be followed several times, the intent might be to gain a first understanding of the flow, strengthening and reinforcing it with repeated examinations of the same code. The Flicking pattern might then suggest the simplest level of the FlowCycle strategy. Inductive: From the special to general, from context to definition, typically combined strategy (mix of Scan, JumpControl and LinearHorizontal). InterproceduralControlFlow: The subject follows call-chains in real or simulated sequence of control flow. Intention is to understand the execution or to get the outcome of a code section. Focus is on execution between blocks. IntraproceduralControlFlow: The subject scans lines of code in real or simulated program execution order. Intention is to understand the execution or to get the outcome of a code section. Focus is on execution on block level. StrayGlance: A glance where something is looked at that does not necessarily involve comprehension or something that we cannot explain. TestHypothesis: Repetition of a pattern or gaze path. Occurs in connection with DesignAtOnce or ControlFlow. The subject’s intention is to check for some details in understanding. Hints at some issue where either the person was distracted, or which is more difficult to comprehend. Involves repetition of a pattern of gaze, and suggests further concentration in order to better understand a particular detail. Touchstone: Analogue to checking the risk of any deal. Before transporting some goods through an unknown route, first you go there without merchandise and see, where to turn and where the traffic lights are. And when you are sure about everything, you take the goods with you to finish the deal. Comparing this example with program comprehension, the route is the algorithm, while the goods are the parameters. Trial&Error: Similar to DesignAtOnce, but with higher reading speed, and some irregular jumps and repetitions in reading. The subject’s intention is to cope with cognitive overload and to try to find some place to start the understanding process. Connected to JustPassingThrough and Wandering. Wandering: It appears that the subject was backtracking, seemingly searching for a point to resume the reading after a particular path of reasoning had been exhausted, essentially a transition period or a brief rest between bursts of effort. | Interpretation |

# Source Code used for the Scheme
```java
public class Rectangle {
    private int x1 , y1 , x2 , y2 ;
    public Rectangle ( int x1 , int y1 , int x2 , int y2 ) { 
        this.x1 = x1 ;
        this.y1 = y1 ;
        this.x2 = x2 ;
        this.y2 = y2 ;
    }
    public int width ( ) { return this.x2 – this.x1 ; }
    public int height ( ) { return this.y2 – this.y1 ; }
    public double area ( ) { return this.width ( ) * this.height ( ) ; }
    public static void main ( String [ ] args ) {
        Rectangle rect1 = new Rectangle ( 0 , 0 , 10 , 10 ) ;
        System.out.println ( rect1.area ( ) ) ;
        Rectangle rect2 = new Rectangle ( 5 , 5 , 10 , 10 ) ;
        System.out.println ( rect2.area ( ) ) ;
    }
}
```