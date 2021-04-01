# allegheny_county_2021_elections

this project matches all declared democrat and republican candidates to their respective position, using a list of all positions up for election in allegheny county's 2021 primaries and general election.

currently i've processed the municipal data. this means all candidates running for municipal positions, e.g. member of counsel, constable, commissioner. all municipalities primarily in allegheny county are included **except** pittsburgh.

finished-ish csvs:
+ candidate_list.csv:
  + a cleaned version of the unofficial declared candidate list available on allegheny county's website [here](https://www.alleghenycounty.us/elections/candidates.aspx)
+ all_muni_positions.csv
  + all municipal positions with candidates matched. only candidate names are included; party information can be found in candidate_list.csv.
+ no_candidates.csv
  + exactly what it sounds like; a subset of all_muni_positions including only the positions with no declared democrat or republican candidates. 
+ unopposed_candidates.csv
  + subset of all_muni_positions including cases where the number of candidates matches up to the number of available seats. e.g. one person running for mayor unopposed, three people running for three open commissioner seats.
+ not_enough_candidates.csv
  + subset of all_muni_positions including cases where 0 < number of candidates < number of seats. e.g. two people running for three open commissioner seats.

other stuff of note:
+ whos_running_for_what.ipynb
  + my data cleaning/analysis, done in python 3.8 using the package pandas

not-yet-asked questions:
+ why did you do this?
  + i'm unemployed. also i want the state to merge all municipalities into one big pittsburgh county like they did for philly. our municipal system is inefficient and corrupt.
+ are you gonna go back and finish the school director data? i see that you started it.
  + yeah probably. i have no sense of time. at some point in the next eon.
+ can i talk to you about this?
  + sure but for the love of g-d please don't email me. 
