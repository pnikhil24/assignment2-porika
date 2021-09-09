# assignment2-porika
This is Webapps Assignment-2
# Nikhil Porika
###### My favorite place Goa

Goa is Located on the **Western Ghats of Konkan**, Goa is known as the smallest and the fourth smallest populated state of India. Goa is bounded by Maharashtra to its north, eastern and southern boundaries were formed by Karnataka, while the western coast is formed by **Arabian Sea**.<br> I like it because it helps me to refresh, last time when i visited the place had good time and enjoyed alot.
 
 ---
 # Directions for traveling from Maryville to Goa
1. Book a flight ticket to Chichago from Kansas City
2. Start your journey to Kansas City from Maryville at least 4 hours before to your flight depature time.
    1. You may have some food at airport because the flight duration is 4+ hour.
    2. After reaching Chichago airport you may use public/private transport or you may hire a rental car.
    3. Book a motel or hotel base upon your interest, but book anything near to your favorite spot to reach quickly.
3. After refreshment, you are in your favorite place.

# list of items that should be brought to the favorite place
  - Clothes
  - Food
  - Money
  - Refreshments
  
  **[About Me](AboutMe.md)**

  ---

 # Food Items

Below are the Items to get Refreshments

| Food/Drinks | Location | Price |
| :---: | :---: | :---: |
| Butter Nan | Hydrabad | $15 |
| Milk Shake | Warangal | $8 |
| Kaju Barfi| Pistahouse | $7 |
| chocolate ice cream| Hanamkonda | $22 |

---
# Pithy Quotes


>"An eye for eye only ends up making the whole world blind."<br/>
>"The weak can never forgive. Forgiveness is the attribute of the strong."<br/>
>―Mahatma Gandhi

---
#  Code Fencing

>In computer programming, a string is traditionally a sequence of characters, either as a literal constant or as some kind of variable. The latter may allow its elements to be mutated and the length changed, or it may be fixed (after creation). A string is generally considered as a data type and is often implemented as an array data structure of bytes (or words) that stores a sequence of elements, typically characters, using some character encoding. String may also denote more general arrays or other sequence (or list) data types and structure

[Quick Data Link](https://en.wikipedia.org/wiki/String_(computer_science))


```
sstring s;
int n;

struct node
 {
    int l, r, par, link;
    map<char,int> next;
node (int l=0, int r=0, int par=-1)
        : l(l), r(r), par(par), link(-1) {}
    int len()  {  return r - l;  }
    int &get (char c) {
        if (!next.count(c))  next[c] = -1;
        return next[c];
    }

struct state {
    int v, pos;
    state (int v, int pos) : v(v), pos(pos)  {}
};
state ptr (0, 0);

state go (state st, int l, int r) {
    while (l < r)
        if (st.pos == t[st.v].len()) {
            st = state (t[st.v].get( s[l] ), 0);
            if (st.v == -1)  return st;
        }
        else {

            if (r-l < t[st.v].len() - st.pos)
                return state (st.v, st.pos + r-l);
            l += t[st.v].len() - st.pos;
        }
```
[Code Source](https://cp-algorithms.com/string/suffix-tree-ukkonen.htm)