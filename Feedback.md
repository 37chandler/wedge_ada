## Feedback

It certainly looks like you corrected any big upload errors since you just have some off-by-one issues. 

These large blocks of commented-out table names are concerning. It should be relatively easy for you to access these files
one at a time in a for loop. That makes your code *much* more sustainable than this brute force approach it seems like you
employed. It seems like you executed Task 1, though it'd be great to see something with a bit more control over it.

I agree with your reflections that we need more practice getting these big files to upload. I'll add that for next year. 

As I mentioned on Katherine's, Task 2 could be done a bit more efficiently, but there's nothing wrong with the slower, steadier approach you took. I like the 
`convert_bytes` function.

You had a file with the department lookups, so that could theoretically just be a `read_csv` followed by a `to_gbq` with just a little
additional info to make sure the file gets put in the correct table. Again, what you did works, just a hard way to do it. The rest of Task 3 looks good and 
my comments remain the same: there are easier ways, but what you did works.

I'll add you to the solutions repo. Go ahead and clone that and read that code. While the solutions don't use Pandas, they might point you in the
right direction for some of these issues. Nice job, this is complete. 

