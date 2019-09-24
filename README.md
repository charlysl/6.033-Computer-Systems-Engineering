# 6.033-Computer-Systems-Engineering
MIT OCW course 2009

At MIT recitation consists of reading a paper followed a group discussion. Given that I am self learning, I substitute the discussion with a relevant youtube video, ideally featuring the author (or, if not, somemone prominent) presenting or discussing the paper at hand.

## REC1 - Worse is Better

- the "ideal" of a software system is not about reaching perfection, but "The Right Thing"
- if implementation is simple, you will deliver much faster (or at all)
- if it has fewer features, it will need fewer resources, and more people will use it
- if people use it, they will ask for improvements, and it will end up being almost complete
- if simple, someone will be much more willing to improve it
- simple means it will rely more on what's already there, as opposed to being monolithic

### [Worse Is Better, for Better or for Worse](https://youtu.be/w3JkpQAbTA4)
A very interesting talk in youtube, which looks back at the paper from a contemporary perspective.

#### Main points:

Worse doesn't mean buggy, it actually means that simplicity allows robustness.  
If something is useful, it's sufficient.  
Make it fast to get feedback ASAP.  
Make is small so that we can throw it away if we have to.  


- A product must be useful and bug free
  - constraints force one to focus on what is most useful
  - it is better to have an underfeatured product that is rock solid, fast and small, than one that covers what an expert would consider the complete requirements
- A **small** product (or iteration) is:
  - easier to get right, and to throw away if wrong
  - if something is small you won't be as reluctant to throw it away if it doesn't work; plan to throw away your first design (Ken Thompson)
  - at the beginning you are at the state of greatest ignorance. If we decide everything at the beginning, we will be stuck later if we want to change it
  - there is a point at which refactoring will be impossible
  - we tend to overrate things we built ourselves, this is why feedback is so important
  - it is not instictive to manage scope, it is easy to be ambitious and hard to constraint yourself
  - a small product is easier to optimize if performance is a problem; it also likely to be faster to begin with
- Simplicity is measured by the number of things there are and by how much they are interconnected; it is how much you need to know
- The implementation is more important than the interface; this applies to UI too
  - speed of UI adds to its beauty, which is irrelevant if slow
  - usability is more important than beauty
- design is in every step of a product's lifecycle
  - waterfall is analysis step (what to do), design (how to do it), coding (doing it), and testing (feedback)

#### Some interesting historical examples:
- installing and playing with C++ on one's home computer back in the 90s was very easy; on the other hand, Smalltalk, which was designed for company workstations, was a pain. C++ won the day.
- the original wiki code (kicked off the editable web) was just 200 lines of Perl and almost naively simple. It didn't have anywhere closed to all the features an expert would have considered for it to be complete. Now we have a whole encyclopedia based on it.
- Google's interface was as simple as it gets. It was also insanely fast.

#### Some good quotes:
> *There are only two kinds of languages:  
> the ones everyone complains about, and the ones nobody uses.*  
> Bjarne Stroustrup

> *Uncertainty is an uncomfortable position,  
> but certainty is an absurd one.*  
> Voltaire
