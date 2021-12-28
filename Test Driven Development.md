After watching this video, you will be able to define test-driven development
(TDD), describe how TDD produces higher-quality code, describe the Red, Green,
Refactor workflow, and describe the importance of TDD for DevOps. This is one of
my favorite quotes: “If it's worth building, it's worth testing. If it's not
worth testing, why are you wasting your time working on it?” Writing test cases
is critical to proving that your code works as intended. What is Test-Driven
Development? Test-Driven Development (TDD) means that your test case drives the
design and development of your code. You don't write code and then test it. You
write the test cases first. You write the tests for the code you wish you had,
then you write the code to make them pass. That may sound counterintuitive. How
can I write test cases for code I haven't written yet? How can you write a
design for code you haven't written yet? You describe in the design how the code
should behave and then you write the code that behaves that way. TDD is no
different. The test case describes the behavior that you want the code to have.
This keeps you focused on the purpose of the code, that is, what's it supposed
to do. You should absolutely be able to specify that before you start writing
any code. Otherwise, how do you know what to write? This is also what keeps you
focused on the clients that will call your code. I do a fair amount of backend
development. I love creating services for others to use. One day, I am creating
what I was sure would be an awesome service with a great Application Programming
Interface (API). I was down in the bowels of the code and I needed some
information, so I added it as a parameter to the API. Then I needed something
else, and I added that as another parameter to the API. Eventually, I needed
more things, so I added those as parameters too. Now it is time to write some
test cases for my code. At the time, I wasn’t following TDD. When I started
writing the test cases, I suddenly realized that I didn’t have half of the
information that my parameters required. My beautiful API was horrible! How
could it be this bad? Where had I gone wrong? I didn’t take the caller of my
code into account because I wasn’t following TDD. TDD gives you the caller’s
perspective. It allows you to explore how you would want to call the code before
even writing it. It makes you consider, "What do I know as a caller that I could
pass in and get an answer?" Having this perspective is critical to writing good
code. Code is of no use if no one can call it. Why don't developers write test
cases? I get these excuses all the time. The first excuse is: I already know my
code works! Yes, but others who work on your code in the future won’t know if
they broke something including the "future you!" I tell programmers that
whenever you clone or pull from a repo, the first thing you do is run the test
cases. How else do you know if you broke something or if it was broken before
you changed it? Test cases give you a baseline so that other people know that
the code is still working. Another one is: I don’t write broken code! Maybe you
don't write broken code, but the environment is constantly churning underneath
you. Vulnerabilities are being patched and new libraries are being upgraded so
your code may no longer work. Someone will say something like, “We have a
vulnerability in the Apache Struts library. Can we update it on our servers?”
Unless you have test cases that test your code and make sure that it works with
a new version of that library, you probably shouldn't do that. And not doing
that, as you may know, from the vulnerabilities that have happened at Equifax,
could be catastrophic! You have to write test cases so you can say with
confidence, "Let me run the test suite... yes, the new version of struts works
fine. Deploy it to production." My favorite excuse is I have no time! This is
the worst excuse because testing actually saves you time in the end. The time
you spend writing a few test cases now is going to save you hours and hours of
debugging later. Trust me on this one. You don't know who's going to use your
code in the future and you want to make sure your code is solid. TDD will keep
you writing solid code. This is the TDD workflow. You write a failing test case
(right?) for the code you wish you had. Then write just enough code to make it
pass. It doesn’t have to be perfect. It doesn't have to be pretty. It does have
to make the test pass. Then you refactor the code to make it better and increase
the quality. Finally, repeat the process. This is known as Red, Green, Refactor.
Many of the testing tools follow this scheme. These tools output failing test
cases in red and passing test cases in green. This is how Red, Green, Refactor
got its name. So why is TDD important to DevOps? First and foremost, it saves
time when developing. As you add new features to the code or changes to existing
features (right?), the test cases will quickly let you know if something broke.
It allows you to code faster because you are more confident. You don't have to
worry if a change you just made broke something. When you refactor code, you can
move much faster because you know the test cases will catch any changes in
behavior. TDD ensures that the code is working as you expected. If you write the
test cases first to define the behavior you want, you will know that you have
achieved that behavior when the tests pass. It also means that future changes
don’t break the code. Failing test cases will instantly alert you that someone
has introduced something that broke the code. Finally, and most importantly, in
order to create a DevOps pipeline (a CI/CD pipeline), all tests must be
automated unless you want to push bugs to production faster. A lot of companies
don't understand this. They want to automate using Continuous Integration (CI)
and Continuous Delivery (CD), without automating their test. Unfortunately, you
can't have a CI/CD pipeline without automating your tests. In this video, you
learned that: TDD means test case drives the design and development of code. TDD
allows you to develop faster and with more confidence. The Red, Green, Refactor
workflow has to do with red as a fail and green as a pass, and it increases the
quality of the code. In order to create a DevOps CI/CD pipeline, you must first
automate your testing.