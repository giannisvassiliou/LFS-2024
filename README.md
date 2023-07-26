# LFS(Love-at-First-Sight) 
 The increasing number of large knowledge graphs
 now available online requires methods for their effective and
 efficient exploration. Most of these knowledge graphs offer
 online SPARQL endpoints for directly issuing queries. In a
 typical scenario, the users issue coarse exploratory queries at
 the beginning, refining them further in the sequel in order to
 find the answer to the question in mind. However, those coarse
 exploratory queries are hard to be answered as they usually
 involve many results and take too much time to be answered, or
 even worse they time out, limiting the exploration potential of
 the data they expose.
 In this paper, we present the LFS (Love-at-First-Sight) system, offering a unique solution to the aforementioned problem,
 enabling users to rapidly fast get example answers to such coarse
 exploratory queries. More specifically we define the problem of
 the first-sight query answering, a form of approximate query
 answering returning only a single example answer to the issued
 query. We provide an effective and efficient solution to the
 problem of the first-sight query answering through summaries
 generated based on past workloads. We experimentally show the
 big benefits of the proposed summaries as their size is minimal
 and they can efficiently provide answers to the first-sight query
 answering the problem, highly increasing the response time for
 query answering over online SPARQL endpoints.
 <p align="center">

</p>
<p align="center">
  <img src="https://github.com/giannisvassiliou/LFS-ICDE-2024/blob/main/Architecture.JPG?raw=true" alt="Sublime's custom image"/>
</p>

## LFS Parser

Firstly we need to create the data accessing the endpoint of the desired dataset. The creator.py script has <b> two </b> input arguments. It will create two files (given as arguments too). 
The input argument is the query log of the dataset we are interested in.

The First output file will be the answered queries from the endpoint. The second output file will be the corresponing queries for the previous answers
