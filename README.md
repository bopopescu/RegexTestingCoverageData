# ISSTA2018

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



