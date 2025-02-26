Download Link : https://programming.engineering/product/shapeshifting-coloring-problems/

# Shapeshifting-Coloring-Problems
Shapeshifting Coloring Problems
In this assignment, you are given a PyGame environment (in the gridgame.py file) that renders an empty n × n grid. Your goal is to build an AI agent that solves a coloring problem over this grid (see next page for constraints).

Your agent will attempt to fill the environment by moving a virtual ‘brush’ over this grid and placing colored shapes, where the shape of the brush can be cycled through the following choices (numbered 0-8):

Additionally, each brush can be cycled through one of four colors (numbered 0-3).

If, despite my best efforts, the color choices here pose accessibility concerns, they may be edited in the gridgame.py file. Alternatively, please reach out to me, and I will be happy to implement an different palette.

Your agent will interact with the environment using the execute() function called from within the hw1.py file, with the following argument options (passed as strings):

    export: returns the current state of the grid, a list of shapes with positions and colors currently placed on the grid, and a Boolean indicating whether the coloring constraints have been satisfied.

    up/down/left/right: move the brush in the specified direction by one cell. The brush starts in the top left corner of the grid when the program is executed.

    place: place a shape on the grid, i.e. color the cells covered by the brush in the currently selected brush color.

    switchshape: cycle to the next brush shape option.

    switchcolor: cycle to the next brush color option.

    undo: undo the last placed shape.

Running the execute function with any argument returns the updated state of the grid, a list of placed shapes, and a Boolean indicating whether coloring constraints have been satisfied.

Your Task

Your goal is to build an AI agent that colors this grid using as few colors as possible, such that no two adjacent cells share a common color. Further, your goal is to achieve this coloring using as few shapes as possible – a larger brush may cover multiple cells, but counts as one shape. You may use any of the concepts we have discussed in class so far to implement your agent. Refer to hw1.py for further instructions.

Environment Rules: Adjacent cells are defined as cells that share an edge between them (i.e., diagonally neighboring cells may share the same color, since they only share a vertex). If a brush partially or fully overlaps with an area of the grid that is already colored, the execute function with the place argument will fail, i.e. the colors in those cells will not be overwritten.

Assignment Rules: Any hardcoded solutions, or attempts to leverage the autograder’s design to maximize points scored will result in an automatic zero on the assignment. An implement must make choices based on one or more concepts discussed in class. Imple-mentations must be optimized for good runtime – Gradescope has an autograder timeout of 10 minutes. Any submissions that do not finish executing in 10 minutes will be treated as incomplete, and will be evaluated for partial credit based on correctness.

Submission: Submit a zip file containing your completed hw1.py file, the provided gridgame.py file, and the grid.txt, shapes.txt and time.txt files produced in your working directory upon executing the homework script. Upload this zip file to Gradescope, and ensure the autograder runs as intended.

3
Solution
