# assignment2-jamalapuram

# ARUN KUMAR JAMALAPURAM

###### Hyderabad

> Hyderabad is ruled by famous king Quli-qutubsha. It is **Beautiful** and **Pleasant** place to take vacation. More over it is my native place and I like the people and the relations with my family.


------

### Route To My Favourite Place
1. Maryville
2. Chicago
    1. Chicago Airport
    2. Terminal 1
    3. Flight
3. Hyderabad
* Dslr
    * BEST views
* Laptop
* Food
   * Paradise Biryani
   * Chicken Fry
**[LinkAboutme.md](Aboutme.md)**

# heading about creating a table food/drinks

Introduction:
The following is to  create a table with at least 4food/drinksthat you would recommend someone try.Include a short paragraph that introduces the table. 

 |Mandatory|fav1             |fav2                  |fav3              |fav4            | 
 |:-------:|:--------:       |:--------:            |:--------:        |:-------:       |
 |Food     |dosa             |biryani               |pizza             |coke            |
 |Location |hyderabad        |warangal              |karimnagar        |kukatpally      |
 |Type     |masala           |veg                   |spicy             |coacola         |
 |Amount   |30-40            |70-80                 |50-60             |20-30           |

  ----
  # quotes section
  >“Winners never quit, and quitters never win.”
  >Author:*Shane watson* <br>   
  >“Don't be pushed around by the fears in your mind. Be led by the dreams in your heart.”
  >Author:*Roy T. Bennett8* 

 ----
 # code fencing
 > "combinatorics is a range of linked studies which have something in common and yet diverge widely in their objectives, their methods, and the degree of coherence they have attained."[3] One way to define combinatorics is, perhaps, to describe its subdivisions with their problems and techniques. This is the approach that is used below. However, there are also purely historical reasons for including or not including some topics under the combinatorics umbrella.[4] Although primarily concerned with finite systems, some combinatorial questions and techniques can be extended to an infinite (specifically, countable) but discrete setting.quick-link to source code<https://en.wikipedia.org/wiki/Combinatorics>
 ```

vector<int> ans;

void gen(int n, int k, int idx, bool rev) {
    if (k > n || k < 0)
        return;

    if (!n) {
        for (int i = 0; i < idx; ++i) {
            if (ans[i])
                cout << i + 1;
        }
        cout << "\n";
        return;
    }

    ans[idx] = rev;
    gen(n - 1, k - rev, idx + 1, false);
    ans[idx] = !rev;
    gen(n - 1, k - !rev, idx + 1, true);
}

void all_combinations(int n, int k) {
    ans.resize(n);
    gen(n, k, 0, false);
}
```
quick link to source code<https://cp-algorithms.com/combinatorics/generating_combinations.html>
 
