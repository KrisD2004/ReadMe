# Local Storage And How To Use It On Websites

https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/

## Adding state to the web: Why of local storage.

* One of the main problems with http as the main transport layer of the web is that it is statless.(Meaning that when you use an application and then close it, its state will be reset the next time you open it. If you close an application on your desktop and re-open it, its most recent state is restored.)
* This is the reason why as a software developer you need to store the state of your interface somewhere. 

## C Is For Cookie. Is That Good Enough For Me?

* The original way to do that is by using a cookie. **Cookie**nis a text file hosted on the users computer and connected to the domain that your webpage runs on. 
* Cookies do have limitations though: They add to the load of every document accessed on the domain. They allow up to only 4 KB of data storage. Because cookies have been used to spy on people’s surfing behavior, security-conscious people and companies turn them off or request to be asked every time whether a cookie should be set.

## The Dark Side Of Local Storage

* Any powerful technology comes with the danger of people abusing it for darker purposes. Samy, the man behind the “Samy is my hero” MySpace worm, recently released a rather scary demo called Evercookie, which shows how to exploit all kind of techniques, including local storage, to store information of a user on their computer even when cookies are turned off.


## Questions

1. Storing information locally on a user’s computer is a powerful strategy for a developer who is creating something for the Web.
2. Never store sensitive information in LocalStorage. This includes passwords, API Keys, authentication tokens like JWTs and financial information like credit card numbers, to name a few.This is info you should never store in local storage. 
3. LocalStorage always store key and value in string format. That is why you should convert your data to string whatever it is Array or Object. To Store data in localStorage first of all stringify it using JSON.stringify () method.
