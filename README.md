# What 2,000 Telegram Messages Reveal About Collectif Nemesis
The Feminist Right-Wing Group influencing French Politics.

Our dataset includes : social media communication from NemesisParis (all messages from their Telegram public channel) and social media communication from NousToutes (all descriptions of TikTok account).

We used pandas, regular expressions throughout analysis.

## Finding the most reoccurring words: NLTK and keyword analysis

Our first analysis of the dataset brought out the top 20 most reoccurring words within their public Telegram channel, and their weighted frequency, using nltk and spacy libraries.

We also did that for the NousToutes dataset.
This gave us an idea of the themes evoked in both groups: “women”, “violence”, “victim” were among the top words for both channels. For NemesisParis, the word “rape” is also among a top word, whereas for NousToutes, the word “VSS” (“Violences Sexistes et Sexuelles” , “Gender Based Violence” in French) is highly occurring. This gave us a first idea that where NousToutes mentions different kinds of gender based violence, NemesisParis focuses on instances of rape. NousToutes also uses altered spelling to evoke rape and violence, which could be an effort to bypass algorithmic censorship, or to discuss topics without triggering readers. We could not find any such altered spelling within NemesisParis’ content.

We also used nltk library to create a word cloud for NemesisParis, and then the spacy library to create a bar chart of the top 20 most reoccurring words.

## Ego-network and semantics

Using Meaningfully (a semantic search tool for text data in spreadsheets) to explore our datasets allowed us to formulate our hypothesis using the meaning of sentences, instead of keywords.

Using Meaningfully we found the following graphic language within NemesisParis’ communication: “meurtre, meurtri, frappe, tuméfié, gonflé, déformé, coups, hématomes, nue, corps, horreur, films, choquant, choc, viol, effroyable, supplice, bourreau, humiliée, sexe, ligotée, fellation, nourrisson, repère, suit, proie, dangerosité, irréparable, victime, exhibition, pénis, coups de poing, insultes, punition à genoux, claques, violences, suspendu par le bras, sa fille, bandes criminelles, faveurs sexuelles, brutalement, déshabillée, violée sur le trottoir, menaces de morts, sacrifiée, l'autel du vice, drame, actes de torture et de barbarie, viols en réunion, filmés et publiés sur le darkweb, insoutenable, pénétrations, rouée de coups par une autre jeune femme voilée, nique ta mère, baise, pute, chiennes en rut, calibres, sordide, horreurs, relations sexuelles avec des animaux, abominable, Orange mécanique, tabassée, extrêmement, longues minutes, couteau, menace, lynché, incapacité de bouger, 700 viols par sodomie, agréable à torturer, me consommer quand il voulait, ensanglanté, strangulations, contusions, dermabrasions, étranglée, tirée par les pieds, mordue, menacée de mort, glacent le sang, barbarie, hurlant.”

Hypothesis: the far-right feminist NemesisParis organisation communicates with more detailed accounts of sexual harassment cases towards women and girls, than left-wing feminist NousToutes group. They use more graphic, detailed and potentially triggering words.
There is also a pattern of re-sharing cases where the perpetrator was a foreigner, immigrant, under an “OQTF” (“Obligation de Quitter le Territoire Français”).

We then created a lexicon of words from our first list, expanding it with AI and creating categories. 

We found out how many times words from this lexicon appeared next to the dataset’s top reoccurring words (found in part 1).

This suggests the high frequency of messages where a particular sexual assault is being described in great details.

Going back to Meaningfully, we searched for the messages that contain this pattern, and found that in addition to gruesome details, the perpetrator’s identity and nationality was only disclosed according to certain conditions; when he was an immigrant, foreigner, or under “OQTF.” (This is only applicable when the perpetrator is not a public personality in France, as those events were equally shared by both NousToutes and NemesisParis).

METHODOLOGY

The choice of comparison (NousToutes vs NemesisParis) was made on the basis of active areas (Paris), and for their historical conflictual and oppositional relationship. We chose to use NousToutes’ TikTok account instead of its Telegram because its Telegram did not provide enough data. Limitations: a choice was made to analyse TikTok descriptions, rather than videos, for ease of analysis. We may have lost some data by only analysing descriptions. 
