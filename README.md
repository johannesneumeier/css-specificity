CSS-SPECIFICITY MODULE
====================

wip - javascript module to calculate css specificity


TODO's:
=======
- detect style="" type of input
- handling of :not() pseudo selector


USAGE:
======
    Specificity.calculate("a > span .foobar");

returns an object with a values, matches and string attribute

    {
        values: {
    		a: 0,
    		b: 0,
    		c: 1,
    		d: 2
    	},
    	matches: {
    		a: [],
    		b: [],
    		c: [".foobar"],
    		d: ["a", "span"]
    	},
    	string: "0,0,1,2"
    }
