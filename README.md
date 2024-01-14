# nlp-project2


### Notes
1. To create a lexicon, run the code here: notebooks/create-lexicon.ipynb
2. The lexicons are output to this folder: lexicon/


### To run code
1. Clone this repo: https://github.com/cristianochesi/e-MGs.git

2. Move the file `lexicon/WAB_pre.json` to the `e-MGs` repo.

3. Run this at the terminal:


python eMG_run.py -i "It is a kite, um I mean it’s a lot of people here having fun, somebody uh uh has a book in there, it is a house back there, the kid has a dog, sail, a sailboat I guess over there, another thing that’s in the air, a basket. The man is reading the poem. It is a dog here, he has a dog. The kite, it is a kite up there. Um there’s a husband is there, the mother’s there too. It’s a kite, somebody has a kite there." -l lexicon/WAB_pre.json  

This was the output:  
```bash
rs_repos/nolab/e-MGs  main ✗                                                                           348d1h ◒  
▶ python eMG_run.py -i "It is a kite, um I mean it’s a lot of people here having fun, somebody uh uh has a book in there, it is a house back there, the kid has a dog, sail, a sailboat I guess over there, another thing that’s in the air, a basket. The man is reading the poem. It is a dog here, he has a dog. The kite, it is a kite up there. Um there’s a husband is there, the mother’s there too. It’s a kite, somebody has a kite there." -l lexicon/WAB_pre.json
Input: "It is a kite, um I mean it’s a lot of people here having fun, somebody uh uh has a book in there, it is a house back there, the kid has a dog, sail, a sailboat I guess over there, another thing that’s in the air, a basket. The man is reading the poem. It is a dog here, he has a dog. The kite, it is a kite up there. Um there’s a husband is there, the mother’s there too. It’s a kite, somebody has a kite there."
Lexicon file:  lexicon/WAB_pre.json
Parameter file:  parameters/eMG_param_default.json
Silent:  False

---Derivation------------
step 1. Phase ROOT | EXPECTING T | MEM = <>
		Unknown word 'It' in the lexicon
		Lexical retrieval of the word 'It'
INPUT exhausted

---Offline-Measures------
Sentence: It is a kite, um I mean it’s a lot of people here having fun, somebody uh uh has a book in there, it is a house back there, the kid has a dog, sail, a sailboat I guess over there, another thing that’s in the air, a basket. The man is reading the poem. It is a dog here, he has a dog. The kite, it is a kite up there. Um there’s a husband is there, the mother’s there too. It’s a kite, somebody has a kite there.
Steps: 2
Pending items im mem: 0
Pending expectations: T
Prediction: UNGRAMMATICAL
Merge unexpected items: 0
Move failures: 0
Ambiguities: 0
MaxD: 0
MaxT: 0
SumT: 0
MaxS: 0
RelM: 0

---Online-Measures------
Sentence:	It	
ENCODING:	0	
INTEGRATION:	0	
RETRIEVAL:	0	
INTERVENTION:	0	
---Tree------------------
\begin{forest}
[ROOT , name=0]

%
\node[index] at (0) {0};
\node[outdex] at (0) {0};
\end{forest}
(base) 
rs_repos/nolab/e-MGs  main ✗                                                                           348d1h ◒  
▶ git status                                                                                           
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.DS_Store
	__pycache__/
	lexicon/WAB_post.json
	lexicon/WAB_pre.json

nothing added to commit but untracked files present (use "git add" to track)
(base) 
rs_repos/nolab/e-MGs  main ✗                                                                           348d1h ◒  
▶       
```