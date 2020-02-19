# Regex Testing Coverage Data
file: data/stack_cov.csv
> "stack_regex" represents 15,096 regular expressions from 1,225 projects;

> "regex_index" refers to 13,632 syntactically unique regexes;

> "page" and "row"  combined locates a repo listed in RepoReaper;

> "type" shows what type of inputs used for calculating covered nodes,
> edges, and edge pairs. If "type" is equal to 1, it means the coverage
> data of this line is only for matching inputs; If equals to 2, it
> means the coverage for failing inputs. And "type" is 0 means combining
> all testing inputs.

> "count" represents the number of testing inputs used for testing coverage.

> "t_node" , "t_edge",  "t_epair"  represents the total nodes, edges,
> and edge pairs of the regex's DFA
> "c_node" , "c_edge" ,  "c_epair"  represents the covered nodes, edges,
> and edge pairs in the regex's DFA


dir: data/select_reporeaper

1)valid_repo_java---select all valid java repos

2)valid_repo_pom----select valid java repos which are maven projects and have at least one match results of "grep -nr "*.matches()", at least oone match results of "java.util.regex.*".

3)valid_pom_mvn-----select valid pom repos which could successfully execute "mvn test"

4)valid_pom_jar-----valid pom repos after changing pom.xml files

5)valid_pom_agent---valid pom repos which could execute "mvn test" with modified pom.xml files.


dir: data/res_regex

1)1.7------all regex after collecting data instrumentation information under JDK1.7

dir: data/log_regex

1)1.7------some instrumentation logs with collected raw regex information under JDK1.7


dir: data/res_regex_merge

1) from_to.regex, from_to.csv-------pickled results and csv results for repos from page "from" to page "to"

2) from_to.df-----------------------merged results of several from_to.regex

3) all.df---------------------------the results of all regex stack information

dir: data/rex_str

1) 1x--------10 rex-generated string samples with equivalent number of strings from repos
2) 5x--------5 rex-generated string samples with 5 times of strings from repos
3) 10x-------5 rex-generated string samples with 5 times of strings from repos
4) 20x-------5 rex-generated string samples with 5 times of strings from repos



